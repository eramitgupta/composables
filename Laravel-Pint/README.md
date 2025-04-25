# 🧹 Laravel Pint Code Style – Custom Configuration

This project uses a customized **Laravel Pint** configuration to enforce consistent, clean, and modern PHP code style.

---

## 🧾 Preset

We use the **`laravel`** preset as the base, which aligns with the official Laravel coding standards.

```json
"preset": "laravel"
```

---

## 🛠 Custom Rules Enabled

| Rule | Description |
|------|-------------|
| `array_push` | Use `$array[] = $value` instead of `array_push()` for better readability. |
| `backtick_to_shell_exec` | Convert backtick operators to `shell_exec()`. |
| `date_time_immutable` | Enforce using `DateTimeImmutable` instead of `DateTime`. |
| `lowercase_keywords` | Ensures all PHP keywords are lowercase. |
| `lowercase_static_reference` | Use lowercase `self`, `static`, `parent` references. |
| `global_namespace_import` | Auto-import classes, constants, and functions from the global namespace. |
| `mb_str_functions` | Enforce using `mb_` string functions (multi-byte safe). |
| `modernize_types_casting` | Use modern casting syntax like `(int) $var` instead of `intval()`. |
| `new_with_parentheses: false` | Allow object creation without parentheses (`new Class` instead of `new Class()`). |
| `no_superfluous_elseif` | Simplify nested `elseif` statements when possible. |
| `no_useless_else` | Remove `else` after `return` or `throw`. |
| `no_multiple_statements_per_line` | Enforce one statement per line. |
| `ordered_class_elements` | Define custom order for class members (traits, constants, properties, methods). |
| `ordered_interfaces` | Alphabetically order interfaces in `implements`. |
| `ordered_traits` | Alphabetically order traits in `use`. |
| `protected_to_private` | Convert unused `protected` to `private`. |
| `self_accessor` | Use `self::` instead of class name inside the class. |
| `self_static_accessor` | Use `self::` for static calls inside the class. |
| `strict_comparison` | Enforce `===` and `!==` for strict comparison. |
| `visibility_required` | Require visibility on all class properties and methods. |

---

## 📦 Using Laravel Pint

### 📁 File

Create a file in your project root: `pint.json`


### ▶️ Run Pint

```bash
./vendor/bin/pint
```

or with verbose output:

```bash
./vendor/bin/pint --test
```

---

## ✅ Benefits

- Consistent coding standards
- Modern PHP practices
- Cleaner and more maintainable code
- Ready for team collaboration and open source
