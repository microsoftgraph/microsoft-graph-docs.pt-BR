---
title: Get androidManagedAppRegistration
description: Ler propriedades e relações do objeto androidManagedAppRegistration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 44388d94550764dfc01409fb4d5283e2d83dd157
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36020763"
---
# <a name="get-androidmanagedappregistration"></a><span data-ttu-id="08ca0-103">Get androidManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="08ca0-103">Get androidManagedAppRegistration</span></span>

> <span data-ttu-id="08ca0-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="08ca0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08ca0-105">Ler propriedades e relações do objeto [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="08ca0-105">Read properties and relationships of the [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="08ca0-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="08ca0-106">Prerequisites</span></span>
<span data-ttu-id="08ca0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08ca0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08ca0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="08ca0-109">Permission type</span></span>|<span data-ttu-id="08ca0-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="08ca0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="08ca0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="08ca0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="08ca0-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="08ca0-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="08ca0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="08ca0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="08ca0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="08ca0-114">Not supported.</span></span>|
|<span data-ttu-id="08ca0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="08ca0-115">Application</span></span>|<span data-ttu-id="08ca0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="08ca0-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="08ca0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="08ca0-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="08ca0-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="08ca0-118">Optional query parameters</span></span>
<span data-ttu-id="08ca0-119">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="08ca0-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="08ca0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="08ca0-120">Request headers</span></span>
|<span data-ttu-id="08ca0-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="08ca0-121">Header</span></span>|<span data-ttu-id="08ca0-122">Valor</span><span class="sxs-lookup"><span data-stu-id="08ca0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="08ca0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="08ca0-123">Authorization</span></span>|<span data-ttu-id="08ca0-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="08ca0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="08ca0-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="08ca0-125">Accept</span></span>|<span data-ttu-id="08ca0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="08ca0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="08ca0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="08ca0-127">Request body</span></span>
<span data-ttu-id="08ca0-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="08ca0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="08ca0-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="08ca0-129">Response</span></span>
<span data-ttu-id="08ca0-130">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="08ca0-130">If successful, this method returns a `200 OK` response code and [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08ca0-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="08ca0-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="08ca0-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="08ca0-132">Request</span></span>
<span data-ttu-id="08ca0-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="08ca0-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

### <a name="response"></a><span data-ttu-id="08ca0-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="08ca0-134">Response</span></span>
<span data-ttu-id="08ca0-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="08ca0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 810

{
  "value": {
    "@odata.type": "#microsoft.graph.androidManagedAppRegistration",
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
      "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
      "packageId": "Package Id value"
    },
    "id": "0e064997-4997-0e06-9749-060e9749060e",
    "version": "Version value"
  }
}
```



