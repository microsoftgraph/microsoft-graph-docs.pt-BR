---
title: Acessar managedDeviceMobileAppConfigurationUserStatus
description: Leia as propriedades e as relações do objeto managedDeviceMobileAppConfigurationUserStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ac4e23b7bc8f6ff915e16c4bf370ee5fc84e198e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27920223"
---
# <a name="get-manageddevicemobileappconfigurationuserstatus"></a><span data-ttu-id="582df-103">Acessar managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="582df-103">Get managedDeviceMobileAppConfigurationUserStatus</span></span>

> <span data-ttu-id="582df-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="582df-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="582df-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="582df-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="582df-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="582df-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="582df-107">Leia as propriedades e as relações do objeto [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="582df-107">Read properties and relationships of the [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="582df-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="582df-108">Prerequisites</span></span>
<span data-ttu-id="582df-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="582df-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="582df-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="582df-111">Permission type</span></span>|<span data-ttu-id="582df-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="582df-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="582df-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="582df-113">Delegated (work or school account)</span></span>|<span data-ttu-id="582df-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="582df-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="582df-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="582df-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="582df-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="582df-116">Not supported.</span></span>|
|<span data-ttu-id="582df-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="582df-117">Application</span></span>|<span data-ttu-id="582df-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="582df-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="582df-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="582df-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses/{managedDeviceMobileAppConfigurationUserStatusId}
GET /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/userStatuses/{managedDeviceMobileAppConfigurationUserStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="582df-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="582df-120">Optional query parameters</span></span>
<span data-ttu-id="582df-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="582df-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="582df-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="582df-122">Request headers</span></span>
|<span data-ttu-id="582df-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="582df-123">Header</span></span>|<span data-ttu-id="582df-124">Valor</span><span class="sxs-lookup"><span data-stu-id="582df-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="582df-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="582df-125">Authorization</span></span>|<span data-ttu-id="582df-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="582df-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="582df-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="582df-127">Accept</span></span>|<span data-ttu-id="582df-128">application/json</span><span class="sxs-lookup"><span data-stu-id="582df-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="582df-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="582df-129">Request body</span></span>
<span data-ttu-id="582df-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="582df-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="582df-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="582df-131">Response</span></span>
<span data-ttu-id="582df-132">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="582df-132">If successful, this method returns a `200 OK` response code and [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="582df-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="582df-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="582df-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="582df-134">Request</span></span>
<span data-ttu-id="582df-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="582df-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses/{managedDeviceMobileAppConfigurationUserStatusId}
```

### <a name="response"></a><span data-ttu-id="582df-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="582df-136">Response</span></span>
<span data-ttu-id="582df-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="582df-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 388

{
  "value": {
    "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserStatus",
    "id": "44960944-0944-4496-4409-964444099644",
    "userDisplayName": "User Display Name value",
    "devicesCount": 12,
    "status": "notApplicable",
    "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
    "userPrincipalName": "User Principal Name value"
  }
}
```





