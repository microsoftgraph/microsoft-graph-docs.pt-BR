---
title: Tipo de recurso accessPackageTextInputQuestion
description: Filho de accessPackageQuestion que tem entrada de texto como o formato de resposta da pergunta.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 0dee144139113716257ee1f41b6e585d22dc26b9
ms.sourcegitcommit: 2d61a35735aeb060cc9f7374dd6b50900566293b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2022
ms.locfileid: "62468277"
---
# <a name="accesspackagetextinputquestion-resource-type"></a>Tipo de recurso accessPackageTextInputQuestion

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um filho de **accessPackageQuestion** que tem entrada de texto como resposta.  Isso é usado na propriedade **questions** de [um accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) e dentro de [um accessPackageResourceAttribute de](accesspackageresourceattribute.md) um recurso de pacote de acesso.

Herda de [accessPackageQuestion](../resources/accesspackagequestion.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|ID da pergunta. Herdado [de accessPackageQuestion](../resources/accesspackagequestion.md).|
|isRequired|Booliano|Indica se o solicitante é necessário para fornecer uma resposta ou não. Herdado [de accessPackageQuestion](../resources/accesspackagequestion.md).|
|isSingleLineQuestion|Boolean|Indica se a resposta estará no formato de linha única ou múltipla.|
|sequence|Int32|Posição relativa dessa pergunta ao exibir uma lista de perguntas para o solicitante. Herdado [de accessPackageQuestion](../resources/accesspackagequestion.md).|
|texto|[accessPackageLocalizedContent](../resources/accesspackagelocalizedcontent.md)|O texto da pergunta a ser mostrar ao solicitante. Herdado [de accessPackageQuestion](../resources/accesspackagequestion.md).|

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

