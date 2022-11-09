---
title: "`complementary`"
description: "Как добавить ориентир для дополнительного содержимого с помощью WAI-ARIA."
authors:
  - doka-dog
keywords:
  - доступность
  - ARIA
  - ARIA-роль
  - ориентир
  - aside
related:
  - a11y/aria-intro
  - a11y/aria-roles
  - html/aside
tags:
  - doka
  - placeholder
---

## Кратко

[ARIA-роль ориентира](/a11y/aria-roles/#roli-orientirov). Определяет область с дополнительным содержимым, которое не теряет смысл без основного. К примеру, боковая колонка на странице.

Роль `complementary` есть у [`<aside>`](/html/aside/) по умолчанию.

## Пример

```html
<div role="complementary">
  <h2>Популярные статьи</h2>
  <ul>
    <li>
      <a href="#">5 признаков того, что кот вас любит</a>
    </li>
    <li>
      <a href="#">Популярные фасоны шляп для лягушек</a>
    </li>
    <li>
      <a href="#">Вяжем носки для морских свинок</a>
    </li>
  </ul>
</div>
```

## Как пишется

Добавьте к тегу `role="complementary"`. Лучше, чтобы это были семантически нейтральные [`<div>`](/html/div/) или [`<span>`](/html/span/). Одно из [правил использования ARIA](/a11y/aria-intro/#pravila-ispolzovaniya) — не перезаписывать роли без необходимости.

В большинстве случаев лучше использовать `<aside>` вместо роли `complementary`.

Для элемента с ролью `complementary` можно использовать все [глобальные ARIA-атрибуты](/a11y/aria-attrs/#globalnye-atributy).

## Как понять

Роль `complementary` создаёт ориентир на странице. Это значит, что пользователи скринридеров могут быстро переместиться к этой части страницы с помощью горячих клавиш или через меню со всеми ориентирами.