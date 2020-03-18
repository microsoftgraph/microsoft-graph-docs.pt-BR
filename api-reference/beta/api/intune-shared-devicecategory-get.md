---
title: Obter deviceCategory
description: Ler propriedades de leitura e relações do objeto deviceCategory.
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b403fd27136888258f7fedf0e443076446b33d08
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42801233"
---
# <a name="get-devicecategory"></a><span data-ttu-id="fe53f-103">Obter deviceCategory</span><span class="sxs-lookup"><span data-stu-id="fe53f-103">Get deviceCategory</span></span>

> <span data-ttu-id="fe53f-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="fe53f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fe53f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fe53f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fe53f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fe53f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe53f-107">Ler propriedades de leitura e relações do objeto [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="fe53f-107">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fe53f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fe53f-108">Prerequisites</span></span>

<span data-ttu-id="fe53f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe53f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe53f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fe53f-111">Permission type</span></span>|<span data-ttu-id="fe53f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fe53f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fe53f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fe53f-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="fe53f-114">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="fe53f-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="fe53f-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="fe53f-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="fe53f-116">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="fe53f-116">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="fe53f-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="fe53f-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="fe53f-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fe53f-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fe53f-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fe53f-119">Not supported.</span></span>|
|<span data-ttu-id="fe53f-120">Application</span><span class="sxs-lookup"><span data-stu-id="fe53f-120">Application</span></span>||
| <span data-ttu-id="fe53f-121">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="fe53f-121">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="fe53f-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="fe53f-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="fe53f-123">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="fe53f-123">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="fe53f-124">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="fe53f-124">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fe53f-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fe53f-125">HTTP Request</span></span>

<span data-ttu-id="fe53f-126">**Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="fe53f-126">**Device management**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCategories/{deviceCategoryId}
```

<span data-ttu-id="fe53f-127">**Integração**</span><span class="sxs-lookup"><span data-stu-id="fe53f-127">**Onboarding**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fe53f-128">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fe53f-128">Optional query parameters</span></span>

<span data-ttu-id="fe53f-129">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fe53f-129">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fe53f-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fe53f-130">Request headers</span></span>

|<span data-ttu-id="fe53f-131">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fe53f-131">Header</span></span>|<span data-ttu-id="fe53f-132">Valor</span><span class="sxs-lookup"><span data-stu-id="fe53f-132">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fe53f-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="fe53f-133">Authorization</span></span>|<span data-ttu-id="fe53f-134">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fe53f-134">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fe53f-135">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fe53f-135">Accept</span></span>|<span data-ttu-id="fe53f-136">application/json</span><span class="sxs-lookup"><span data-stu-id="fe53f-136">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe53f-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fe53f-137">Request body</span></span>

<span data-ttu-id="fe53f-138">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fe53f-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fe53f-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe53f-139">Response</span></span>

<span data-ttu-id="fe53f-140">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceCategory](../resources/intune-shared-devicecategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fe53f-140">If successful, this method returns a `200 OK` response code and [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe53f-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fe53f-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="fe53f-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fe53f-142">Request</span></span>

<span data-ttu-id="fe53f-143">Veja a seguir exemplos de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fe53f-143">Here is are examples of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
GET https://graph.microsoft.com/beta/deviceManagement/deviceCategories/{deviceCategoryId}
```

### <a name="response"></a><span data-ttu-id="fe53f-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe53f-144">Response</span></span>

<span data-ttu-id="fe53f-145">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fe53f-145">Here is an example of the response.</span></span> <span data-ttu-id="fe53f-146">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="fe53f-146">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="fe53f-147">As propriedades retornadas de uma chamada real variam de acordo com o contexto.</span><span class="sxs-lookup"><span data-stu-id="fe53f-147">Properties returned from an actual call vary according to context.</span></span>

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










