---
title: Tipo de recurso accessPackageAnswer
description: O tipo complexo para respostas a um accessPackageQuestion armazenado em um accessPackageAssignmentRequest.
author: markwahl-msft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 3da6d1b0e2e519895af4dacca009b027807b0184
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135485"
---
# <a name="accesspackageanswer-resource-type"></a>Tipo de recurso accessPackageAnswer

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O tipo complexo de uma resposta fornecida pelo solicitante para um [accessPackageQuestion](../resources/accesspackagequestion.md). A resposta real será um subtipo desse tipo complexo, [accessPackageAnswerString](../resources/accesspackageanswerstring.md) ou [accessPackageAnswerChoice](../resources/accesspackageanswerchoice.md). Essas respostas serão armazenadas em um [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|answeredQuestion|[accessPackageQuestion](../resources/accesspackagequestion.md)|A pergunta para a que a resposta se trata. Obrigatório e somente leitura.|
|displayValue|String|O valor de exibição da resposta. Obrigatório.|

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

