---
author: swapnil1993
title: tipo de recurso columnValidation
description: Contém dados para validar valores de coluna.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 8c1b20b239b894aa0da63222bb69a8d720e5ab50
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445929"
---
# <a name="columnvalidation-resource-type"></a>tipo de recurso columnValidation

Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
Contém metadados para validar a coluna.


## <a name="properties"></a>Propriedades

| Nome da propriedade  | Tipo    | Descrição
|:---------------|:--------|:--------------------------------------------------
| **formula**    | string  | A fórmula para validar o valor da coluna. Por exemplos, consulte [Exemplos de fórmulas comuns em listas](https://support.microsoft.com/office/examples-of-common-formulas-in-sharepoint-lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3) 
| **descriptions**    | Collection(microsoft.graph.displayNameLocalization)  | Mensagens localizadas que explicam o que é necessário para que o valor dessa coluna seja considerado válido. O usuário será solicitado com essa mensagem se a validação falhar. 
| **defaultLanguage**    | string  | Marca de idioma padrão BCP 47 para a descrição.

As fórmulas do SharePoint usam uma sintaxe semelhante a fórmulas do Excel.
Consulte [Exemplos de fórmulas comuns em listas do SharePoint][SPFormulas] para obter mais informações.

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
