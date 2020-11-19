---
title: função getRelatedAppStates
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d59a56df349f1deb5f8c8ba110cf4e5db69a7bb9
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49285146"
---
# <a name="getrelatedappstates-function"></a><span data-ttu-id="c51e4-103">função getRelatedAppStates</span><span class="sxs-lookup"><span data-stu-id="c51e4-103">getRelatedAppStates function</span></span>

<span data-ttu-id="c51e4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c51e4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c51e4-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c51e4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c51e4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c51e4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c51e4-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c51e4-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c51e4-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c51e4-108">Prerequisites</span></span>
<span data-ttu-id="c51e4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c51e4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c51e4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c51e4-111">Permission type</span></span>|<span data-ttu-id="c51e4-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c51e4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c51e4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c51e4-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="c51e4-114">&nbsp;&nbsp; **Aplicativos)**</span><span class="sxs-lookup"><span data-stu-id="c51e4-114">&nbsp; &nbsp; **Apps)**</span></span> | <span data-ttu-id="c51e4-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c51e4-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c51e4-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c51e4-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c51e4-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c51e4-117">Not supported.</span></span>|
|<span data-ttu-id="c51e4-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c51e4-118">Application</span></span>||
| <span data-ttu-id="c51e4-119">&nbsp;&nbsp; **Aplicativos)**</span><span class="sxs-lookup"><span data-stu-id="c51e4-119">&nbsp; &nbsp; **Apps)**</span></span> | <span data-ttu-id="c51e4-120">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c51e4-120">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c51e4-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c51e4-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/getRelatedAppStates
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/getRelatedAppStates
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/getRelatedAppStates
```

## <a name="request-headers"></a><span data-ttu-id="c51e4-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c51e4-122">Request headers</span></span>
|<span data-ttu-id="c51e4-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c51e4-123">Header</span></span>|<span data-ttu-id="c51e4-124">Valor</span><span class="sxs-lookup"><span data-stu-id="c51e4-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c51e4-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="c51e4-125">Authorization</span></span>|<span data-ttu-id="c51e4-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c51e4-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c51e4-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c51e4-127">Accept</span></span>|<span data-ttu-id="c51e4-128">application/json</span><span class="sxs-lookup"><span data-stu-id="c51e4-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c51e4-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c51e4-129">Request body</span></span>
<span data-ttu-id="c51e4-130">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="c51e4-130">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="c51e4-131">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="c51e4-131">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="c51e4-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c51e4-132">Property</span></span>|<span data-ttu-id="c51e4-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="c51e4-133">Type</span></span>|<span data-ttu-id="c51e4-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="c51e4-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c51e4-135">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c51e4-135">userPrincipalName</span></span>|<span data-ttu-id="c51e4-136">String</span><span class="sxs-lookup"><span data-stu-id="c51e4-136">String</span></span>|<span data-ttu-id="c51e4-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c51e4-137">Not yet documented</span></span>|
|<span data-ttu-id="c51e4-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="c51e4-138">deviceId</span></span>|<span data-ttu-id="c51e4-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c51e4-139">String</span></span>|<span data-ttu-id="c51e4-140">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c51e4-140">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="c51e4-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="c51e4-141">Response</span></span>
<span data-ttu-id="c51e4-142">Se tiver êxito, essa função retornará um `200 OK` código de resposta e uma coleção [mobileAppRelationshipState](../resources/intune-apps-mobileapprelationshipstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c51e4-142">If successful, this function returns a `200 OK` response code and a [mobileAppRelationshipState](../resources/intune-apps-mobileapprelationshipstate.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c51e4-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c51e4-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="c51e4-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c51e4-144">Request</span></span>
<span data-ttu-id="c51e4-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c51e4-145">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/getRelatedAppStates(userPrincipalName='parameterValue',deviceId='parameterValue')
```

### <a name="response"></a><span data-ttu-id="c51e4-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="c51e4-146">Response</span></span>
<span data-ttu-id="c51e4-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c51e4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







