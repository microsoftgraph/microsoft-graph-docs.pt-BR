---
title: Atualizar deviceCategory
description: Atualizar as propriedades de um objeto deviceCategory.
author: tfitzmac
ms.openlocfilehash: 8676067ff4ce34358bcfd8400d28e1d73bd11f68
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321515"
---
# <a name="update-devicecategory"></a><span data-ttu-id="67a8e-103">Atualizar deviceCategory</span><span class="sxs-lookup"><span data-stu-id="67a8e-103">Update deviceCategory</span></span>

> <span data-ttu-id="67a8e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="67a8e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="67a8e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="67a8e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="67a8e-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="67a8e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="67a8e-107">Atualizar as propriedades de um objeto [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="67a8e-107">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="67a8e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="67a8e-108">Prerequisites</span></span>

<span data-ttu-id="67a8e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67a8e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67a8e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="67a8e-111">Permission type</span></span>|<span data-ttu-id="67a8e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="67a8e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="67a8e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="67a8e-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="67a8e-114">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="67a8e-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="67a8e-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67a8e-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="67a8e-116">&nbsp;&nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="67a8e-116">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="67a8e-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67a8e-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="67a8e-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="67a8e-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="67a8e-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="67a8e-119">Not supported.</span></span>|
|<span data-ttu-id="67a8e-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="67a8e-120">Application</span></span>|<span data-ttu-id="67a8e-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="67a8e-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="67a8e-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="67a8e-122">HTTP Request</span></span>

<span data-ttu-id="67a8e-123">**Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="67a8e-123">**Device management**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
```

<span data-ttu-id="67a8e-124">**Nível de contratação**</span><span class="sxs-lookup"><span data-stu-id="67a8e-124">**On-boarding**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="67a8e-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="67a8e-125">Request headers</span></span>

|<span data-ttu-id="67a8e-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="67a8e-126">Header</span></span>|<span data-ttu-id="67a8e-127">Valor</span><span class="sxs-lookup"><span data-stu-id="67a8e-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="67a8e-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="67a8e-128">Authorization</span></span>|<span data-ttu-id="67a8e-129">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="67a8e-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="67a8e-130">Accept</span><span class="sxs-lookup"><span data-stu-id="67a8e-130">Accept</span></span>|<span data-ttu-id="67a8e-131">application/json</span><span class="sxs-lookup"><span data-stu-id="67a8e-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="67a8e-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="67a8e-132">Request body</span></span>

<span data-ttu-id="67a8e-133">No corpo da solicitação, forneça uma representação JSON do objeto [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="67a8e-133">In the request body, supply a JSON representation for the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

<span data-ttu-id="67a8e-134">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="67a8e-134">The following table shows the properties that are required when you create the [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>

|<span data-ttu-id="67a8e-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="67a8e-135">Property</span></span>|<span data-ttu-id="67a8e-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="67a8e-136">Type</span></span>|<span data-ttu-id="67a8e-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="67a8e-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67a8e-138">id</span><span class="sxs-lookup"><span data-stu-id="67a8e-138">id</span></span>|<span data-ttu-id="67a8e-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="67a8e-139">String</span></span>|<span data-ttu-id="67a8e-140">O identificador exclusivo da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="67a8e-140">Unique identifier for the device category.</span></span> <span data-ttu-id="67a8e-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="67a8e-141">Read-only.</span></span>|
|<span data-ttu-id="67a8e-142">**Inclusão**</span><span class="sxs-lookup"><span data-stu-id="67a8e-142">**Onboarding**</span></span>|
|<span data-ttu-id="67a8e-143">description</span><span class="sxs-lookup"><span data-stu-id="67a8e-143">description</span></span>|<span data-ttu-id="67a8e-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="67a8e-144">String</span></span>|<span data-ttu-id="67a8e-145">Descrição opcional da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="67a8e-145">Optional description for the device category.</span></span>|
|<span data-ttu-id="67a8e-146">displayName</span><span class="sxs-lookup"><span data-stu-id="67a8e-146">displayName</span></span>|<span data-ttu-id="67a8e-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="67a8e-147">String</span></span>|<span data-ttu-id="67a8e-148">Nome de exibição da categoria de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="67a8e-148">Display name for the device category.</span></span>|

## <a name="response"></a><span data-ttu-id="67a8e-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="67a8e-149">Response</span></span>

<span data-ttu-id="67a8e-150">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceCategory](../resources/intune-shared-devicecategory.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="67a8e-150">If successful, this method returns a `200 OK` response code and an updated [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67a8e-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="67a8e-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="67a8e-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="67a8e-152">Request</span></span>

<span data-ttu-id="67a8e-153">Estes são exemplos da solicitação.</span><span class="sxs-lookup"><span data-stu-id="67a8e-153">Here are examples of the request.</span></span>

``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCategories/{deviceCategoryId}
Content-type: application/json
Content-length: 82

{
  "displayName": "Display Name value",
  "description": "Description value"
}

PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
```

### <a name="response"></a><span data-ttu-id="67a8e-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="67a8e-154">Response</span></span>

<span data-ttu-id="67a8e-155">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="67a8e-155">Here is an example of the response.</span></span> <span data-ttu-id="67a8e-156">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="67a8e-156">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="67a8e-157">Propriedades de resposta irá variar de acordo com o contexto.</span><span class="sxs-lookup"><span data-stu-id="67a8e-157">Response properties will vary according to context.</span></span>

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



