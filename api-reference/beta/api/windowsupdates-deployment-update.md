---
title: Atualizar implantação
description: Atualize as propriedades de um objeto de implantação.
author: Alice-at-Microsoft
ms.localizationpriority: medium
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: f86305a223147cfc081cd5dd71657e25260ce4e8
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61004363"
---
# <a name="update-deployment"></a>Atualizar implantação
Namespace: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize as propriedades de um [objeto de](../resources/windowsupdates-deployment.md) implantação.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|WindowsUpdates.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|WindowsUpdates.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /admin/windows/updates/deployments/{deploymentId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON do [objeto de](../resources/windowsupdates-deployment.md) implantação.

A tabela a seguir mostra as propriedades que podem ser definidas quando você atualiza a [implantação](../resources/windowsupdates-deployment.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|state|[microsoft.graph.windowsUpdates.deploymentState](../resources/windowsupdates-deploymentstate.md)|Status de execução da implantação.|
|settings|[microsoft.graph.windowsUpdates.deploymentSettings](../resources/windowsupdates-deploymentsettings.md)|Configurações especificado na implantação específica que rege como implantar a implantação `content` .|


## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código `202 Accepted` de resposta e um objeto de [implantação](../resources/windowsupdates-deployment.md) atualizado no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-pause-a-deployment"></a>Exemplo: pausar uma implantação

Neste exemplo, a implantação é pausada atualizando a `requestedValue` implantação `state` .

#### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_deployment_1",
  "@odata.type": "microsoft.graph.windowsUpdates.deployment"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/admin/windows/updates/deployments/b5171742-1742-b517-4217-17b5421717b5
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.windowsUpdates.deployment",
  "state": {
    "@odata.type": "microsoft.graph.windowsUpdates.deploymentState",
    "requestedValue": "paused"
  },
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-deployment-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-deployment-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-deployment-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-deployment-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-deployment-1-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.windowsUpdates.deployment"
}
-->
``` http
HTTP/1.1 202 Accepted
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.windowsUpdates.deployment",
  "id": "b5171742-1742-b517-4217-17b5421717b5",
  "state": {
    "@odata.type": "microsoft.graph.windowsUpdates.deploymentState",
    "reasons": [
      {
        "@odata.type": "microsoft.graph.windowsUpdates.deploymentStateReason",
        "value": "pausedByRequest"
      }
    ],
    "requestedValue": "paused",
    "value": "paused"
  },
  "content": {
    "@odata.type": "microsoft.graph.windowsUpdates.featureUpdateReference",
    "version": "20H2"
  },
  "settings": null,
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)"
}
```

### <a name="example-update-deployment-settings-to-add-a-monitoring-rule"></a>Exemplo: atualizar configurações de implantação para adicionar uma regra de monitoramento

Neste exemplo, a `settings` propriedade da implantação é atualizada para adicionar uma regra de monitoramento.

#### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_deployment_2",
  "@odata.type": "microsoft.graph.windowsUpdates.deployment"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/admin/windows/updates/deployments/b5171742-1742-b517-4217-17b5421717b5
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.windowsUpdates.deployment",
  "settings": {
    "@odata.type": "microsoft.graph.windowsUpdates.windowsDeploymentSettings",
    "monitoring": {
      "monitoringRules": [
        {
          "signal": "rollback",
          "threshold": 5,
          "action": "pauseDeployment"
        }
      ]
    }
  }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-deployment-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-deployment-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-deployment-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-deployment-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-deployment-2-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.windowsUpdates.deployment"
}
-->
``` http
HTTP/1.1 202 Accepted
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.windowsUpdates.deployment",
  "id": "b5171742-1742-b517-4217-17b5421717b5",
  "state": {
    "@odata.type": "microsoft.graph.windowsUpdates.deploymentState",
    "reasons": [
      {
        "@odata.type": "microsoft.graph.windowsUpdates.deploymentStateReason",
        "value": "offeringByRequest"
      }
    ],
    "requestedValue": "none",
    "value": "offering"
  },
  "content": {
    "@odata.type": "microsoft.graph.windowsUpdates.featureUpdateReference",
    "version": "20H2"
  },
  "settings": {
    "@odata.type": "microsoft.graph.windowsUpdates.windowsDeploymentSettings",
    "monitoring": {
      "monitoringRules": [
        {
          "signal": "rollback",
          "threshold": 5,
          "action": "pauseDeployment"
        }
      ]
    }
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)"
}
```

