---
title: Acessar deviceManagementPartner
description: Leia as propriedades e as relações do objeto deviceManagementPartner.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 71bb10e7d7e3fd514f7591b84c5999a411941c90
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50153806"
---
# <a name="get-devicemanagementpartner"></a><span data-ttu-id="b310c-103">Acessar deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="b310c-103">Get deviceManagementPartner</span></span>

<span data-ttu-id="b310c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b310c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b310c-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b310c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b310c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b310c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b310c-107">Leia as propriedades e as relações do objeto [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="b310c-107">Read properties and relationships of the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b310c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b310c-108">Prerequisites</span></span>
<span data-ttu-id="b310c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b310c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b310c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b310c-111">Permission type</span></span>|<span data-ttu-id="b310c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b310c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b310c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b310c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b310c-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b310c-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="b310c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b310c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b310c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b310c-116">Not supported.</span></span>|
|<span data-ttu-id="b310c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b310c-117">Application</span></span>|<span data-ttu-id="b310c-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b310c-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b310c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b310c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b310c-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b310c-120">Optional query parameters</span></span>
<span data-ttu-id="b310c-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b310c-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b310c-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b310c-122">Request headers</span></span>
|<span data-ttu-id="b310c-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b310c-123">Header</span></span>|<span data-ttu-id="b310c-124">Valor</span><span class="sxs-lookup"><span data-stu-id="b310c-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b310c-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="b310c-125">Authorization</span></span>|<span data-ttu-id="b310c-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b310c-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b310c-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b310c-127">Accept</span></span>|<span data-ttu-id="b310c-128">application/json</span><span class="sxs-lookup"><span data-stu-id="b310c-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b310c-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b310c-129">Request body</span></span>
<span data-ttu-id="b310c-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b310c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b310c-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="b310c-131">Response</span></span>
<span data-ttu-id="b310c-132">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b310c-132">If successful, this method returns a `200 OK` response code and [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b310c-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b310c-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="b310c-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b310c-134">Request</span></span>
<span data-ttu-id="b310c-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b310c-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

### <a name="response"></a><span data-ttu-id="b310c-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="b310c-136">Response</span></span>
<span data-ttu-id="b310c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b310c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1254

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementPartner",
    "id": "d21e377a-377a-d21e-7a37-1ed27a371ed2",
    "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
    "partnerState": "unavailable",
    "partnerAppType": "singleTenantApp",
    "singleTenantAppId": "Single Tenant App Id value",
    "displayName": "Display Name value",
    "isConfigured": true,
    "whenPartnerDevicesWillBeRemoved": "2017-01-01T00:00:34.890321-08:00",
    "whenPartnerDevicesWillBeMarkedAsNonCompliant": "2017-01-01T00:02:38.9066046-08:00",
    "whenPartnerDevicesWillBeRemovedDateTime": "2016-12-31T23:56:38.2655023-08:00",
    "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2016-12-31T23:58:42.2131231-08:00",
    "groupsRequiringPartnerEnrollment": [
      {
        "@odata.type": "microsoft.graph.deviceManagementPartnerAssignment",
        "target": {
          "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
          "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
          "deviceAndAppManagementAssignmentFilterType": "include",
          "collectionId": "Collection Id value"
        }
      }
    ]
  }
}
```




