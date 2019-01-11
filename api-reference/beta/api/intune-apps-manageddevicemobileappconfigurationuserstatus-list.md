---
title: Listar managedDeviceMobileAppConfigurationUserStatuses
description: Listar propriedades e relações dos objetos managedDeviceMobileAppConfigurationUserStatus.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5ed4c1efcbee91401b767b0450afe7167b8677ba
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837664"
---
# <a name="list-manageddevicemobileappconfigurationuserstatuses"></a><span data-ttu-id="8bd2a-103">Listar managedDeviceMobileAppConfigurationUserStatuses</span><span class="sxs-lookup"><span data-stu-id="8bd2a-103">List managedDeviceMobileAppConfigurationUserStatuses</span></span>

> <span data-ttu-id="8bd2a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8bd2a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8bd2a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8bd2a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8bd2a-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8bd2a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8bd2a-107">Listar propriedades e relações dos objetos [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="8bd2a-107">List properties and relationships of the [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8bd2a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8bd2a-108">Prerequisites</span></span>
<span data-ttu-id="8bd2a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8bd2a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8bd2a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8bd2a-111">Permission type</span></span>|<span data-ttu-id="8bd2a-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8bd2a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8bd2a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8bd2a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8bd2a-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="8bd2a-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="8bd2a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8bd2a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8bd2a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8bd2a-116">Not supported.</span></span>|
|<span data-ttu-id="8bd2a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8bd2a-117">Application</span></span>|<span data-ttu-id="8bd2a-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8bd2a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8bd2a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8bd2a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses
GET /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="8bd2a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8bd2a-120">Request headers</span></span>
|<span data-ttu-id="8bd2a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8bd2a-121">Header</span></span>|<span data-ttu-id="8bd2a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8bd2a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8bd2a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8bd2a-123">Authorization</span></span>|<span data-ttu-id="8bd2a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8bd2a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8bd2a-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8bd2a-125">Accept</span></span>|<span data-ttu-id="8bd2a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8bd2a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8bd2a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8bd2a-127">Request body</span></span>
<span data-ttu-id="8bd2a-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8bd2a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8bd2a-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="8bd2a-129">Response</span></span>
<span data-ttu-id="8bd2a-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8bd2a-130">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8bd2a-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8bd2a-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="8bd2a-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8bd2a-132">Request</span></span>
<span data-ttu-id="8bd2a-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8bd2a-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses
```

### <a name="response"></a><span data-ttu-id="8bd2a-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="8bd2a-134">Response</span></span>
<span data-ttu-id="8bd2a-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8bd2a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





