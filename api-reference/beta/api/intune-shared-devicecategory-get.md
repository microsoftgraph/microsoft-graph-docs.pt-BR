---
title: Obter deviceCategory
description: Ler propriedades de leitura e relações do objeto deviceCategory.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f634d5ca490a7ae28ab134dbcbb60fff7f2e1721
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39940149"
---
# <a name="get-devicecategory"></a><span data-ttu-id="109cf-103">Obter deviceCategory</span><span class="sxs-lookup"><span data-stu-id="109cf-103">Get deviceCategory</span></span>

> <span data-ttu-id="109cf-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="109cf-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="109cf-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="109cf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="109cf-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="109cf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="109cf-107">Ler propriedades de leitura e relações do objeto [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="109cf-107">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="109cf-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="109cf-108">Prerequisites</span></span>

<span data-ttu-id="109cf-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="109cf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="109cf-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="109cf-111">Permission type</span></span>|<span data-ttu-id="109cf-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="109cf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="109cf-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="109cf-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="109cf-114">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="109cf-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="109cf-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="109cf-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="109cf-116">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="109cf-116">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="109cf-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="109cf-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="109cf-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="109cf-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="109cf-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="109cf-119">Not supported.</span></span>|
|<span data-ttu-id="109cf-120">Application</span><span class="sxs-lookup"><span data-stu-id="109cf-120">Application</span></span>||
| <span data-ttu-id="109cf-121">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="109cf-121">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="109cf-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="109cf-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="109cf-123">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="109cf-123">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="109cf-124">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="109cf-124">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="109cf-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="109cf-125">HTTP Request</span></span>

<span data-ttu-id="109cf-126">**Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="109cf-126">**Device management**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCategories/{deviceCategoryId}
```

<span data-ttu-id="109cf-127">**Integração**</span><span class="sxs-lookup"><span data-stu-id="109cf-127">**Onboarding**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
```

## <a name="optional-query-parameters"></a><span data-ttu-id="109cf-128">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="109cf-128">Optional query parameters</span></span>

<span data-ttu-id="109cf-129">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="109cf-129">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="109cf-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="109cf-130">Request headers</span></span>

|<span data-ttu-id="109cf-131">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="109cf-131">Header</span></span>|<span data-ttu-id="109cf-132">Valor</span><span class="sxs-lookup"><span data-stu-id="109cf-132">Value</span></span>|
|:---|:---|
|<span data-ttu-id="109cf-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="109cf-133">Authorization</span></span>|<span data-ttu-id="109cf-134">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="109cf-134">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="109cf-135">Aceitar</span><span class="sxs-lookup"><span data-stu-id="109cf-135">Accept</span></span>|<span data-ttu-id="109cf-136">application/json</span><span class="sxs-lookup"><span data-stu-id="109cf-136">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="109cf-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="109cf-137">Request body</span></span>

<span data-ttu-id="109cf-138">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="109cf-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="109cf-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="109cf-139">Response</span></span>

<span data-ttu-id="109cf-140">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceCategory](../resources/intune-shared-devicecategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="109cf-140">If successful, this method returns a `200 OK` response code and [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="109cf-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="109cf-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="109cf-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="109cf-142">Request</span></span>

<span data-ttu-id="109cf-143">Veja a seguir exemplos de solicitação.</span><span class="sxs-lookup"><span data-stu-id="109cf-143">Here is are examples of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
GET https://graph.microsoft.com/beta/deviceManagement/deviceCategories/{deviceCategoryId}
```

### <a name="response"></a><span data-ttu-id="109cf-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="109cf-144">Response</span></span>

<span data-ttu-id="109cf-145">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="109cf-145">Here is an example of the response.</span></span> <span data-ttu-id="109cf-146">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="109cf-146">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="109cf-147">As propriedades retornadas de uma chamada real variam de acordo com o contexto.</span><span class="sxs-lookup"><span data-stu-id="109cf-147">Properties returned from an actual call vary according to context.</span></span>

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











