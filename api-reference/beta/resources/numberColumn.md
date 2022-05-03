---
author: JeremyKelley
description: O recurso numberColumn em um recurso columnDefinition indica que os valores da coluna são números.
ms.date: 09/11/2017
title: NumberColumn
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: cloud-pc
ms.openlocfilehash: 8970c7a2526a4a29a3efe8e27759e81338013ed8
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176920"
---
# <a name="numbercolumn-resource-type"></a>Tipo de recurso NumberColumn

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso **numberColumn** em um recurso [columnDefinition](columndefinition.md) indica que os valores da coluna são números.

## <a name="json-representation"></a>Representação JSON

Aqui está uma representação JSON de um recurso **numberColumn**.

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.numberColumn" } -->

```json
{
  "decimalPlaces": "automatic | none | one | two | three | four | five",
  "displayAs": "number | percentage",
  "maximum": 10.551,
  "minimum": 99.993
}
```

## <a name="properties"></a>Propriedades

| Propriedade          | Tipo   | Descrição                                                                                                                |
| :---------------- | :----- | :------------------------------------------------------------------------------------------------------------------------- |
| **decimalPlaces** | string | Quantas casas decimais exibir. Consulte abaixo para saber mais sobre os valores possíveis.                                   |
| **displayAs**     | string | Como o valor deve ser apresentado na experiência do usuário. Deve ser `number` ou `percentage`. Se não for especificado, é tratado como `number`. |
| **maximum**       | double | O valor máximo permitido.                                                                                               |
| **minimum**       | double | O valor mínimo permitido.                                                                                               |

## <a name="decimalplaces-values"></a>Valores de DecimalPlaces

| Valor         | Descrição                                              |
| :------------ | :------------------------------------------------------- |
| **automatic** | Padrão. Exibir casas decimais automaticamente conforme necessário. |
| **none**      | Não exibir casas decimais.                       |
| **one**       | Exibir sempre uma casa decimal.                        |
| **two**       | Exibir sempre duas casas decimais.                       |
| **three**     | Exibir sempre três casas decimais.                     |
| **four**      | Exibir sempre quatro casas decimais.                      |
| **five**      | Exibir sempre cinco casas decimais.                      |

Observação: **decimalPlaces** e **displayAs** aplicam-se a como os números são processados, não armazenados.
Essas propriedades podem ser atualizadas.

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/NumberColumn",
  "suppressions": []
}
-->
