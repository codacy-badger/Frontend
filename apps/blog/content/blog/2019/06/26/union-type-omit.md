---
title: 'Omit types'
date: '2019-06-26T01:18:00+09:00'
---

# TL;DR

- TypeScriptで　`Omit` がサポートされた
- Union typesから `Omit` する難易度が高い

## formik-material-ui

- <https://github.com/stackworx/formik-material-ui/pull/82>
  - 公式の `Omit` はUnionTypesでもサポートしてるっぽい？🤔
- <https://github.com/microsoft/TypeScript/issues/28791>
  - もともと、 UnionTYpesからOmitするためには全部入りみたいな状態にしてそいつを対象にPick, Excludeしている？
- <https://github.com/sindresorhus/type-fest/blob/master/source/omit.d.ts#L17>
  - type-festはunion 　 typeのことは考慮できていない？