---
title: Propsの使い方
description: プロップスとその使い方
publishDate: "2025-10-05T19:00:00+09:00"
---

## Propsの使い方について

I.e., instead of
```
1. <CoreConcept
2.   title={CORE_CONCEPTS[0].title}
3.   description={CORE_CONCEPTS[0].description}  
4.   image={CORE_CONCEPTS[0].image} />
```
or
```
1. <CoreConcept
2.   {...CORE_CONCEPTS[0]} />
```

you could also pass a single `concept` (or any name of your choice) prop to the `CoreConcept` component:
```
1. <CoreConcept
2.   concept={CORE_CONCEPTS[0]} />
```

In the `CoreConcept` component, you would then get that one single prop:
```
1. export default function CoreConcept({ concept }) {
2.   // Use concept.title, concept.description etc.
3.   // Or destructure the concept object: const { title, description, image } = concept;
4. }
```

## Propsとは

propertyを省略したもので詳細情報や設定、状態を指す。