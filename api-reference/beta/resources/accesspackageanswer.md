---
title: tipo de recurso accessPackageAnswer
description: O tipo complexo para as respostas a um accessPackageQuestion que são armazenadas em um accessPackageAssignmentRequest.
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f947c5235c18d3be5115199d789512602a3e0739
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720071"
---
# <a name="accesspackageanswer-resource-type"></a>tipo de recurso accessPackageAnswer

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O tipo complexo de uma resposta fornecida pelo solicitante para um [accessPackageQuestion](../resources/accesspackagequestion.md). A resposta real será um subtipo desse tipo complexo, seja [accessPackageAnswerString](../resources/accesspackageanswerstring.md) ou [accessPackageAnswerChoice](../resources/accesspackageanswerchoice.md). Essas respostas serão armazenadas em um [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|answeredQuestion|[accessPackageQuestion](../resources/accesspackagequestion.md)|A pergunta para a resposta. Obrigatório e somente leitura.|
|displayValue|Cadeia de caracteres|O valor de exibição da resposta. Obrigatório.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageAnswer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageAnswer",
  "displayValue": "String",
  "answeredQuestion": {
    "@odata.type": "microsoft.graph.accessPackageQuestion"
  }
}
```

