---
author: JeremyKelley
description: O choiceColumn em um recurso columnDefinition indica que os valores da coluna podem ser selecionados em uma lista de opções.
ms.date: 09/11/2017
title: ChoiceColumn
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: d7c2e1292bc3868b188b9389a0c44477606cbb3e
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/22/2022
ms.locfileid: "63722252"
---
# <a name="choicecolumn-resource-type"></a>Tipo de recurso ChoiceColumn

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O **choiceColumn** em um recurso [columnDefinition](columndefinition.md) indica que os valores da coluna podem ser selecionados em uma lista de opções.

## <a name="json-representation"></a>Representação JSON

Aqui está uma representação JSON de um recurso **choiceColumn**.

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.choiceColumn" } -->

```json
{
  "allowTextEntry": true,
  "choices": ["red", "blue", "green"],
  "displayAs": "checkBoxes | dropDownMenu | radioButtons"
}
```

## <a name="properties"></a>Propriedades

| Propriedade           | Tipo               | Descrição                                                                                                   |
| :----------------- | :----------------- | :------------------------------------------------------------------------------------------------------------ |
| **allowTextEntry** | booliano            | Se verdadeiro, permite valores personalizados que não estão em opções configuradas.                                          |
| **choices**        | collection(string) | A lista de valores disponíveis para essa coluna.                                                                 |
| **displayAs**      | string             | Como as opções devem ser apresentadas na UX. Deve ser `checkBoxes`, `dropDownMenu` ou `radioButtons` |

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ChoiceColumn",
  "suppressions": []
}
-->
