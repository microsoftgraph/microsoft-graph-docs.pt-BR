---
title: Obter windowsInformationProtectionDeviceRegistration
description: Leia as propriedades e as relações do objeto windowsInformationProtectionDeviceRegistration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 51e9d78ee7b2c671886e60988cf99e4e7b4d8240
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "38086750"
---
# <a name="get-windowsinformationprotectiondeviceregistration"></a><span data-ttu-id="ec0e1-103">Obter windowsInformationProtectionDeviceRegistration</span><span class="sxs-lookup"><span data-stu-id="ec0e1-103">Get windowsInformationProtectionDeviceRegistration</span></span>

> <span data-ttu-id="ec0e1-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ec0e1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ec0e1-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ec0e1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ec0e1-106">Leia as propriedades e as relações do objeto [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) .</span><span class="sxs-lookup"><span data-stu-id="ec0e1-106">Read properties and relationships of the [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ec0e1-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ec0e1-107">Prerequisites</span></span>
<span data-ttu-id="ec0e1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec0e1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec0e1-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ec0e1-110">Permission type</span></span>|<span data-ttu-id="ec0e1-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ec0e1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ec0e1-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ec0e1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ec0e1-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ec0e1-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="ec0e1-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ec0e1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ec0e1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ec0e1-115">Not supported.</span></span>|
|<span data-ttu-id="ec0e1-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ec0e1-116">Application</span></span>|<span data-ttu-id="ec0e1-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ec0e1-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ec0e1-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ec0e1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/windowsInformationProtectionDeviceRegistrations/{windowsInformationProtectionDeviceRegistrationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ec0e1-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ec0e1-119">Optional query parameters</span></span>
<span data-ttu-id="ec0e1-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ec0e1-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ec0e1-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ec0e1-121">Request headers</span></span>
|<span data-ttu-id="ec0e1-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ec0e1-122">Header</span></span>|<span data-ttu-id="ec0e1-123">Valor</span><span class="sxs-lookup"><span data-stu-id="ec0e1-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ec0e1-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="ec0e1-124">Authorization</span></span>|<span data-ttu-id="ec0e1-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ec0e1-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ec0e1-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ec0e1-126">Accept</span></span>|<span data-ttu-id="ec0e1-127">application/json</span><span class="sxs-lookup"><span data-stu-id="ec0e1-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ec0e1-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ec0e1-128">Request body</span></span>
<span data-ttu-id="ec0e1-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ec0e1-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ec0e1-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec0e1-130">Response</span></span>
<span data-ttu-id="ec0e1-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ec0e1-131">If successful, this method returns a `200 OK` response code and [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec0e1-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ec0e1-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="ec0e1-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ec0e1-133">Request</span></span>
<span data-ttu-id="ec0e1-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ec0e1-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionDeviceRegistrations/{windowsInformationProtectionDeviceRegistrationId}
```

### <a name="response"></a><span data-ttu-id="ec0e1-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec0e1-135">Response</span></span>
<span data-ttu-id="ec0e1-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ec0e1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 450

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsInformationProtectionDeviceRegistration",
    "id": "dd72e2c8-e2c8-dd72-c8e2-72ddc8e272dd",
    "userId": "User Id value",
    "deviceRegistrationId": "Device Registration Id value",
    "deviceName": "Device Name value",
    "deviceType": "Device Type value",
    "deviceMacAddress": "Device Mac Address value",
    "lastCheckInDateTime": "2016-12-31T23:59:56.413532-08:00"
  }
}
```






