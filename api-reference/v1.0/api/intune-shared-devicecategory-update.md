---
title: Atualizar deviceCategory
description: Atualizar as propriedades de um objeto deviceCategory.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b055f8865592e935aaa32e8a3a541151886d36de
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986856"
---
# <a name="update-devicecategory"></a><span data-ttu-id="f5324-103">Atualizar deviceCategory</span><span class="sxs-lookup"><span data-stu-id="f5324-103">Update deviceCategory</span></span>

> <span data-ttu-id="f5324-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f5324-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f5324-105">Atualizar as propriedades de um objeto [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="f5324-105">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f5324-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f5324-106">Prerequisites</span></span>
<span data-ttu-id="f5324-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5324-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5324-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f5324-109">Permission type</span></span>|<span data-ttu-id="f5324-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f5324-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f5324-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f5324-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="f5324-112">&nbsp;&nbsp; **Onboarding** e</span><span class="sxs-lookup"><span data-stu-id="f5324-112">&nbsp; &nbsp; **Onboarding** and</span></span> <br> <span data-ttu-id="f5324-113">&nbsp;&nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="f5324-113">&nbsp; &nbsp; **Device Management**</span></span>| <span data-ttu-id="f5324-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5324-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f5324-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f5324-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f5324-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f5324-116">Not supported.</span></span>|
|<span data-ttu-id="f5324-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f5324-117">Application</span></span>|<span data-ttu-id="f5324-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f5324-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f5324-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f5324-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCategories/{deviceCategoryId}
PATCH /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
```

## <a name="request-headers"></a><span data-ttu-id="f5324-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f5324-120">Request headers</span></span>
|<span data-ttu-id="f5324-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f5324-121">Header</span></span>|<span data-ttu-id="f5324-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f5324-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f5324-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f5324-123">Authorization</span></span>|<span data-ttu-id="f5324-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f5324-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f5324-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f5324-125">Accept</span></span>|<span data-ttu-id="f5324-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f5324-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f5324-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f5324-127">Request body</span></span>
<span data-ttu-id="f5324-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="f5324-128">In the request body, supply a JSON representation for the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

<span data-ttu-id="f5324-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="f5324-129">The following table shows the properties that are required when you create the [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>

|<span data-ttu-id="f5324-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f5324-130">Property</span></span>|<span data-ttu-id="f5324-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f5324-131">Type</span></span>|<span data-ttu-id="f5324-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5324-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5324-133">id</span><span class="sxs-lookup"><span data-stu-id="f5324-133">id</span></span>|<span data-ttu-id="f5324-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f5324-134">String</span></span>|<span data-ttu-id="f5324-135">O identificador exclusivo da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f5324-135">Unique identifier for the device category.</span></span> <span data-ttu-id="f5324-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f5324-136">Read-only.</span></span>|
|<span data-ttu-id="f5324-137">**Inclusão**</span><span class="sxs-lookup"><span data-stu-id="f5324-137">**Onboarding**</span></span>|
|<span data-ttu-id="f5324-138">displayName</span><span class="sxs-lookup"><span data-stu-id="f5324-138">displayName</span></span>|<span data-ttu-id="f5324-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f5324-139">String</span></span>|<span data-ttu-id="f5324-140">Nome de exibição da categoria de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f5324-140">Display name for the device category.</span></span>|
|<span data-ttu-id="f5324-141">description</span><span class="sxs-lookup"><span data-stu-id="f5324-141">description</span></span>|<span data-ttu-id="f5324-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f5324-142">String</span></span>|<span data-ttu-id="f5324-143">Descrição opcional da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f5324-143">Optional description for the device category.</span></span>|



## <a name="response"></a><span data-ttu-id="f5324-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5324-144">Response</span></span>
<span data-ttu-id="f5324-145">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceCategory](../resources/intune-shared-devicecategory.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f5324-145">If successful, this method returns a `200 OK` response code and an updated [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5324-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f5324-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="f5324-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f5324-147">Request</span></span>
<span data-ttu-id="f5324-148">Estes são exemplos da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f5324-148">Here are examples of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f5324-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5324-149">Response</span></span>
<span data-ttu-id="f5324-150">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f5324-150">Here is an example of the response.</span></span> <span data-ttu-id="f5324-151">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="f5324-151">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="f5324-152">Propriedades de resposta irá variar de acordo com o contexto.</span><span class="sxs-lookup"><span data-stu-id="f5324-152">Response properties will vary according to context.</span></span>
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



