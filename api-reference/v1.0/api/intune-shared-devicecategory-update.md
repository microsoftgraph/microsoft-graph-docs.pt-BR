---
title: Atualizar deviceCategory
description: Atualizar as propriedades de um objeto deviceCategory.
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bfd74da1d030b6a424662949d13180cda2a46b6f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42512080"
---
# <a name="update-devicecategory"></a><span data-ttu-id="54ad0-103">Atualizar deviceCategory</span><span class="sxs-lookup"><span data-stu-id="54ad0-103">Update deviceCategory</span></span>

<span data-ttu-id="54ad0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54ad0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="54ad0-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="54ad0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54ad0-106">Atualizar as propriedades de um objeto [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="54ad0-106">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="54ad0-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="54ad0-107">Prerequisites</span></span>
<span data-ttu-id="54ad0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54ad0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54ad0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="54ad0-110">Permission type</span></span>|<span data-ttu-id="54ad0-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="54ad0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="54ad0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="54ad0-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="54ad0-113">&nbsp;&nbsp; **Integração** e</span><span class="sxs-lookup"><span data-stu-id="54ad0-113">&nbsp; &nbsp; **Onboarding** and</span></span> <br> <span data-ttu-id="54ad0-114">&nbsp;&nbsp; **Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="54ad0-114">&nbsp; &nbsp; **Device Management**</span></span>| <span data-ttu-id="54ad0-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54ad0-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="54ad0-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="54ad0-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="54ad0-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="54ad0-117">Not supported.</span></span>|
|<span data-ttu-id="54ad0-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="54ad0-118">Application</span></span>|<span data-ttu-id="54ad0-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="54ad0-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="54ad0-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="54ad0-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCategories/{deviceCategoryId}
PATCH /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
```

## <a name="request-headers"></a><span data-ttu-id="54ad0-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="54ad0-121">Request headers</span></span>
|<span data-ttu-id="54ad0-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="54ad0-122">Header</span></span>|<span data-ttu-id="54ad0-123">Valor</span><span class="sxs-lookup"><span data-stu-id="54ad0-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="54ad0-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="54ad0-124">Authorization</span></span>|<span data-ttu-id="54ad0-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="54ad0-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="54ad0-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="54ad0-126">Accept</span></span>|<span data-ttu-id="54ad0-127">application/json</span><span class="sxs-lookup"><span data-stu-id="54ad0-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="54ad0-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="54ad0-128">Request body</span></span>
<span data-ttu-id="54ad0-129">No corpo da solicitação, forneça uma representação JSON do objeto [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="54ad0-129">In the request body, supply a JSON representation for the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

<span data-ttu-id="54ad0-130">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="54ad0-130">The following table shows the properties that are required when you create the [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>

|<span data-ttu-id="54ad0-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="54ad0-131">Property</span></span>|<span data-ttu-id="54ad0-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="54ad0-132">Type</span></span>|<span data-ttu-id="54ad0-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="54ad0-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54ad0-134">id</span><span class="sxs-lookup"><span data-stu-id="54ad0-134">id</span></span>|<span data-ttu-id="54ad0-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="54ad0-135">String</span></span>|<span data-ttu-id="54ad0-136">O identificador exclusivo da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="54ad0-136">Unique identifier for the device category.</span></span> <span data-ttu-id="54ad0-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="54ad0-137">Read-only.</span></span>|
|<span data-ttu-id="54ad0-138">**Integração**</span><span class="sxs-lookup"><span data-stu-id="54ad0-138">**Onboarding**</span></span>|
|<span data-ttu-id="54ad0-139">displayName</span><span class="sxs-lookup"><span data-stu-id="54ad0-139">displayName</span></span>|<span data-ttu-id="54ad0-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="54ad0-140">String</span></span>|<span data-ttu-id="54ad0-141">Nome de exibição da categoria de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="54ad0-141">Display name for the device category.</span></span>|
|<span data-ttu-id="54ad0-142">description</span><span class="sxs-lookup"><span data-stu-id="54ad0-142">description</span></span>|<span data-ttu-id="54ad0-143">String</span><span class="sxs-lookup"><span data-stu-id="54ad0-143">String</span></span>|<span data-ttu-id="54ad0-144">Descrição opcional da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="54ad0-144">Optional description for the device category.</span></span>|



## <a name="response"></a><span data-ttu-id="54ad0-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="54ad0-145">Response</span></span>
<span data-ttu-id="54ad0-146">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceCategory](../resources/intune-shared-devicecategory.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="54ad0-146">If successful, this method returns a `200 OK` response code and an updated [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="54ad0-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="54ad0-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="54ad0-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="54ad0-148">Request</span></span>
<span data-ttu-id="54ad0-149">Aqui estão exemplos de solicitação.</span><span class="sxs-lookup"><span data-stu-id="54ad0-149">Here are examples of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories/{deviceCategoryId}
Content-type: application/json
Content-length: 82

{
  "displayName": "Display Name value",
  "description": "Description value"
}

PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
```

### <a name="response"></a><span data-ttu-id="54ad0-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="54ad0-150">Response</span></span>
<span data-ttu-id="54ad0-151">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="54ad0-151">Here is an example of the response.</span></span> <span data-ttu-id="54ad0-152">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="54ad0-152">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="54ad0-153">As propriedades de resposta irão variar de acordo com o contexto.</span><span class="sxs-lookup"><span data-stu-id="54ad0-153">Response properties will vary according to context.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 184

{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "f881b841-b841-f881-41b8-81f841b881f8",
  "displayName": "Display Name value",
  "description": "Description value"
}
```




