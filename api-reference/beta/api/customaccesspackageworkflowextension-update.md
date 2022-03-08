---
title: Atualizar customAccessPackageWorkflowExtension
description: Atualize as propriedades de um objeto customAccessPackageWorkflowExtension.
author: currenmehta
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: e0f0c0304ff1fa4ac102d73dcc8949567aa706c4
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338021"
---
# <a name="update-customaccesspackageworkflowextension"></a>Atualizar customAccessPackageWorkflowExtension
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize as propriedades de um [objeto customAccessPackageWorkflowExtension](../resources/customaccesspackageworkflowextension.md) existente.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|EntitlementManagement.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|EntitlementManagement.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
PUT /identityGovernance/entitlementManagement/accessPackageCatalogs/{catalogId}/customAccessPackageWorkflowExtensions/{customAccessPackageWorkflowExtensionId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]


|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|description|String|Descrição do objeto customAccessPackageWorkflowExtension.|
|displayName|String|Nome para exibição do customAccessPackageWorkflowExtension.|
|endpointConfiguration|[customExtensionEndpointConfiguration](../resources/customextensionendpointconfiguration.md)|O tipo e os detalhes para configurar o ponto de extremidade para chamar o fluxo de trabalho do aplicativo lógico.|  
|authenticationConfiguration|[customExtensionAuthenticationConfiguration](../resources/customextensionauthenticationconfiguration.md)|Configuração para proteger a chamada da API para o aplicativo lógico. Por exemplo, o fluxo de credenciais do cliente OAuth.|


## <a name="response"></a>Resposta

Se tiver êxito, este método retornará `200 OK` um código de resposta e um [objeto customAccessPackageWorkflowExtension](../resources/customaccesspackageworkflowextension.md) atualizado no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_customaccesspackageworkflowextension"
}
-->
``` http
PUT https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/32efb28c-9a7a-446c-986b-ca6528c6669d/customAccessPackageWorkflowExtensions/98ffaec5-ae8e-4902-a434-5ffc5d3d3cd0
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.customAccessPackageWorkflowExtension",
  "displayName": "test_action_0124_email",
  "description": "this is for graph testing only"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-customaccesspackageworkflowextension-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-customaccesspackageworkflowextension-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-customaccesspackageworkflowextension-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-customaccesspackageworkflowextension-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-customaccesspackageworkflowextension-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.customAccessPackageWorkflowExtension"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{ 
    "displayName": "test_action_0124_email", 
    "description": "this is for graph testing only", 
    "endpointConfiguration": { 
        "@odata.type": "#microsoft.graph.logicAppTriggerEndpointConfiguration", 
        "subscriptionId": "38ab2ccc-3747-4567-b36b-9478f5602f0d", 
        "resourceGroupName": "EMLogicApp", 
        "logicAppWorkflowName": "elm-extension-email" 
    }, 
    "authenticationConfiguration": { 
        "@odata.type": "#microsoft.graph.azureAdTokenAuthentication", 
        "resourceId": "eed6dee9-7ff7-44a5-8980-c11e8886cea2" 
    } 
} 
```

