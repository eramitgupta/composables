# 🔥 useFlashMessages – Vue Composable for Flash Toasts

A simple composable that shows flash messages using [vue-toastification](https://github.com/Maronato/vue-toastification).

---

## 📦 Installation

Make sure you have [vue-toastification](https://github.com/Maronato/vue-toastification) installed:

```bash
npm install vue-toastification
```

---

## ⚙️ Usage

### 1. Import the composable

```js
import { useFlashMessages } from "@/composables/useFlashMessages";
```

### 2. Use inside your component

```js
const { showFlashMessages } = useFlashMessages();

onMounted(() => {
    showFlashMessages();
});
```

---

## 💡 What It Does

- Automatically reads flash messages (e.g., from `window.flash` or a similar source).
- Uses `vue-toastification` to display them as toast notifications.
- Clean and reusable – follows Vue Composition API standards.
