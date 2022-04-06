---
author: swapnil1993
title: tipo de recurso columnValidation
description: Contém dados que validam valores de coluna.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 41136c74347e0acdfe41b5b8fd9a5ddc1501a08b
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2022
ms.locfileid: "63757847"
---
# <a name="columnvalidation-resource-type"></a>tipo de recurso columnValidation

Namespace: microsoft.graph

Representa propriedades que validam valores de coluna.
## <a name="properties"></a>Propriedades

| Propriedade  | Tipo    | Descrição|
|:---------------|:--------|:--------------------------------------------------|
| **formula**    | string  | A fórmula para validar o valor da coluna. Por exemplos, consulte [Exemplos de fórmulas comuns em listas](https://support.microsoft.com/office/examples-of-common-formulas-in-sharepoint-lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3).|
| **descriptions**    | Collection(microsoft.graph.displayNameLocalization)  | Mensagens localizadas que explicam o que é necessário para que o valor dessa coluna seja considerado válido. O usuário será solicitado com essa mensagem se a validação falhar. |
| **defaultLanguage**    | cadeia de caracteres  | Marca de idioma padrão BCP 47 para a descrição.|

As fórmulas do SharePoint usam uma sintaxe semelhante a fórmulas do Excel.
Para obter mais informações, [consulte Exemplos de fórmulas comuns em SharePoint Lists][SPFormulas].

## <a name="json-representation"></a>Representação JSON

A seguir está uma representação JSON de um **recurso columnValidation** .
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.columnValidation"} -->

```json
{
  "formula": "string",
  "descriptions": [{ "@type": "microsoft.graph.displayNameLocalization" }],
  "defaultLanguage": "string"
}
```

[SPFormulas]: https://support.office.com/article/Examples-of-common-formulas-in-SharePoint-Lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3
