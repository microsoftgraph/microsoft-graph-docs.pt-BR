---
title: tipo de recurso accessPackageAnswerChoice
description: Uma opção de resposta para um accessPackageMultipleChoiceQuestion.
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6f34656a72d217adec1ff46be689b283461332fb
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720083"
---
# <a name="accesspackageanswerchoice-resource-type"></a>tipo de recurso accessPackageAnswerChoice

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Indica uma opção de resposta para um [accessPackageMultipleChoiceQuestion](../resources/accesspackagemultiplechoicequestion.md). Vários accessPackageAnswerChoices podem ser adicionados a um [accessPackageMultipleChoiceQuestion](../resources/accesspackagemultiplechoicequestion.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|realvalue|Cadeia de caracteres|O valor real da escolha selecionada. Normalmente, esse é um valor de cadeia de caracteres que é compreensível por aplicativos. Obrigatório. |
|displayValue|[accessPackageLocalizedContent](../resources/accesspackagelocalizedcontent.md)|Os valores de exibição localizados mostrados para o solicitante e aprovadores. Obrigatório.

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
