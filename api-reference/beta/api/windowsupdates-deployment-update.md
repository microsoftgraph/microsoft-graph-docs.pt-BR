---
title: Atualizar implantação
description: Atualize as propriedades de um objeto de implantação.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 2b5857f70136b804494825eb7cb66945d2b1a452
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52785253"
---
# <a name="update-deployment"></a><span data-ttu-id="d2a1d-103">Atualizar implantação</span><span class="sxs-lookup"><span data-stu-id="d2a1d-103">Update deployment</span></span>
<span data-ttu-id="d2a1d-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="d2a1d-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2a1d-105">Atualize as propriedades de um [objeto de](../resources/windowsupdates-deployment.md) implantação.</span><span class="sxs-lookup"><span data-stu-id="d2a1d-105">Update the properties of a [deployment](../resources/windowsupdates-deployment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d2a1d-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="d2a1d-106">Permissions</span></span>
<span data-ttu-id="d2a1d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2a1d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2a1d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d2a1d-109">Permission type</span></span>|<span data-ttu-id="d2a1d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d2a1d-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d2a1d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d2a1d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d2a1d-112">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2a1d-112">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="d2a1d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d2a1d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d2a1d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d2a1d-114">Not supported.</span></span>|
|<span data-ttu-id="d2a1d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d2a1d-115">Application</span></span>|<span data-ttu-id="d2a1d-116">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2a1d-116">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d2a1d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d2a1d-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /admin/windows/updates/deployments/{deploymentId}
```

## <a name="request-headers"></a><span data-ttu-id="d2a1d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d2a1d-118">Request headers</span></span>
|<span data-ttu-id="d2a1d-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d2a1d-119">Name</span></span>|<span data-ttu-id="d2a1d-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2a1d-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d2a1d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d2a1d-121">Authorization</span></span>|<span data-ttu-id="d2a1d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d2a1d-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d2a1d-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d2a1d-124">Content-Type</span></span>|<span data-ttu-id="d2a1d-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d2a1d-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2a1d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d2a1d-127">Request body</span></span>
<span data-ttu-id="d2a1d-128">No corpo da solicitação, fornece uma representação JSON do [objeto de](../resources/windowsupdates-deployment.md) implantação.</span><span class="sxs-lookup"><span data-stu-id="d2a1d-128">In the request body, supply a JSON representation of the [deployment](../resources/windowsupdates-deployment.md) object.</span></span>

<span data-ttu-id="d2a1d-129">A tabela a seguir mostra as propriedades que podem ser definidas quando você atualiza a [implantação](../resources/windowsupdates-deployment.md).</span><span class="sxs-lookup"><span data-stu-id="d2a1d-129">The following table shows the properties that can be set when you update the [deployment](../resources/windowsupdates-deployment.md).</span></span>

|<span data-ttu-id="d2a1d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d2a1d-130">Property</span></span>|<span data-ttu-id="d2a1d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d2a1d-131">Type</span></span>|<span data-ttu-id="d2a1d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2a1d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2a1d-133">state</span><span class="sxs-lookup"><span data-stu-id="d2a1d-133">state</span></span>|[<span data-ttu-id="d2a1d-134">microsoft.graph.windowsUpdates.deploymentState</span><span class="sxs-lookup"><span data-stu-id="d2a1d-134">microsoft.graph.windowsUpdates.deploymentState</span></span>](../resources/windowsupdates-deploymentstate.md)|<span data-ttu-id="d2a1d-135">Status de execução da implantação.</span><span class="sxs-lookup"><span data-stu-id="d2a1d-135">Execution status of the deployment.</span></span>|
|<span data-ttu-id="d2a1d-136">settings</span><span class="sxs-lookup"><span data-stu-id="d2a1d-136">settings</span></span>|[<span data-ttu-id="d2a1d-137">microsoft.graph.windowsUpdates.deploymentSettings</span><span class="sxs-lookup"><span data-stu-id="d2a1d-137">microsoft.graph.windowsUpdates.deploymentSettings</span></span>](../resources/windowsupdates-deploymentsettings.md)|<span data-ttu-id="d2a1d-138">Configurações especificado na implantação específica que rege como implantar a implantação `content` .</span><span class="sxs-lookup"><span data-stu-id="d2a1d-138">Settings specified on the specific deployment governing how to deploy deployment `content`.</span></span>|


## <a name="response"></a><span data-ttu-id="d2a1d-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2a1d-139">Response</span></span>

<span data-ttu-id="d2a1d-140">Se tiver êxito, este método retornará um código `202 Accepted` de resposta e um objeto de [implantação](../resources/windowsupdates-deployment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d2a1d-140">If successful, this method returns a `202 Accepted` response code and an updated [deployment](../resources/windowsupdates-deployment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d2a1d-141">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d2a1d-141">Examples</span></span>

### <a name="example-pause-a-deployment"></a><span data-ttu-id="d2a1d-142">Exemplo: pausar uma implantação</span><span class="sxs-lookup"><span data-stu-id="d2a1d-142">Example: Pause a deployment</span></span>

<span data-ttu-id="d2a1d-143">Neste exemplo, a implantação é pausada atualizando a `requestedValue` implantação `state` .</span><span class="sxs-lookup"><span data-stu-id="d2a1d-143">In this example, the deployment is paused by updating the `requestedValue` of the deployment `state`.</span></span>

#### <a name="request"></a><span data-ttu-id="d2a1d-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d2a1d-144">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="d2a1d-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="d2a1d-145">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="d2a1d-146">C#</span><span class="sxs-lookup"><span data-stu-id="d2a1d-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-deployment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d2a1d-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d2a1d-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-deployment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d2a1d-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d2a1d-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-deployment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d2a1d-149">Java</span><span class="sxs-lookup"><span data-stu-id="d2a1d-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-deployment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="d2a1d-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2a1d-150">Response</span></span>

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

### <a name="example-update-deployment-settings-to-add-a-monitoring-rule"></a><span data-ttu-id="d2a1d-151">Exemplo: atualizar configurações de implantação para adicionar uma regra de monitoramento</span><span class="sxs-lookup"><span data-stu-id="d2a1d-151">Example: Update deployment settings to add a monitoring rule</span></span>

<span data-ttu-id="d2a1d-152">Neste exemplo, a `settings` propriedade da implantação é atualizada para adicionar uma regra de monitoramento.</span><span class="sxs-lookup"><span data-stu-id="d2a1d-152">In this example, the `settings` property of the deployment is updated to add a monitoring rule.</span></span>

#### <a name="request"></a><span data-ttu-id="d2a1d-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d2a1d-153">Request</span></span>
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


#### <a name="response"></a><span data-ttu-id="d2a1d-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2a1d-154">Response</span></span>

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

