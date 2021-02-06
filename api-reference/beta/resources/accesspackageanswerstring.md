---
title: Tipo de recurso accessPackageAnswerString
description: Uma resposta de cadeia de caracteres para um accessPackageTextInputQuestion
author: markwahl-msft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: def7753e62239e403821ed6472b3613d025942ac
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132388"
---
# <a name="accesspackageanswerstring-resource-type"></a>Tipo de recurso accessPackageAnswerString

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Indica a resposta de entrada de cadeia de caracteres para [um accessPackageTextInputQuestion](../resources/accesspackagetextinputquestion.md). Armazenado em um [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md).

Herda de [accessPackageAnswer](../resources/accesspackageanswer.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|answeredQuestion|[accessPackageQuestion](../resources/accesspackagequestion.md)|A pergunta à que a resposta se aplica. Herdado de [accessPackageAnswer](../resources/accesspackageanswer.md).|
|displayValue|String|Os valores de exibição localizados mostrados para o solicitante e os aprovadores. Herdado de [accessPackageAnswer](../resources/accesspackageanswer.md).|
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

