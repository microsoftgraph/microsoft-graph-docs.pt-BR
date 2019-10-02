---
title: Get iosManagedAppRegistration
description: Ler propriedades e relações do objeto iosManagedAppRegistration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1d4d4a18a9c04be43d2e7be125520a6c352f6068
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37363763"
---
# <a name="get-iosmanagedappregistration"></a><span data-ttu-id="33607-103">Get iosManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="33607-103">Get iosManagedAppRegistration</span></span>

> <span data-ttu-id="33607-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="33607-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="33607-105">Ler propriedades e relações do objeto [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="33607-105">Read properties and relationships of the [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="33607-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="33607-106">Prerequisites</span></span>
<span data-ttu-id="33607-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33607-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33607-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="33607-109">Permission type</span></span>|<span data-ttu-id="33607-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="33607-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="33607-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="33607-111">Delegated (work or school account)</span></span>|<span data-ttu-id="33607-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="33607-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="33607-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="33607-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="33607-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="33607-114">Not supported.</span></span>|
|<span data-ttu-id="33607-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="33607-115">Application</span></span>|<span data-ttu-id="33607-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="33607-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="33607-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="33607-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="33607-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="33607-118">Optional query parameters</span></span>
<span data-ttu-id="33607-119">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="33607-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="33607-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="33607-120">Request headers</span></span>
|<span data-ttu-id="33607-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="33607-121">Header</span></span>|<span data-ttu-id="33607-122">Valor</span><span class="sxs-lookup"><span data-stu-id="33607-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="33607-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="33607-123">Authorization</span></span>|<span data-ttu-id="33607-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="33607-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="33607-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="33607-125">Accept</span></span>|<span data-ttu-id="33607-126">application/json</span><span class="sxs-lookup"><span data-stu-id="33607-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="33607-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="33607-127">Request body</span></span>
<span data-ttu-id="33607-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="33607-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="33607-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="33607-129">Response</span></span>
<span data-ttu-id="33607-130">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="33607-130">If successful, this method returns a `200 OK` response code and [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33607-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="33607-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="33607-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="33607-132">Request</span></span>
<span data-ttu-id="33607-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="33607-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

### <a name="response"></a><span data-ttu-id="33607-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="33607-134">Response</span></span>
<span data-ttu-id="33607-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="33607-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




