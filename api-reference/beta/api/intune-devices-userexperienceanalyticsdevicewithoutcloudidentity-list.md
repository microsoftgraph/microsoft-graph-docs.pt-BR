---
title: Listar userExperienceAnalyticsDeviceWithoutCloudIdentities
description: Listar propriedades e relações dos objetos userExperienceAnalyticsDeviceWithoutCloudIdentity.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7904937e64ad41b1855c0d3fc58b8885266be37e
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160089"
---
# <a name="list-userexperienceanalyticsdevicewithoutcloudidentities"></a><span data-ttu-id="74a6f-103">Listar userExperienceAnalyticsDeviceWithoutCloudIdentities</span><span class="sxs-lookup"><span data-stu-id="74a6f-103">List userExperienceAnalyticsDeviceWithoutCloudIdentities</span></span>

<span data-ttu-id="74a6f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74a6f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="74a6f-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="74a6f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="74a6f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="74a6f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="74a6f-107">Listar propriedades e relações dos [objetos userExperienceAnalyticsDeviceWithoutCloudIdentity.](../resources/intune-devices-userexperienceanalyticsdevicewithoutcloudidentity.md)</span><span class="sxs-lookup"><span data-stu-id="74a6f-107">List properties and relationships of the [userExperienceAnalyticsDeviceWithoutCloudIdentity](../resources/intune-devices-userexperienceanalyticsdevicewithoutcloudidentity.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="74a6f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="74a6f-108">Prerequisites</span></span>
<span data-ttu-id="74a6f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74a6f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74a6f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="74a6f-111">Permission type</span></span>|<span data-ttu-id="74a6f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="74a6f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="74a6f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="74a6f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="74a6f-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="74a6f-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="74a6f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="74a6f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="74a6f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="74a6f-116">Not supported.</span></span>|
|<span data-ttu-id="74a6f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="74a6f-117">Application</span></span>|<span data-ttu-id="74a6f-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="74a6f-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="74a6f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="74a6f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsDevicesWithoutCloudIdentity
```

## <a name="request-headers"></a><span data-ttu-id="74a6f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="74a6f-120">Request headers</span></span>
|<span data-ttu-id="74a6f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="74a6f-121">Header</span></span>|<span data-ttu-id="74a6f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="74a6f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="74a6f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="74a6f-123">Authorization</span></span>|<span data-ttu-id="74a6f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="74a6f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="74a6f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="74a6f-125">Accept</span></span>|<span data-ttu-id="74a6f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="74a6f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="74a6f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="74a6f-127">Request body</span></span>
<span data-ttu-id="74a6f-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="74a6f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="74a6f-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="74a6f-129">Response</span></span>
<span data-ttu-id="74a6f-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [userExperienceAnalyticsDeviceWithoutCloudIdentity](../resources/intune-devices-userexperienceanalyticsdevicewithoutcloudidentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="74a6f-130">If successful, this method returns a `200 OK` response code and a collection of [userExperienceAnalyticsDeviceWithoutCloudIdentity](../resources/intune-devices-userexperienceanalyticsdevicewithoutcloudidentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74a6f-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="74a6f-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="74a6f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="74a6f-132">Request</span></span>
<span data-ttu-id="74a6f-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="74a6f-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDevicesWithoutCloudIdentity
```

### <a name="response"></a><span data-ttu-id="74a6f-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="74a6f-134">Response</span></span>
<span data-ttu-id="74a6f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="74a6f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 277

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceWithoutCloudIdentity",
      "id": "80537287-7287-8053-8772-538087725380",
      "deviceName": "Device Name value",
      "azureAdDeviceId": "Azure Ad Device Id value"
    }
  ]
}
```




