---
title: Tipo de recurso accessPackageMultipleChoiceQuestion
description: Subclasse de accessPackageQuestion que tem várias opções como o formato de resposta da pergunta
author: markwahl-msft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 54054edcda2f41ad3f4e1bd29fb807c18709ee1d
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137337"
---
# <a name="accesspackagemultiplechoicequestion-resource-type"></a>Tipo de recurso accessPackageMultipleChoiceQuestion

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um filho de **accessPackageQuestion** que apresenta várias opções das quais o solicitante deve escolher uma resposta.

Herda de [accessPackageQuestion](../resources/accesspackagequestion.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|allowsMultipleSelection|Boolean|Indica se o solicitante pode selecionar várias opções como resposta.|
|choices|[coleção accessPackageAnswerChoice](../resources/accesspackageanswerchoice.md)|Lista de opções de resposta.|
|id|String|ID da pergunta. Herdado [de accessPackageQuestion](../resources/accesspackagequestion.md).|
|isRequired|Booliano|Indica se o solicitante é obrigado a fornecer uma resposta ou não. Herdado [de accessPackageQuestion](../resources/accesspackagequestion.md).|
|sequence|Int32|Posição relativa dessa pergunta ao exibir uma lista de perguntas para o solicitante. Herdado [de accessPackageQuestion](../resources/accesspackagequestion.md).|
|texto|[accessPackageLocalizedContent](../resources/accesspackagelocalizedcontent.md)|O texto da pergunta para mostrar o solicitante. Herdado [de accessPackageQuestion](../resources/accesspackagequestion.md).|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageMultipleChoiceQuestion"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageMultipleChoiceQuestion",
  "id": "String (identifier)",
  "isRequired": "Boolean",
  "text": {
    "@odata.type": "microsoft.graph.accessPackageLocalizedContent"
  },
  "sequence": "Integer",
  "choices": [
    {
      "@odata.type": "microsoft.graph.accessPackageAnswerChoice"
    }
  ],
  "allowsMultipleSelection": "Boolean"
}
```
