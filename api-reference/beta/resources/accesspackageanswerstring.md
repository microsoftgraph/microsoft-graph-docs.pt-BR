---
title: tipo de recurso accessPackageAnswerString
description: Uma resposta de cadeia de caracteres para um accessPackageTextInputQuestion
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4a5273872b2ded749ddfc13998c5b0104a0a63ec
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720039"
---
# <a name="accesspackageanswerstring-resource-type"></a>tipo de recurso accessPackageAnswerString

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Indica a resposta de entrada da cadeia de caracteres para um [accessPackageTextInputQuestion](../resources/accesspackagetextinputquestion.md). Armazenado em um [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md).

Herda de [accessPackageAnswer](../resources/accesspackageanswer.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|answeredQuestion|[accessPackageQuestion](../resources/accesspackagequestion.md)|A pergunta à qual a resposta se aplica. Herdado de [accessPackageAnswer](../resources/accesspackageanswer.md).|
|displayValue|Cadeia de caracteres|Os valores de exibição localizados mostrados para o solicitante e aprovadores. Herdado de [accessPackageAnswer](../resources/accesspackageanswer.md).|
|value|Cadeia de caracteres|O valor armazenado no perfil de usuário do solicitante, se essa resposta estiver configurada para ser armazenada como um atributo específico.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageAnswerString"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageAnswerString",
  "displayValue": "String",
  "answeredQuestion": {
    "@odata.type": "microsoft.graph.accessPackageQuestion"
  },
  "value": "String"
}
```

