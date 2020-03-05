---
title: função getRelatedAppStates
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 15b3e278e669c17c6f66ae37976cd8c74ee702d4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42458291"
---
# <a name="getrelatedappstates-function"></a><span data-ttu-id="4d921-103">função getRelatedAppStates</span><span class="sxs-lookup"><span data-stu-id="4d921-103">getRelatedAppStates function</span></span>

<span data-ttu-id="4d921-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4d921-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4d921-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4d921-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4d921-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4d921-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4d921-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="4d921-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4d921-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4d921-108">Prerequisites</span></span>
<span data-ttu-id="4d921-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d921-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d921-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4d921-111">Permission type</span></span>|<span data-ttu-id="4d921-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4d921-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4d921-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4d921-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="4d921-114">&nbsp;&nbsp; **Aplicativos)**</span><span class="sxs-lookup"><span data-stu-id="4d921-114">&nbsp; &nbsp; **Apps)**</span></span> | <span data-ttu-id="4d921-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4d921-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="4d921-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4d921-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4d921-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4d921-117">Not supported.</span></span>|
|<span data-ttu-id="4d921-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4d921-118">Application</span></span>||
| <span data-ttu-id="4d921-119">&nbsp;&nbsp; **Aplicativos)**</span><span class="sxs-lookup"><span data-stu-id="4d921-119">&nbsp; &nbsp; **Apps)**</span></span> | <span data-ttu-id="4d921-120">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4d921-120">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4d921-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4d921-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/getRelatedAppStates
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/getRelatedAppStates
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/getRelatedAppStates
```

## <a name="request-headers"></a><span data-ttu-id="4d921-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4d921-122">Request headers</span></span>
|<span data-ttu-id="4d921-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4d921-123">Header</span></span>|<span data-ttu-id="4d921-124">Valor</span><span class="sxs-lookup"><span data-stu-id="4d921-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4d921-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="4d921-125">Authorization</span></span>|<span data-ttu-id="4d921-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4d921-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4d921-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4d921-127">Accept</span></span>|<span data-ttu-id="4d921-128">application/json</span><span class="sxs-lookup"><span data-stu-id="4d921-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d921-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4d921-129">Request body</span></span>
<span data-ttu-id="4d921-130">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="4d921-130">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="4d921-131">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="4d921-131">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="4d921-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4d921-132">Property</span></span>|<span data-ttu-id="4d921-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="4d921-133">Type</span></span>|<span data-ttu-id="4d921-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="4d921-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d921-135">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4d921-135">userPrincipalName</span></span>|<span data-ttu-id="4d921-136">String</span><span class="sxs-lookup"><span data-stu-id="4d921-136">String</span></span>|<span data-ttu-id="4d921-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="4d921-137">Not yet documented</span></span>|
|<span data-ttu-id="4d921-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="4d921-138">deviceId</span></span>|<span data-ttu-id="4d921-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4d921-139">String</span></span>|<span data-ttu-id="4d921-140">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="4d921-140">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="4d921-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d921-141">Response</span></span>
<span data-ttu-id="4d921-142">Se tiver êxito, essa função retornará `200 OK` um código de resposta e uma coleção [mobileAppRelationshipState](../resources/intune-apps-mobileapprelationshipstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4d921-142">If successful, this function returns a `200 OK` response code and a [mobileAppRelationshipState](../resources/intune-apps-mobileapprelationshipstate.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d921-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4d921-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="4d921-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4d921-144">Request</span></span>
<span data-ttu-id="4d921-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4d921-145">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/getRelatedAppStates(userPrincipalName='parameterValue',deviceId='parameterValue')
```

### <a name="response"></a><span data-ttu-id="4d921-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d921-146">Response</span></span>
<span data-ttu-id="4d921-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4d921-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 481

{
  "value": [
    {
      "@odata.type": "microsoft.graph.mobileAppRelationshipState",
      "sourceIds": [
        "Source Ids value"
      ],
      "targetId": "Target Id value",
      "targetDisplayName": "Target Display Name value",
      "deviceId": "Device Id value",
      "installState": "failed",
      "installStateDetail": "dependencyFailedToInstall",
      "errorCode": 9,
      "targetLastSyncDateTime": "2017-01-01T00:02:09.7809949-08:00"
    }
  ]
}
```








