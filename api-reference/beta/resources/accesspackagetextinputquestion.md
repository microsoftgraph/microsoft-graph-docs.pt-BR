---
title: Tipo de recurso accessPackageTextInputQuestion
description: Filho de accessPackageQuestion que tem entrada de texto como formato de resposta da pergunta.
author: markwahl-msft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 5f7d4d0ee7517ec3455d9e63647461e8101cab9d
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133571"
---
# <a name="accesspackagetextinputquestion-resource-type"></a>Tipo de recurso accessPackageTextInputQuestion

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um filho de **accessPackageQuestion** que tem entrada de texto como resposta.

Herda de [accessPackageQuestion](../resources/accesspackagequestion.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|ID da pergunta. Herdado [de accessPackageQuestion](../resources/accesspackagequestion.md).|
|isRequired|Booliano|Indica se o solicitante é obrigado a fornecer uma resposta ou não. Herdado [de accessPackageQuestion](../resources/accesspackagequestion.md).|
|isSingleLineQuestion|Boolean|Indica se a resposta estará no formato de uma ou várias linhas.|
|sequence|Int32|Posição relativa dessa pergunta ao exibir uma lista de perguntas para o solicitante. Herdado [de accessPackageQuestion](../resources/accesspackagequestion.md).|
|texto|[accessPackageLocalizedContent](../resources/accesspackagelocalizedcontent.md)|O texto da pergunta a ser mostre ao solicitante. Herdado [de accessPackageQuestion](../resources/accesspackagequestion.md).|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageTextInputQuestion"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageTextInputQuestion",
  "id": "String (identifier)",
  "isRequired": "Boolean",
  "text": {
    "@odata.type": "microsoft.graph.accessPackageLocalizedContent"
  },
  "sequence": "Integer",
  "isSingleLineQuestion": "Boolean"
}
```

