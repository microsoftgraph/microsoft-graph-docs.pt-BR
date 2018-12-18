---
title: Get iosManagedAppRegistration
description: Ler propriedades e relações do objeto iosManagedAppRegistration.
author: tfitzmac
ms.openlocfilehash: 0199362bdc92db6ed45f44a28b135327b1cb9a94
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351629"
---
# <a name="get-iosmanagedappregistration"></a><span data-ttu-id="a56cc-103">Get iosManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="a56cc-103">Get iosManagedAppRegistration</span></span>

> <span data-ttu-id="a56cc-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a56cc-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a56cc-105">Ler propriedades e relações do objeto [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="a56cc-105">Read properties and relationships of the [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a56cc-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a56cc-106">Prerequisites</span></span>
<span data-ttu-id="a56cc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a56cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a56cc-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a56cc-109">Permission type</span></span>|<span data-ttu-id="a56cc-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a56cc-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a56cc-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a56cc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a56cc-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a56cc-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a56cc-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a56cc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a56cc-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a56cc-114">Not supported.</span></span>|
|<span data-ttu-id="a56cc-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a56cc-115">Application</span></span>|<span data-ttu-id="a56cc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a56cc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a56cc-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a56cc-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a56cc-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a56cc-118">Optional query parameters</span></span>
<span data-ttu-id="a56cc-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a56cc-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a56cc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a56cc-120">Request headers</span></span>
|<span data-ttu-id="a56cc-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a56cc-121">Header</span></span>|<span data-ttu-id="a56cc-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a56cc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a56cc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a56cc-123">Authorization</span></span>|<span data-ttu-id="a56cc-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a56cc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a56cc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a56cc-125">Accept</span></span>|<span data-ttu-id="a56cc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a56cc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a56cc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a56cc-127">Request body</span></span>
<span data-ttu-id="a56cc-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a56cc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a56cc-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a56cc-129">Response</span></span>
<span data-ttu-id="a56cc-130">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a56cc-130">If successful, this method returns a `200 OK` response code and [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a56cc-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a56cc-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="a56cc-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a56cc-132">Request</span></span>
<span data-ttu-id="a56cc-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a56cc-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

### <a name="response"></a><span data-ttu-id="a56cc-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="a56cc-134">Response</span></span>
<span data-ttu-id="a56cc-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a56cc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 800

{
  "value": {
    "@odata.type": "#microsoft.graph.iosManagedAppRegistration",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
    "applicationVersion": "Application Version value",
    "managementSdkVersion": "Management Sdk Version value",
    "platformVersion": "Platform Version value",
    "deviceType": "Device Type value",
    "deviceTag": "Device Tag value",
    "deviceName": "Device Name value",
    "flaggedReasons": [
      "rootedDevice"
    ],
    "userId": "User Id value",
    "appIdentifier": {
      "@odata.type": "microsoft.graph.iosMobileAppIdentifier",
      "bundleId": "Bundle Id value"
    },
    "id": "47632c19-2c19-4763-192c-6347192c6347",
    "version": "Version value"
  }
}
```



