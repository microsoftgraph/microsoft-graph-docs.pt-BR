---
author: swapnil1993
title: tipo de recurso columnValidation
description: Contém dados para validar valores de coluna.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 20bf526aff4f10b0b9b16a31e9912b5695602db6
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/22/2022
ms.locfileid: "63721721"
---
# <a name="columnvalidation-resource-type"></a>tipo de recurso columnValidation

Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
Contém metadados para validar a coluna.

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo                                                | Descrição                                                                                                                                                                                                               |
| :------------------ | :-------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **formula**         | string                                              | A fórmula para validar o valor da coluna. Por exemplos, consulte [Exemplos de fórmulas comuns em listas](https://support.microsoft.com/office/examples-of-common-formulas-in-sharepoint-lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3) |
| **descriptions**    | Collection(microsoft.graph.displayNameLocalization) | Mensagens localizadas que explicam o que é necessário para que o valor dessa coluna seja considerado válido. O usuário será solicitado com essa mensagem se a validação falhar.                                                               |
| **defaultLanguage** | string                                              | Marca de idioma padrão BCP 47 para a descrição.                                                                                                                                                                          |

As fórmulas do SharePoint usam uma sintaxe semelhante a fórmulas do Excel.
Consulte [Exemplos de fórmulas comuns em listas do SharePoint][SPFormulas] para obter mais informações.

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
