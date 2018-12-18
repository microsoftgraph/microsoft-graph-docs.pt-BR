---
title: Obter deviceCategory
description: Ler propriedades de leitura e relações do objeto deviceCategory.
author: tfitzmac
ms.openlocfilehash: c69e3ecf97889636dd00deab213caf116233f6b6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309694"
---
# <a name="get-devicecategory"></a><span data-ttu-id="0b265-103">Obter deviceCategory</span><span class="sxs-lookup"><span data-stu-id="0b265-103">Get deviceCategory</span></span>



> <span data-ttu-id="0b265-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="0b265-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0b265-105">Ler propriedades de leitura e relações do objeto [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="0b265-105">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0b265-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0b265-106">Prerequisites</span></span>
<span data-ttu-id="0b265-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b265-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b265-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0b265-109">Permission type</span></span>|<span data-ttu-id="0b265-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0b265-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0b265-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0b265-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="0b265-112">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="0b265-112">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="0b265-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="0b265-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="0b265-114">&nbsp;&nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="0b265-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="0b265-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="0b265-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="0b265-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0b265-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b265-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0b265-117">Not supported.</span></span>|
|<span data-ttu-id="0b265-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0b265-118">Application</span></span>|<span data-ttu-id="0b265-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0b265-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b265-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0b265-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
GET /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0b265-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0b265-121">Optional query parameters</span></span>
<span data-ttu-id="0b265-122">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0b265-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0b265-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0b265-123">Request headers</span></span>
|<span data-ttu-id="0b265-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0b265-124">Header</span></span>|<span data-ttu-id="0b265-125">Valor</span><span class="sxs-lookup"><span data-stu-id="0b265-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0b265-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="0b265-126">Authorization</span></span>|<span data-ttu-id="0b265-127">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0b265-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0b265-128">Accept</span><span class="sxs-lookup"><span data-stu-id="0b265-128">Accept</span></span>|<span data-ttu-id="0b265-129">application/json</span><span class="sxs-lookup"><span data-stu-id="0b265-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b265-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0b265-130">Request body</span></span>
<span data-ttu-id="0b265-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0b265-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0b265-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b265-132">Response</span></span>
<span data-ttu-id="0b265-133">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceCategory](../resources/intune-shared-devicecategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0b265-133">If successful, this method returns a `200 OK` response code and [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b265-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0b265-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="0b265-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0b265-135">Request</span></span>
<span data-ttu-id="0b265-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0b265-136">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories/{deviceCategoryId}

```

### <a name="response"></a><span data-ttu-id="0b265-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b265-137">Response</span></span>
<span data-ttu-id="0b265-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0b265-138">Here is an example of the response.</span></span> <span data-ttu-id="0b265-139">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="0b265-139">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="0b265-140">Propriedades retornadas de uma chamada real variam de acordo com o contexto.</span><span class="sxs-lookup"><span data-stu-id="0b265-140">Properties returned from an actual call vary according to context.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 211

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceCategory",
    "id": "f881b841-b841-f881-41b8-81f841b881f8",
    "displayName": "Display Name value",
    "description": "Description value"
  }
}
```



