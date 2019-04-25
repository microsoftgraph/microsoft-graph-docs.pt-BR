---
title: Acessar managedDeviceMobileAppConfigurationUserStatus
description: Leia as propriedades e as relações do objeto managedDeviceMobileAppConfigurationUserStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d0b7a848aefebfbc35c6dd22e8243fc35309be6b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32578173"
---
# <a name="get-manageddevicemobileappconfigurationuserstatus"></a><span data-ttu-id="8e769-103">Acessar managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="8e769-103">Get managedDeviceMobileAppConfigurationUserStatus</span></span>

> <span data-ttu-id="8e769-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8e769-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e769-105">Leia as propriedades e as relações do objeto [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="8e769-105">Read properties and relationships of the [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8e769-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8e769-106">Prerequisites</span></span>
<span data-ttu-id="8e769-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e769-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e769-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8e769-109">Permission type</span></span>|<span data-ttu-id="8e769-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8e769-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8e769-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8e769-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8e769-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="8e769-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="8e769-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8e769-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e769-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8e769-114">Not supported.</span></span>|
|<span data-ttu-id="8e769-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8e769-115">Application</span></span>|<span data-ttu-id="8e769-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8e769-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e769-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8e769-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses/{managedDeviceMobileAppConfigurationUserStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8e769-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8e769-118">Optional query parameters</span></span>
<span data-ttu-id="8e769-119">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8e769-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8e769-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8e769-120">Request headers</span></span>
|<span data-ttu-id="8e769-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8e769-121">Header</span></span>|<span data-ttu-id="8e769-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8e769-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8e769-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8e769-123">Authorization</span></span>|<span data-ttu-id="8e769-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8e769-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8e769-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8e769-125">Accept</span></span>|<span data-ttu-id="8e769-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8e769-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e769-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8e769-127">Request body</span></span>
<span data-ttu-id="8e769-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8e769-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8e769-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e769-129">Response</span></span>
<span data-ttu-id="8e769-130">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8e769-130">If successful, this method returns a `200 OK` response code and [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e769-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8e769-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="8e769-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8e769-132">Request</span></span>
<span data-ttu-id="8e769-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8e769-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses/{managedDeviceMobileAppConfigurationUserStatusId}
```

### <a name="response"></a><span data-ttu-id="8e769-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e769-134">Response</span></span>
<span data-ttu-id="8e769-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8e769-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



