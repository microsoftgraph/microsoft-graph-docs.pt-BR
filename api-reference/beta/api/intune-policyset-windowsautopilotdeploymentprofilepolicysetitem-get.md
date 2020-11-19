---
title: Obter windowsAutopilotDeploymentProfilePolicySetItem
description: Leia as propriedades e as relações do objeto windowsAutopilotDeploymentProfilePolicySetItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 53c35bc57d7dc3d2b2c7452be739711c21d343de
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49217729"
---
# <a name="get-windowsautopilotdeploymentprofilepolicysetitem"></a><span data-ttu-id="22f08-103">Obter windowsAutopilotDeploymentProfilePolicySetItem</span><span class="sxs-lookup"><span data-stu-id="22f08-103">Get windowsAutopilotDeploymentProfilePolicySetItem</span></span>

<span data-ttu-id="22f08-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22f08-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="22f08-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="22f08-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="22f08-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="22f08-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22f08-107">Leia as propriedades e as relações do objeto [windowsAutopilotDeploymentProfilePolicySetItem](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="22f08-107">Read properties and relationships of the [windowsAutopilotDeploymentProfilePolicySetItem](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="22f08-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="22f08-108">Prerequisites</span></span>
<span data-ttu-id="22f08-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22f08-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22f08-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="22f08-111">Permission type</span></span>|<span data-ttu-id="22f08-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="22f08-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22f08-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="22f08-113">Delegated (work or school account)</span></span>|<span data-ttu-id="22f08-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="22f08-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="22f08-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="22f08-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22f08-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="22f08-116">Not supported.</span></span>|
|<span data-ttu-id="22f08-117">Application</span><span class="sxs-lookup"><span data-stu-id="22f08-117">Application</span></span>|<span data-ttu-id="22f08-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="22f08-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="22f08-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="22f08-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="22f08-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="22f08-120">Optional query parameters</span></span>
<span data-ttu-id="22f08-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="22f08-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="22f08-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="22f08-122">Request headers</span></span>
|<span data-ttu-id="22f08-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="22f08-123">Header</span></span>|<span data-ttu-id="22f08-124">Valor</span><span class="sxs-lookup"><span data-stu-id="22f08-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22f08-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="22f08-125">Authorization</span></span>|<span data-ttu-id="22f08-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="22f08-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22f08-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="22f08-127">Accept</span></span>|<span data-ttu-id="22f08-128">application/json</span><span class="sxs-lookup"><span data-stu-id="22f08-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22f08-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="22f08-129">Request body</span></span>
<span data-ttu-id="22f08-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="22f08-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="22f08-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="22f08-131">Response</span></span>
<span data-ttu-id="22f08-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [windowsAutopilotDeploymentProfilePolicySetItem](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="22f08-132">If successful, this method returns a `200 OK` response code and [windowsAutopilotDeploymentProfilePolicySetItem](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22f08-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="22f08-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="22f08-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="22f08-134">Request</span></span>
<span data-ttu-id="22f08-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="22f08-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

### <a name="response"></a><span data-ttu-id="22f08-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="22f08-136">Response</span></span>
<span data-ttu-id="22f08-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="22f08-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 543

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfilePolicySetItem",
    "id": "850e84d8-84d8-850e-d884-0e85d8840e85",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "payloadId": "Payload Id value",
    "itemType": "Item Type value",
    "displayName": "Display Name value",
    "status": "validating",
    "errorCode": "unauthorized",
    "guidedDeploymentTags": [
      "Guided Deployment Tags value"
    ]
  }
}
```




