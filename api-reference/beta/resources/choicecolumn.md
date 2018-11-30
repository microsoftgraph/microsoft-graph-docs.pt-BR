---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ChoiceColumn
ms.openlocfilehash: 659ece2eab255fe7b55a258b0980eda4e7bde5b2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033156"
---
# <a name="choicecolumn-resource-type"></a>Tipo de recurso ChoiceColumn

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

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


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ChoiceColumn"
} -->
