---
title: função getRelatedAppStates
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1f2cf130b7e205767ddae5a5a7e857a12725d824
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34974304"
---
# <a name="getrelatedappstates-function"></a><span data-ttu-id="29a08-103">função getRelatedAppStates</span><span class="sxs-lookup"><span data-stu-id="29a08-103">getRelatedAppStates function</span></span>

> <span data-ttu-id="29a08-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="29a08-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="29a08-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="29a08-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="29a08-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="29a08-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="29a08-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="29a08-107">Prerequisites</span></span>
<span data-ttu-id="29a08-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29a08-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29a08-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="29a08-110">Permission type</span></span>|<span data-ttu-id="29a08-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="29a08-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="29a08-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="29a08-112">Delegated (work or school account)</span></span>|<span data-ttu-id="29a08-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="29a08-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="29a08-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="29a08-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="29a08-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="29a08-115">Not supported.</span></span>|
|<span data-ttu-id="29a08-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="29a08-116">Application</span></span>|<span data-ttu-id="29a08-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="29a08-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="29a08-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="29a08-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/getRelatedAppStates
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/getRelatedAppStates
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/getRelatedAppStates
```

## <a name="request-headers"></a><span data-ttu-id="29a08-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="29a08-119">Request headers</span></span>
|<span data-ttu-id="29a08-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="29a08-120">Header</span></span>|<span data-ttu-id="29a08-121">Valor</span><span class="sxs-lookup"><span data-stu-id="29a08-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="29a08-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="29a08-122">Authorization</span></span>|<span data-ttu-id="29a08-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="29a08-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="29a08-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="29a08-124">Accept</span></span>|<span data-ttu-id="29a08-125">application/json</span><span class="sxs-lookup"><span data-stu-id="29a08-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="29a08-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="29a08-126">Request body</span></span>
<span data-ttu-id="29a08-127">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="29a08-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="29a08-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="29a08-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="29a08-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="29a08-129">Property</span></span>|<span data-ttu-id="29a08-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="29a08-130">Type</span></span>|<span data-ttu-id="29a08-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="29a08-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29a08-132">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="29a08-132">userPrincipalName</span></span>|<span data-ttu-id="29a08-133">String</span><span class="sxs-lookup"><span data-stu-id="29a08-133">String</span></span>|<span data-ttu-id="29a08-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="29a08-134">Not yet documented</span></span>|
|<span data-ttu-id="29a08-135">deviceId</span><span class="sxs-lookup"><span data-stu-id="29a08-135">deviceId</span></span>|<span data-ttu-id="29a08-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="29a08-136">String</span></span>|<span data-ttu-id="29a08-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="29a08-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="29a08-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="29a08-138">Response</span></span>
<span data-ttu-id="29a08-139">Se tiver êxito, essa função retornará `200 OK` um código de resposta e uma coleção [mobileAppRelationshipState](../resources/intune-apps-mobileapprelationshipstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="29a08-139">If successful, this function returns a `200 OK` response code and a [mobileAppRelationshipState](../resources/intune-apps-mobileapprelationshipstate.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29a08-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="29a08-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="29a08-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="29a08-141">Request</span></span>
<span data-ttu-id="29a08-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="29a08-142">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/getRelatedAppStates(userPrincipalName='parameterValue',deviceId='parameterValue')
```

### <a name="response"></a><span data-ttu-id="29a08-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="29a08-143">Response</span></span>
<span data-ttu-id="29a08-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="29a08-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





