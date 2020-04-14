---
title: Obter deviceCategory
description: Ler propriedades de leitura e relações do objeto deviceCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: df3e73f282d643f65492eb2138bf4c9b7e078871
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43391045"
---
# <a name="get-devicecategory"></a><span data-ttu-id="34107-103">Obter deviceCategory</span><span class="sxs-lookup"><span data-stu-id="34107-103">Get deviceCategory</span></span>

<span data-ttu-id="34107-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34107-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="34107-105">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="34107-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="34107-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="34107-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="34107-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="34107-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34107-108">Ler propriedades de leitura e relações do objeto [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="34107-108">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="34107-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="34107-109">Prerequisites</span></span>

<span data-ttu-id="34107-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34107-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34107-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="34107-112">Permission type</span></span>|<span data-ttu-id="34107-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="34107-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="34107-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="34107-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="34107-115">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="34107-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="34107-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="34107-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="34107-117">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="34107-117">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="34107-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="34107-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="34107-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="34107-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="34107-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="34107-120">Not supported.</span></span>|
|<span data-ttu-id="34107-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="34107-121">Application</span></span>||
| <span data-ttu-id="34107-122">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="34107-122">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="34107-123">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="34107-123">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="34107-124">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="34107-124">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="34107-125">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="34107-125">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="34107-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="34107-126">HTTP Request</span></span>

<span data-ttu-id="34107-127">**Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="34107-127">**Device management**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCategories/{deviceCategoryId}
```

<span data-ttu-id="34107-128">**Integração**</span><span class="sxs-lookup"><span data-stu-id="34107-128">**Onboarding**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
```

## <a name="optional-query-parameters"></a><span data-ttu-id="34107-129">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="34107-129">Optional query parameters</span></span>

<span data-ttu-id="34107-130">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="34107-130">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="34107-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="34107-131">Request headers</span></span>

|<span data-ttu-id="34107-132">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="34107-132">Header</span></span>|<span data-ttu-id="34107-133">Valor</span><span class="sxs-lookup"><span data-stu-id="34107-133">Value</span></span>|
|:---|:---|
|<span data-ttu-id="34107-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="34107-134">Authorization</span></span>|<span data-ttu-id="34107-135">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="34107-135">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="34107-136">Aceitar</span><span class="sxs-lookup"><span data-stu-id="34107-136">Accept</span></span>|<span data-ttu-id="34107-137">application/json</span><span class="sxs-lookup"><span data-stu-id="34107-137">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="34107-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="34107-138">Request body</span></span>

<span data-ttu-id="34107-139">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="34107-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="34107-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="34107-140">Response</span></span>

<span data-ttu-id="34107-141">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceCategory](../resources/intune-shared-devicecategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="34107-141">If successful, this method returns a `200 OK` response code and [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34107-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="34107-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="34107-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="34107-143">Request</span></span>

<span data-ttu-id="34107-144">Veja a seguir exemplos de solicitação.</span><span class="sxs-lookup"><span data-stu-id="34107-144">Here is are examples of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
GET https://graph.microsoft.com/beta/deviceManagement/deviceCategories/{deviceCategoryId}
```

### <a name="response"></a><span data-ttu-id="34107-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="34107-145">Response</span></span>

<span data-ttu-id="34107-146">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="34107-146">Here is an example of the response.</span></span> <span data-ttu-id="34107-147">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="34107-147">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="34107-148">As propriedades retornadas de uma chamada real variam de acordo com o contexto.</span><span class="sxs-lookup"><span data-stu-id="34107-148">Properties returned from an actual call vary according to context.</span></span>

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









