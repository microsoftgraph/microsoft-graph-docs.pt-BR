---
title: Obter deviceCategory
description: Ler propriedades de leitura e relações do objeto deviceCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e371567d984285365fcadb6c2304a560638d0a04
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732208"
---
# <a name="get-devicecategory"></a><span data-ttu-id="9bfd4-103">Obter deviceCategory</span><span class="sxs-lookup"><span data-stu-id="9bfd4-103">Get deviceCategory</span></span>

<span data-ttu-id="9bfd4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9bfd4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9bfd4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9bfd4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9bfd4-106">Ler propriedades de leitura e relações do objeto [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="9bfd4-106">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9bfd4-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9bfd4-107">Prerequisites</span></span>
<span data-ttu-id="9bfd4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9bfd4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9bfd4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9bfd4-110">Permission type</span></span>|<span data-ttu-id="9bfd4-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9bfd4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9bfd4-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9bfd4-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="9bfd4-113">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="9bfd4-113">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="9bfd4-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="9bfd4-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="9bfd4-115">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="9bfd4-115">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="9bfd4-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="9bfd4-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="9bfd4-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9bfd4-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9bfd4-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9bfd4-118">Not supported.</span></span>|
|<span data-ttu-id="9bfd4-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9bfd4-119">Application</span></span>|<span data-ttu-id="9bfd4-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9bfd4-120">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9bfd4-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9bfd4-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
GET /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9bfd4-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9bfd4-122">Optional query parameters</span></span>
<span data-ttu-id="9bfd4-123">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9bfd4-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9bfd4-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9bfd4-124">Request headers</span></span>
|<span data-ttu-id="9bfd4-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9bfd4-125">Header</span></span>|<span data-ttu-id="9bfd4-126">Valor</span><span class="sxs-lookup"><span data-stu-id="9bfd4-126">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9bfd4-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="9bfd4-127">Authorization</span></span>|<span data-ttu-id="9bfd4-128">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9bfd4-128">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9bfd4-129">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9bfd4-129">Accept</span></span>|<span data-ttu-id="9bfd4-130">application/json</span><span class="sxs-lookup"><span data-stu-id="9bfd4-130">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9bfd4-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9bfd4-131">Request body</span></span>
<span data-ttu-id="9bfd4-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9bfd4-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9bfd4-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="9bfd4-133">Response</span></span>
<span data-ttu-id="9bfd4-134">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceCategory](../resources/intune-shared-devicecategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9bfd4-134">If successful, this method returns a `200 OK` response code and [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9bfd4-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9bfd4-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="9bfd4-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9bfd4-136">Request</span></span>
<span data-ttu-id="9bfd4-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9bfd4-137">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories/{deviceCategoryId}

```

### <a name="response"></a><span data-ttu-id="9bfd4-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="9bfd4-138">Response</span></span>
<span data-ttu-id="9bfd4-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9bfd4-139">Here is an example of the response.</span></span> <span data-ttu-id="9bfd4-140">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="9bfd4-140">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="9bfd4-141">As propriedades retornadas de uma chamada real variam de acordo com o contexto.</span><span class="sxs-lookup"><span data-stu-id="9bfd4-141">Properties returned from an actual call vary according to context.</span></span>

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