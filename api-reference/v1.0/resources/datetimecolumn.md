---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: DateTimeColumn
ms.openlocfilehash: ce5f06b6e0d88324813372c2431b62e6b9105bcb
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2017
---
# <a name="datetimecolumn-resource-type"></a>Tipo de recurso DateTimeColumn

**dateTimeColumn** em um recurso [columnDefinition](columnDefinition.md) indica que os valores da coluna são datas ou horas.

## <a name="json-representation"></a>Representação JSON

Aqui está uma representação JSON de um recurso **dateTimeColumn**.
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.dateTimeColumn" } -->

```json
{
  "displayAs": "default | friendly | standard",
  "format": "dateOnly | dateTime"
}
```

## <a name="properties"></a>Propriedades

| Nome da propriedade      | Tipo               | Descrição
|:-------------------|:-------------------|:----------------------------------------------
| **displayAs**      | string             | Como o valor deve ser apresentado na experiência do usuário. Deve ser `default`, `friendly` ou `standard`. Consulte abaixo para ver mais detalhes. Se não for especificado, é tratado como `default`.
| **format**         | string             | Indica se o valor deve ser apresentado como apenas uma data ou uma data e hora. Deve ser `dateOnly` ou `dateTime`

## <a name="displayas-values"></a>Valores de displayAs

| Valor        | Descrição
|:-------------|:--------------------------------------------------------------
| **default**  | Usa o processamento de renderização padrão na UX.
| **amigável** | Usa uma representação amigável relativa (ex. "hoje às 15:00")
| **standard** | Usa a representação padrão absoluta (ex. "10/05/2017 15:20")


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/DateTimeColumn"
} -->
