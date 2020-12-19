---
title: tipo de recurso accessPackageQuestion
description: O tipo complexo para perguntas configuradas em uma política de atribuição de pacote do Access.
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 876c21018104ed579cbaf04b0f4642395627964e
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720068"
---
# <a name="accesspackagequestion-resource-type"></a>tipo de recurso accessPackageQuestion

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Usada para a `accessPackageQuestion` propriedade de uma [política de atribuição de pacote do Access](accesspackageassignmentpolicy.md). 

Os subtipos incluem [accessPackageTextInputQuestions](accesspackagetextinputquestion.md) e [accessPackageMultipleChoiceQuestions](accesspackagemultiplechoicequestion.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres| ID da pergunta.|
|isRequired|Booliano| Se o solicitante é necessário para fornecer uma resposta ou não.|
|sequence|Int32| Posição relativa desta pergunta ao exibir uma lista de perguntas para o solicitante.|
|texto|[accessPackageLocalizedContent](../resources/accesspackagelocalizedcontent.md)|O texto da pergunta a ser mostrado para o solicitante.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageQuestion"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageQuestion",
  "id": "String (identifier)",
  "isRequired": "Boolean",
  "text": {
    "@odata.type": "microsoft.graph.accessPackageLocalizedContent"
  },
  "sequence": "Integer"
}
```

