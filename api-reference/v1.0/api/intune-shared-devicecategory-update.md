---
title: Atualizar deviceCategory
description: Atualizar as propriedades de um objeto deviceCategory.
ms.openlocfilehash: 0a236a48877f6d71501fbd0dc6ad35664f766ff2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005456"
---
# <a name="update-devicecategory"></a><span data-ttu-id="788dd-103">Atualizar deviceCategory</span><span class="sxs-lookup"><span data-stu-id="788dd-103">Update deviceCategory</span></span>

> <span data-ttu-id="788dd-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="788dd-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="788dd-105">Atualizar as propriedades de um objeto [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="788dd-105">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="788dd-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="788dd-106">Prerequisites</span></span>
<span data-ttu-id="788dd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="788dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="788dd-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="788dd-109">Permission type</span></span>|<span data-ttu-id="788dd-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="788dd-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="788dd-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="788dd-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="788dd-112">&nbsp;&nbsp; **Onboarding** e</span><span class="sxs-lookup"><span data-stu-id="788dd-112">&nbsp; &nbsp; **Onboarding** and</span></span> <br> <span data-ttu-id="788dd-113">&nbsp;&nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="788dd-113">&nbsp; &nbsp; **Device Management**</span></span>| <span data-ttu-id="788dd-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="788dd-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="788dd-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="788dd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="788dd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="788dd-116">Not supported.</span></span>|
|<span data-ttu-id="788dd-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="788dd-117">Application</span></span>|<span data-ttu-id="788dd-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="788dd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="788dd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="788dd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCategories/{deviceCategoryId}
PATCH /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
```

## <a name="request-headers"></a><span data-ttu-id="788dd-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="788dd-120">Request headers</span></span>
|<span data-ttu-id="788dd-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="788dd-121">Header</span></span>|<span data-ttu-id="788dd-122">Valor</span><span class="sxs-lookup"><span data-stu-id="788dd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="788dd-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="788dd-123">Authorization</span></span>|<span data-ttu-id="788dd-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="788dd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="788dd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="788dd-125">Accept</span></span>|<span data-ttu-id="788dd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="788dd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="788dd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="788dd-127">Request body</span></span>
<span data-ttu-id="788dd-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="788dd-128">In the request body, supply a JSON representation for the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

<span data-ttu-id="788dd-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="788dd-129">The following table shows the properties that are required when you create the [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>

|<span data-ttu-id="788dd-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="788dd-130">Property</span></span>|<span data-ttu-id="788dd-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="788dd-131">Type</span></span>|<span data-ttu-id="788dd-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="788dd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="788dd-133">id</span><span class="sxs-lookup"><span data-stu-id="788dd-133">id</span></span>|<span data-ttu-id="788dd-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="788dd-134">String</span></span>|<span data-ttu-id="788dd-135">O identificador exclusivo da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="788dd-135">Unique identifier for the device category.</span></span> <span data-ttu-id="788dd-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="788dd-136">Read-only.</span></span>|
|<span data-ttu-id="788dd-137">**Inclusão**</span><span class="sxs-lookup"><span data-stu-id="788dd-137">**Onboarding**</span></span>|
|<span data-ttu-id="788dd-138">displayName</span><span class="sxs-lookup"><span data-stu-id="788dd-138">displayName</span></span>|<span data-ttu-id="788dd-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="788dd-139">String</span></span>|<span data-ttu-id="788dd-140">Nome de exibição da categoria de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="788dd-140">Display name for the device category.</span></span>|
|<span data-ttu-id="788dd-141">description</span><span class="sxs-lookup"><span data-stu-id="788dd-141">description</span></span>|<span data-ttu-id="788dd-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="788dd-142">String</span></span>|<span data-ttu-id="788dd-143">Descrição opcional da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="788dd-143">Optional description for the device category.</span></span>|



## <a name="response"></a><span data-ttu-id="788dd-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="788dd-144">Response</span></span>
<span data-ttu-id="788dd-145">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceCategory](../resources/intune-shared-devicecategory.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="788dd-145">If successful, this method returns a `200 OK` response code and an updated [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="788dd-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="788dd-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="788dd-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="788dd-147">Request</span></span>
<span data-ttu-id="788dd-148">Estes são exemplos da solicitação.</span><span class="sxs-lookup"><span data-stu-id="788dd-148">Here are examples of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="788dd-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="788dd-149">Response</span></span>
<span data-ttu-id="788dd-150">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="788dd-150">Here is an example of the response.</span></span> <span data-ttu-id="788dd-151">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="788dd-151">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="788dd-152">Propriedades de resposta irá variar de acordo com o contexto.</span><span class="sxs-lookup"><span data-stu-id="788dd-152">Response properties will vary according to context.</span></span>
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



