---
title: Obter mobileAppPolicySetItem
description: Leia as propriedades e as relações do objeto mobileAppPolicySetItem.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a6aed518ae86abd179d8751ace9acf457fce3685
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42802164"
---
# <a name="get-mobileapppolicysetitem"></a><span data-ttu-id="92b17-103">Obter mobileAppPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="92b17-103">Get mobileAppPolicySetItem</span></span>

> <span data-ttu-id="92b17-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="92b17-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92b17-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="92b17-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92b17-106">Leia as propriedades e as relações do objeto [mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md) .</span><span class="sxs-lookup"><span data-stu-id="92b17-106">Read properties and relationships of the [mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="92b17-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="92b17-107">Prerequisites</span></span>
<span data-ttu-id="92b17-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92b17-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92b17-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="92b17-110">Permission type</span></span>|<span data-ttu-id="92b17-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="92b17-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92b17-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="92b17-112">Delegated (work or school account)</span></span>|<span data-ttu-id="92b17-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="92b17-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="92b17-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="92b17-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92b17-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="92b17-115">Not supported.</span></span>|
|<span data-ttu-id="92b17-116">Application</span><span class="sxs-lookup"><span data-stu-id="92b17-116">Application</span></span>|<span data-ttu-id="92b17-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="92b17-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="92b17-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="92b17-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="92b17-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="92b17-119">Optional query parameters</span></span>
<span data-ttu-id="92b17-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="92b17-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="92b17-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="92b17-121">Request headers</span></span>
|<span data-ttu-id="92b17-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="92b17-122">Header</span></span>|<span data-ttu-id="92b17-123">Valor</span><span class="sxs-lookup"><span data-stu-id="92b17-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="92b17-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="92b17-124">Authorization</span></span>|<span data-ttu-id="92b17-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="92b17-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="92b17-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="92b17-126">Accept</span></span>|<span data-ttu-id="92b17-127">application/json</span><span class="sxs-lookup"><span data-stu-id="92b17-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="92b17-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="92b17-128">Request body</span></span>
<span data-ttu-id="92b17-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="92b17-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="92b17-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="92b17-130">Response</span></span>
<span data-ttu-id="92b17-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="92b17-131">If successful, this method returns a `200 OK` response code and [mobileAppPolicySetItem](../resources/intune-policyset-mobileapppolicysetitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92b17-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="92b17-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="92b17-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="92b17-133">Request</span></span>
<span data-ttu-id="92b17-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="92b17-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

### <a name="response"></a><span data-ttu-id="92b17-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="92b17-135">Response</span></span>
<span data-ttu-id="92b17-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="92b17-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 641

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileAppPolicySetItem",
    "id": "b6ffe6cf-e6cf-b6ff-cfe6-ffb6cfe6ffb6",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "payloadId": "Payload Id value",
    "itemType": "Item Type value",
    "displayName": "Display Name value",
    "status": "validating",
    "errorCode": "unauthorized",
    "guidedDeploymentTags": [
      "Guided Deployment Tags value"
    ],
    "intent": "required",
    "settings": {
      "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
    }
  }
}
```




