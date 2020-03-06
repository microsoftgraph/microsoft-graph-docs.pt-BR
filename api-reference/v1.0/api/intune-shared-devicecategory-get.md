---
title: Obter deviceCategory
description: Ler propriedades de leitura e relações do objeto deviceCategory.
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7a158ca444c631e8797ab3f3ce2ec95f525f0f1a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42512094"
---
# <a name="get-devicecategory"></a><span data-ttu-id="bd08c-103">Obter deviceCategory</span><span class="sxs-lookup"><span data-stu-id="bd08c-103">Get deviceCategory</span></span>

<span data-ttu-id="bd08c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bd08c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bd08c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bd08c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bd08c-106">Ler propriedades de leitura e relações do objeto [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="bd08c-106">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bd08c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bd08c-107">Prerequisites</span></span>
<span data-ttu-id="bd08c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd08c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd08c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bd08c-110">Permission type</span></span>|<span data-ttu-id="bd08c-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bd08c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bd08c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bd08c-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="bd08c-113">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="bd08c-113">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="bd08c-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="bd08c-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="bd08c-115">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="bd08c-115">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="bd08c-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="bd08c-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="bd08c-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bd08c-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bd08c-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bd08c-118">Not supported.</span></span>|
|<span data-ttu-id="bd08c-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bd08c-119">Application</span></span>|<span data-ttu-id="bd08c-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bd08c-120">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bd08c-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bd08c-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
GET /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bd08c-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="bd08c-122">Optional query parameters</span></span>
<span data-ttu-id="bd08c-123">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="bd08c-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bd08c-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bd08c-124">Request headers</span></span>
|<span data-ttu-id="bd08c-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bd08c-125">Header</span></span>|<span data-ttu-id="bd08c-126">Valor</span><span class="sxs-lookup"><span data-stu-id="bd08c-126">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bd08c-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="bd08c-127">Authorization</span></span>|<span data-ttu-id="bd08c-128">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bd08c-128">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bd08c-129">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bd08c-129">Accept</span></span>|<span data-ttu-id="bd08c-130">application/json</span><span class="sxs-lookup"><span data-stu-id="bd08c-130">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bd08c-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bd08c-131">Request body</span></span>
<span data-ttu-id="bd08c-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bd08c-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bd08c-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="bd08c-133">Response</span></span>
<span data-ttu-id="bd08c-134">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceCategory](../resources/intune-shared-devicecategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bd08c-134">If successful, this method returns a `200 OK` response code and [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd08c-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bd08c-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="bd08c-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bd08c-136">Request</span></span>
<span data-ttu-id="bd08c-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bd08c-137">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories/{deviceCategoryId}

```

### <a name="response"></a><span data-ttu-id="bd08c-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="bd08c-138">Response</span></span>
<span data-ttu-id="bd08c-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bd08c-139">Here is an example of the response.</span></span> <span data-ttu-id="bd08c-140">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="bd08c-140">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="bd08c-141">As propriedades retornadas de uma chamada real variam de acordo com o contexto.</span><span class="sxs-lookup"><span data-stu-id="bd08c-141">Properties returned from an actual call vary according to context.</span></span>

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




