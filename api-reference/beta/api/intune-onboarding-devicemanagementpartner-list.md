---
title: Listar deviceManagementPartners
description: Listar propriedades e relações de objetos de deviceManagementPartner.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: febe8f3f8f8a2ecffcf94982090e812355899ad7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42462051"
---
# <a name="list-devicemanagementpartners"></a><span data-ttu-id="164f4-103">Listar deviceManagementPartners</span><span class="sxs-lookup"><span data-stu-id="164f4-103">List deviceManagementPartners</span></span>

<span data-ttu-id="164f4-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="164f4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="164f4-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="164f4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="164f4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="164f4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="164f4-107">Listar propriedades e relações de objetos de [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="164f4-107">List properties and relationships of the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="164f4-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="164f4-108">Prerequisites</span></span>
<span data-ttu-id="164f4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="164f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="164f4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="164f4-111">Permission type</span></span>|<span data-ttu-id="164f4-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="164f4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="164f4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="164f4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="164f4-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="164f4-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="164f4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="164f4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="164f4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="164f4-116">Not supported.</span></span>|
|<span data-ttu-id="164f4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="164f4-117">Application</span></span>|<span data-ttu-id="164f4-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="164f4-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="164f4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="164f4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="164f4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="164f4-120">Request headers</span></span>
|<span data-ttu-id="164f4-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="164f4-121">Header</span></span>|<span data-ttu-id="164f4-122">Valor</span><span class="sxs-lookup"><span data-stu-id="164f4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="164f4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="164f4-123">Authorization</span></span>|<span data-ttu-id="164f4-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="164f4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="164f4-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="164f4-125">Accept</span></span>|<span data-ttu-id="164f4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="164f4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="164f4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="164f4-127">Request body</span></span>
<span data-ttu-id="164f4-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="164f4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="164f4-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="164f4-129">Response</span></span>
<span data-ttu-id="164f4-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="164f4-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="164f4-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="164f4-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="164f4-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="164f4-132">Request</span></span>
<span data-ttu-id="164f4-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="164f4-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementPartners
```

### <a name="response"></a><span data-ttu-id="164f4-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="164f4-134">Response</span></span>
<span data-ttu-id="164f4-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="164f4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1059

{
  "value": [
    {
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
            "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
          }
        }
      ]
    }
  ]
}
```





