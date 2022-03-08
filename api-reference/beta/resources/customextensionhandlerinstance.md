---
title: Tipo de recurso customExtensionHandlerInstance
description: Usado para registrar o status de uma instância de extensão de fluxo de trabalho personalizada sendo executado em uma solicitação de atribuição de pacote de acesso.
author: currenmehta
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: d832ca092404eb3221952b0b46b720d8f0c217cc
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338044"
---
# <a name="customextensionhandlerinstance-resource-type"></a>Tipo de recurso customExtensionHandlerInstance

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Usado para registrar o status da instância  [de extensão de fluxo de trabalho](customaccesspackageworkflowextension.md) personalizada sendo executado em uma solicitação de atribuição [de pacote de acesso](accesspackageassignmentrequest.md).

## <a name="methods"></a>Métodos
Nenhum

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|customExtensionId|Cadeia de caracteres|Identificador do [customAccessPackageWorkflowExtension](customaccesspackageworkflowextension.md) disparado nesta instância.|
|externalCorrelationId|String|A ID de executar exclusiva para o aplicativo lógico.|
|stage|accessPackageCustomExtensionStage|Indica o estágio do fluxo de trabalho de solicitação quando a extensão personalizada do pacote de acesso é executado. Os valores possíveis são `assignmentRequestCreated`, `assignmentRequestApproved`, `assignmentRequestGranted`, `assignmentRequestRemoved`, `assignmentFourteenDaysBeforeExpiration`, `assignmentOneDayBeforeExpiration`, `unknownFutureValue`.|
|status|accessPackageCustomExtensionHandlerStatus|Status da solicitação para executar o fluxo de trabalho de extensão personalizado do pacote de acesso associado ao aplicativo lógico. Os valores possíveis são: `requestSent`, `requestReceived`, `unknownFutureValue`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.customExtensionHandlerInstance"
}
-->
``` json

{
  "@odata.type": "#microsoft.graph.customExtensionHandlerInstance",
  "stage": "String",
  "customExtensionId": "String",
  "externalCorrelationId": "String",
  "status": "String"
}
```

