---
title: Obter deviceCategory
description: Ler propriedades de leitura e relações do objeto deviceCategory.
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5ad4c146eb4a5344b87becdf3e82ae76b0808153
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37361508"
---
# <a name="get-devicecategory"></a><span data-ttu-id="96a36-103">Obter deviceCategory</span><span class="sxs-lookup"><span data-stu-id="96a36-103">Get deviceCategory</span></span>

> <span data-ttu-id="96a36-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="96a36-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="96a36-105">Ler propriedades de leitura e relações do objeto [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="96a36-105">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="96a36-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="96a36-106">Prerequisites</span></span>
<span data-ttu-id="96a36-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96a36-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96a36-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="96a36-109">Permission type</span></span>|<span data-ttu-id="96a36-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="96a36-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="96a36-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="96a36-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="96a36-112">&nbsp;&nbsp; **Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="96a36-112">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="96a36-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="96a36-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="96a36-114">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="96a36-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="96a36-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="96a36-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="96a36-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="96a36-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="96a36-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="96a36-117">Not supported.</span></span>|
|<span data-ttu-id="96a36-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="96a36-118">Application</span></span>|<span data-ttu-id="96a36-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="96a36-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="96a36-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="96a36-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
GET /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="96a36-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="96a36-121">Optional query parameters</span></span>
<span data-ttu-id="96a36-122">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="96a36-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="96a36-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="96a36-123">Request headers</span></span>
|<span data-ttu-id="96a36-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="96a36-124">Header</span></span>|<span data-ttu-id="96a36-125">Valor</span><span class="sxs-lookup"><span data-stu-id="96a36-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="96a36-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="96a36-126">Authorization</span></span>|<span data-ttu-id="96a36-127">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="96a36-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="96a36-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="96a36-128">Accept</span></span>|<span data-ttu-id="96a36-129">application/json</span><span class="sxs-lookup"><span data-stu-id="96a36-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="96a36-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="96a36-130">Request body</span></span>
<span data-ttu-id="96a36-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="96a36-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="96a36-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="96a36-132">Response</span></span>
<span data-ttu-id="96a36-133">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceCategory](../resources/intune-shared-devicecategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="96a36-133">If successful, this method returns a `200 OK` response code and [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96a36-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="96a36-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="96a36-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="96a36-135">Request</span></span>
<span data-ttu-id="96a36-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="96a36-136">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories/{deviceCategoryId}

```

### <a name="response"></a><span data-ttu-id="96a36-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="96a36-137">Response</span></span>
<span data-ttu-id="96a36-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="96a36-138">Here is an example of the response.</span></span> <span data-ttu-id="96a36-139">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="96a36-139">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="96a36-140">As propriedades retornadas de uma chamada real variam de acordo com o contexto.</span><span class="sxs-lookup"><span data-stu-id="96a36-140">Properties returned from an actual call vary according to context.</span></span>

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




