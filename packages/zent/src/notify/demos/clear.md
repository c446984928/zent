---
order: 5
zh-CN:
	title: 清除屏幕所有通知
	success: 成功通知
	clear: 清除通知
en-US:
	title: Clear all nofications in screen
	success: notify success
	clear: notify clear

---

```jsx
import { Notify, Button } from 'zent';

function closeCallback() {
	alert('Callback has call');
}

ReactDOM.render(
	<div>
		<Button onClick={() => Notify.success('{i18n.success}', 2000, closeCallback)}>{i18n.success}</Button>
		<Button onClick={() => Notify.clear()}>{i18n.clear}</Button>
	</div>
	, mountNode
);

```
