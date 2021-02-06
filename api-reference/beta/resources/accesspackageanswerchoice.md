---
title: Tipo de recurso accessPackageAnswerChoice
description: Uma opção de resposta para um accessPackageMultipleChoiceQuestion.
author: markwahl-msft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 7c7fc7db1c9360146c2f62fd9048ad0db3d58b80
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135475"
---
# <a name="accesspackageanswerchoice-resource-type"></a>Tipo de recurso accessPackageAnswerChoice

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Indica uma opção de resposta para um [accessPackageMultipleChoiceQuestion](../resources/accesspackagemultiplechoicequestion.md). Vários accessPackageAnswerChoices podem ser adicionados a [um accessPackageMultipleChoiceQuestion](../resources/accesspackagemultiplechoicequestion.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|actualValue|String|O valor real da opção selecionada. Isso geralmente é um valor de cadeia de caracteres que pode ser entendido pelos aplicativos. Obrigatório. |
|displayValue|[accessPackageLocalizedContent](../resources/accesspackagelocalizedcontent.md)|Os valores de exibição localizados mostrados para o solicitante e os aprovadores. Obrigatório.

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageAnswerChoice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageAnswerChoice",
  "actualValue": "String",
  "displayValue": {
    "@odata.type": "microsoft.graph.accessPackageLocalizedContent"
  }
}
```
