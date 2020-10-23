---
title: Listar managedDeviceMobileAppConfigurationUserStatuses
description: Listar propriedades e relações dos objetos managedDeviceMobileAppConfigurationUserStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6423c827e7286d8a3471ba5fd9637c24f0999ccf
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48699349"
---
# <a name="list-manageddevicemobileappconfigurationuserstatuses"></a><span data-ttu-id="a0bea-103">Listar managedDeviceMobileAppConfigurationUserStatuses</span><span class="sxs-lookup"><span data-stu-id="a0bea-103">List managedDeviceMobileAppConfigurationUserStatuses</span></span>

<span data-ttu-id="a0bea-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0bea-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a0bea-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a0bea-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a0bea-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a0bea-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a0bea-107">Listar propriedades e relações dos objetos [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="a0bea-107">List properties and relationships of the [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a0bea-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a0bea-108">Prerequisites</span></span>
<span data-ttu-id="a0bea-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0bea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0bea-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a0bea-111">Permission type</span></span>|<span data-ttu-id="a0bea-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a0bea-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a0bea-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a0bea-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a0bea-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a0bea-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a0bea-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a0bea-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a0bea-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a0bea-116">Not supported.</span></span>|
|<span data-ttu-id="a0bea-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a0bea-117">Application</span></span>|<span data-ttu-id="a0bea-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a0bea-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a0bea-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a0bea-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses
GET /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="a0bea-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a0bea-120">Request headers</span></span>
|<span data-ttu-id="a0bea-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a0bea-121">Header</span></span>|<span data-ttu-id="a0bea-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a0bea-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a0bea-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a0bea-123">Authorization</span></span>|<span data-ttu-id="a0bea-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a0bea-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a0bea-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a0bea-125">Accept</span></span>|<span data-ttu-id="a0bea-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a0bea-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0bea-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a0bea-127">Request body</span></span>
<span data-ttu-id="a0bea-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a0bea-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a0bea-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0bea-129">Response</span></span>
<span data-ttu-id="a0bea-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a0bea-130">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0bea-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a0bea-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="a0bea-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a0bea-132">Request</span></span>
<span data-ttu-id="a0bea-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a0bea-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses
```

### <a name="response"></a><span data-ttu-id="a0bea-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0bea-134">Response</span></span>
<span data-ttu-id="a0bea-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a0bea-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 416

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserStatus",
      "id": "44960944-0944-4496-4409-964444099644",
      "userDisplayName": "User Display Name value",
      "devicesCount": 12,
      "status": "notApplicable",
      "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```





