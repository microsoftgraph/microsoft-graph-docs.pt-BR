---
author: JeremyKelley
description: O choiceColumn em um recurso columnDefinition indica que os valores da coluna podem ser selecionados em uma lista de opções.
ms.date: 09/11/2017
title: ChoiceColumn
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 72ef8adb96614fc32b9aee8141eb19248e963639
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973482"
---
# <a name="choicecolumn-resource-type"></a>Tipo de recurso ChoiceColumn

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

| Nome da propriedade      | Tipo               | Descrição
|:-------------------|:-------------------|:----------------------------------------------
| **allowTextEntry** | booliano            | Se verdadeiro, permite valores personalizados que não estão em opções configuradas.
| **choices**        | collection(string) | A lista de valores disponíveis para essa coluna.
| **displayAs**      | string             | Como as opções devem ser apresentadas na UX. Deve ser `checkBoxes`, `dropDownMenu` ou `radioButtons`


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
