---
title: função getRelatedAppStates
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 575a1d7c33801f474a23451cac900d612dc5bf65
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32490336"
---
# <a name="getrelatedappstates-function"></a><span data-ttu-id="de53e-103">função getRelatedAppStates</span><span class="sxs-lookup"><span data-stu-id="de53e-103">getRelatedAppStates function</span></span>

> <span data-ttu-id="de53e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="de53e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="de53e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="de53e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="de53e-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="de53e-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="de53e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="de53e-107">Prerequisites</span></span>
<span data-ttu-id="de53e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de53e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de53e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="de53e-110">Permission type</span></span>|<span data-ttu-id="de53e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="de53e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="de53e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="de53e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="de53e-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="de53e-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="de53e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="de53e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="de53e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="de53e-115">Not supported.</span></span>|
|<span data-ttu-id="de53e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="de53e-116">Application</span></span>|<span data-ttu-id="de53e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="de53e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="de53e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="de53e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/getRelatedAppStates
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/getRelatedAppStates
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/getRelatedAppStates
```

## <a name="request-headers"></a><span data-ttu-id="de53e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="de53e-119">Request headers</span></span>
|<span data-ttu-id="de53e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="de53e-120">Header</span></span>|<span data-ttu-id="de53e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="de53e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="de53e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="de53e-122">Authorization</span></span>|<span data-ttu-id="de53e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="de53e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="de53e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="de53e-124">Accept</span></span>|<span data-ttu-id="de53e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="de53e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="de53e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="de53e-126">Request body</span></span>
<span data-ttu-id="de53e-127">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="de53e-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="de53e-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="de53e-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="de53e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="de53e-129">Property</span></span>|<span data-ttu-id="de53e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="de53e-130">Type</span></span>|<span data-ttu-id="de53e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="de53e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de53e-132">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="de53e-132">userPrincipalName</span></span>|<span data-ttu-id="de53e-133">String</span><span class="sxs-lookup"><span data-stu-id="de53e-133">String</span></span>|<span data-ttu-id="de53e-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="de53e-134">Not yet documented</span></span>|
|<span data-ttu-id="de53e-135">deviceId</span><span class="sxs-lookup"><span data-stu-id="de53e-135">deviceId</span></span>|<span data-ttu-id="de53e-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="de53e-136">String</span></span>|<span data-ttu-id="de53e-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="de53e-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="de53e-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="de53e-138">Response</span></span>
<span data-ttu-id="de53e-139">Se tiver êxito, essa função retornará `200 OK` um código de resposta e uma coleção [mobileAppRelationshipState](../resources/intune-apps-mobileapprelationshipstate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="de53e-139">If successful, this function returns a `200 OK` response code and a [mobileAppRelationshipState](../resources/intune-apps-mobileapprelationshipstate.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de53e-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="de53e-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="de53e-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="de53e-141">Request</span></span>
<span data-ttu-id="de53e-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="de53e-142">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/getRelatedAppStates(userPrincipalName='parameterValue',deviceId='parameterValue')
```

### <a name="response"></a><span data-ttu-id="de53e-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="de53e-143">Response</span></span>
<span data-ttu-id="de53e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="de53e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





