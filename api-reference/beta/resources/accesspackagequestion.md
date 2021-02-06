---
title: Tipo de recurso accessPackageQuestion
description: O tipo complexo para perguntas configuradas em uma política de atribuição de pacote de acesso.
author: markwahl-msft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 04849b79cfa6c58132360f8ec20c363ea21453ec
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132374"
---
# <a name="accesspackagequestion-resource-type"></a>Tipo de recurso accessPackageQuestion

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Usado para a propriedade `accessPackageQuestion` de uma política de [atribuição de pacote de acesso.](accesspackageassignmentpolicy.md) 

Os subtipos [incluem accessPackageTextInputQuestions](accesspackagetextinputquestion.md) e [accessPackageMultipleChoiceQuestions](accesspackagemultiplechoicequestion.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String| ID da pergunta.|
|isRequired|Booliano| Se o solicitante precisa fornecer uma resposta ou não.|
|sequence|Int32| Posição relativa dessa pergunta ao exibir uma lista de perguntas para o solicitante.|
|texto|[accessPackageLocalizedContent](../resources/accesspackagelocalizedcontent.md)|O texto da pergunta a ser mostre ao solicitante.|

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

