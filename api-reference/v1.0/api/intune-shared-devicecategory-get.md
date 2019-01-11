---
title: Obter deviceCategory
description: Ler propriedades de leitura e relações do objeto deviceCategory.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ba5fdee5ba2290b25bdf9485b94307f0f637649a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27872188"
---
# <a name="get-devicecategory"></a><span data-ttu-id="ea332-103">Obter deviceCategory</span><span class="sxs-lookup"><span data-stu-id="ea332-103">Get deviceCategory</span></span>



> <span data-ttu-id="ea332-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ea332-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ea332-105">Ler propriedades de leitura e relações do objeto [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="ea332-105">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ea332-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ea332-106">Prerequisites</span></span>
<span data-ttu-id="ea332-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea332-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea332-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ea332-109">Permission type</span></span>|<span data-ttu-id="ea332-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ea332-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ea332-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ea332-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="ea332-112">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="ea332-112">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="ea332-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="ea332-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="ea332-114">&nbsp;&nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="ea332-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="ea332-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="ea332-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="ea332-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ea332-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ea332-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ea332-117">Not supported.</span></span>|
|<span data-ttu-id="ea332-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ea332-118">Application</span></span>|<span data-ttu-id="ea332-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ea332-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ea332-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ea332-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
GET /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ea332-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ea332-121">Optional query parameters</span></span>
<span data-ttu-id="ea332-122">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ea332-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ea332-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ea332-123">Request headers</span></span>
|<span data-ttu-id="ea332-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ea332-124">Header</span></span>|<span data-ttu-id="ea332-125">Valor</span><span class="sxs-lookup"><span data-stu-id="ea332-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ea332-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="ea332-126">Authorization</span></span>|<span data-ttu-id="ea332-127">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ea332-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ea332-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ea332-128">Accept</span></span>|<span data-ttu-id="ea332-129">application/json</span><span class="sxs-lookup"><span data-stu-id="ea332-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea332-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ea332-130">Request body</span></span>
<span data-ttu-id="ea332-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ea332-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ea332-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="ea332-132">Response</span></span>
<span data-ttu-id="ea332-133">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceCategory](../resources/intune-shared-devicecategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ea332-133">If successful, this method returns a `200 OK` response code and [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea332-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ea332-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="ea332-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ea332-135">Request</span></span>
<span data-ttu-id="ea332-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ea332-136">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories/{deviceCategoryId}

```

### <a name="response"></a><span data-ttu-id="ea332-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="ea332-137">Response</span></span>
<span data-ttu-id="ea332-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ea332-138">Here is an example of the response.</span></span> <span data-ttu-id="ea332-139">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="ea332-139">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="ea332-140">Propriedades retornadas de uma chamada real variam de acordo com o contexto.</span><span class="sxs-lookup"><span data-stu-id="ea332-140">Properties returned from an actual call vary according to context.</span></span>

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



