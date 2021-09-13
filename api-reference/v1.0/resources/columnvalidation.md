---
author: swapnil1993
title: tipo de recurso columnValidation
description: Contém dados que validam valores de coluna.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: a2c5b464b7f08fcd1de078b94b5ca1b039b6a6f9
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59062786"
---
# <a name="columnvalidation-resource-type"></a>tipo de recurso columnValidation

Namespace: microsoft.graph

Representa propriedades que validam valores de coluna.
## <a name="properties"></a>Propriedades

| Nome da propriedade  | Tipo    | Descrição|
|:---------------|:--------|:--------------------------------------------------|
| **formula**    | string  | A fórmula para validar o valor da coluna. Por exemplos, consulte [Exemplos de fórmulas comuns em listas](https://support.microsoft.com/office/examples-of-common-formulas-in-sharepoint-lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3).|
| **descriptions**    | Collection(microsoft.graph.displayNameLocalization)  | Mensagens localizadas que explicam o que é necessário para que o valor dessa coluna seja considerado válido. O usuário será solicitado com essa mensagem se a validação falhar. |
| **defaultLanguage**    | cadeia de caracteres  | Marca de idioma padrão BCP 47 para a descrição.|

As fórmulas do SharePoint usam uma sintaxe semelhante a fórmulas do Excel.
Para obter mais informações, [consulte Exemplos de fórmulas comuns em SharePoint Lists][SPFormulas].

## <a name="json-representation"></a>Representação JSON

A seguir está uma representação JSON de um **recurso columnValidation.**
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.columnValidation"} -->

```json
{
  "formula": "string",
  "descriptions": [{ "@type": "microsoft.graph.displayNameLocalization" }],
  "defaultLanguage": "string"
}
```

[SPFormulas]: https://support.office.com/article/Examples-of-common-formulas-in-SharePoint-Lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3
