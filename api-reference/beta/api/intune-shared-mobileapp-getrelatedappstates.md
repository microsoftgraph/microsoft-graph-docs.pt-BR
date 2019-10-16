---
title: função getRelatedAppStates
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2341db4c477a1cd255eff21348bb4708b458545f
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37537997"
---
# <a name="getrelatedappstates-function"></a><span data-ttu-id="86ff4-103">função getRelatedAppStates</span><span class="sxs-lookup"><span data-stu-id="86ff4-103">getRelatedAppStates function</span></span>

> <span data-ttu-id="86ff4-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="86ff4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="86ff4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="86ff4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86ff4-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="86ff4-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="86ff4-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="86ff4-107">Prerequisites</span></span>
<span data-ttu-id="86ff4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86ff4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86ff4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="86ff4-110">Permission type</span></span>|<span data-ttu-id="86ff4-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="86ff4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86ff4-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="86ff4-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="86ff4-113">&nbsp;&nbsp; **Aplicativos)**</span><span class="sxs-lookup"><span data-stu-id="86ff4-113">&nbsp; &nbsp; **Apps)**</span></span> | <span data-ttu-id="86ff4-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="86ff4-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="86ff4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="86ff4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86ff4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="86ff4-116">Not supported.</span></span>|
|<span data-ttu-id="86ff4-117">Application</span><span class="sxs-lookup"><span data-stu-id="86ff4-117">Application</span></span>||
| <span data-ttu-id="86ff4-118">&nbsp;&nbsp; **Aplicativos)**</span><span class="sxs-lookup"><span data-stu-id="86ff4-118">&nbsp; &nbsp; **Apps)**</span></span> | <span data-ttu-id="86ff4-119">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="86ff4-119">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="86ff4-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="86ff4-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/getRelatedAppStates
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/getRelatedAppStates
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/getRelatedAppStates
```

## <a name="request-headers"></a><span data-ttu-id="86ff4-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="86ff4-121">Request headers</span></span>
|<span data-ttu-id="86ff4-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="86ff4-122">Header</span></span>|<span data-ttu-id="86ff4-123">Valor</span><span class="sxs-lookup"><span data-stu-id="86ff4-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="86ff4-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="86ff4-124">Authorization</span></span>|<span data-ttu-id="86ff4-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="86ff4-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="86ff4-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="86ff4-126">Accept</span></span>|<span data-ttu-id="86ff4-127">application/json</span><span class="sxs-lookup"><span data-stu-id="86ff4-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="86ff4-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="86ff4-128">Request body</span></span>
<span data-ttu-id="86ff4-129">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="86ff4-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="86ff4-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="86ff4-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="86ff4-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="86ff4-131">Property</span></span>|<span data-ttu-id="86ff4-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="86ff4-132">Type</span></span>|<span data-ttu-id="86ff4-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="86ff4-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86ff4-134">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="86ff4-134">userPrincipalName</span></span>|<span data-ttu-id="86ff4-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="86ff4-135">String</span></span>|<span data-ttu-id="86ff4-136">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="86ff4-136">Not yet documented</span></span>|
|<span data-ttu-id="86ff4-137">deviceId</span><span class="sxs-lookup"><span data-stu-id="86ff4-137">deviceId</span></span>|<span data-ttu-id="86ff4-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="86ff4-138">String</span></span>|<span data-ttu-id="86ff4-139">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="86ff4-139">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="86ff4-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="86ff4-140">Response</span></span>
<span data-ttu-id="86ff4-141">Se tiver êxito, essa função retornará `200 OK` um código de resposta e uma coleção [mobileAppRelationshipState](../resources/intune-apps-mobileapprelationshipstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="86ff4-141">If successful, this function returns a `200 OK` response code and a [mobileAppRelationshipState](../resources/intune-apps-mobileapprelationshipstate.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86ff4-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="86ff4-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="86ff4-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="86ff4-143">Request</span></span>
<span data-ttu-id="86ff4-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="86ff4-144">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/getRelatedAppStates(userPrincipalName='parameterValue',deviceId='parameterValue')
```

### <a name="response"></a><span data-ttu-id="86ff4-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="86ff4-145">Response</span></span>
<span data-ttu-id="86ff4-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="86ff4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






