---
title: tipo de recurso accessPackageTextInputQuestion
description: Filho de accessPackageQuestion que tem entrada de texto como o formato de resposta da pergunta.
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8609532e096fb587b4dcf49b8eb624aea314a8c6
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720051"
---
# <a name="accesspackagetextinputquestion-resource-type"></a>tipo de recurso accessPackageTextInputQuestion

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um filho de **accessPackageQuestion** que tem entrada de texto como resposta.

Herda de [accessPackageQuestion](../resources/accesspackagequestion.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|ID da pergunta. Herdado de [accessPackageQuestion](../resources/accesspackagequestion.md).|
|isRequired|Booliano|Indica se o solicitante é necessário para fornecer uma resposta ou não. Herdado de [accessPackageQuestion](../resources/accesspackagequestion.md).|
|isSingleLineQuestion|Booliano|Indica se a resposta estará em um formato de linha única ou múltipla.|
|sequence|Int32|Posição relativa desta pergunta ao exibir uma lista de perguntas para o solicitante. Herdado de [accessPackageQuestion](../resources/accesspackagequestion.md).|
|texto|[accessPackageLocalizedContent](../resources/accesspackagelocalizedcontent.md)|O texto da pergunta a ser mostrado para o solicitante. Herdado de [accessPackageQuestion](../resources/accesspackagequestion.md).|

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

