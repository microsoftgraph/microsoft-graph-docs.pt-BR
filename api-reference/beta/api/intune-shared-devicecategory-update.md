---
title: Atualizar deviceCategory
description: Atualizar as propriedades de um objeto deviceCategory.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: eb2d3bc4f081065f27de1c303f87f9e98700d7b9
ms.sourcegitcommit: f58ff560fa02ac95e296375c143b0922fb6a425c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/19/2019
ms.locfileid: "30572345"
---
# <a name="update-devicecategory"></a><span data-ttu-id="4a827-103">Atualizar deviceCategory</span><span class="sxs-lookup"><span data-stu-id="4a827-103">Update deviceCategory</span></span>

> <span data-ttu-id="4a827-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4a827-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4a827-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4a827-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4a827-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4a827-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a827-107">Atualizar as propriedades de um objeto [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="4a827-107">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4a827-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4a827-108">Prerequisites</span></span>

<span data-ttu-id="4a827-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="4a827-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4a827-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4a827-111">Permission type</span></span>|<span data-ttu-id="4a827-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4a827-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4a827-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4a827-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="4a827-114">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="4a827-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="4a827-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a827-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="4a827-116">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="4a827-116">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="4a827-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a827-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="4a827-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4a827-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4a827-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4a827-119">Not supported.</span></span>|
|<span data-ttu-id="4a827-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4a827-120">Application</span></span>|<span data-ttu-id="4a827-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4a827-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4a827-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4a827-122">HTTP Request</span></span>

<span data-ttu-id="4a827-123">**Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="4a827-123">**Device management**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
```

<span data-ttu-id="4a827-124">**Integração**</span><span class="sxs-lookup"><span data-stu-id="4a827-124">**On-boarding**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="4a827-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4a827-125">Request headers</span></span>

|<span data-ttu-id="4a827-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4a827-126">Header</span></span>|<span data-ttu-id="4a827-127">Valor</span><span class="sxs-lookup"><span data-stu-id="4a827-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4a827-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="4a827-128">Authorization</span></span>|<span data-ttu-id="4a827-129">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4a827-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4a827-130">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4a827-130">Accept</span></span>|<span data-ttu-id="4a827-131">application/json</span><span class="sxs-lookup"><span data-stu-id="4a827-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a827-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4a827-132">Request body</span></span>

<span data-ttu-id="4a827-133">No corpo da solicitação, forneça uma representação JSON do objeto [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="4a827-133">In the request body, supply a JSON representation for the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

<span data-ttu-id="4a827-134">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="4a827-134">The following table shows the properties that are required when you create the [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>

|<span data-ttu-id="4a827-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4a827-135">Property</span></span>|<span data-ttu-id="4a827-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="4a827-136">Type</span></span>|<span data-ttu-id="4a827-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a827-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a827-138">id</span><span class="sxs-lookup"><span data-stu-id="4a827-138">id</span></span>|<span data-ttu-id="4a827-139">String</span><span class="sxs-lookup"><span data-stu-id="4a827-139">String</span></span>|<span data-ttu-id="4a827-140">O identificador exclusivo da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4a827-140">Unique identifier for the device category.</span></span> <span data-ttu-id="4a827-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4a827-141">Read-only.</span></span>|
|<span data-ttu-id="4a827-142">**Integração**</span><span class="sxs-lookup"><span data-stu-id="4a827-142">**Onboarding**</span></span>|
|<span data-ttu-id="4a827-143">descrição</span><span class="sxs-lookup"><span data-stu-id="4a827-143">description</span></span>|<span data-ttu-id="4a827-144">String</span><span class="sxs-lookup"><span data-stu-id="4a827-144">String</span></span>|<span data-ttu-id="4a827-145">Descrição opcional da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4a827-145">Optional description for the device category.</span></span>|
|<span data-ttu-id="4a827-146">displayName</span><span class="sxs-lookup"><span data-stu-id="4a827-146">displayName</span></span>|<span data-ttu-id="4a827-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4a827-147">String</span></span>|<span data-ttu-id="4a827-148">Nome de exibição da categoria de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4a827-148">Display name for the device category.</span></span>|

## <a name="response"></a><span data-ttu-id="4a827-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a827-149">Response</span></span>

<span data-ttu-id="4a827-150">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceCategory](../resources/intune-shared-devicecategory.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4a827-150">If successful, this method returns a `200 OK` response code and an updated [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a827-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4a827-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="4a827-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4a827-152">Request</span></span>

<span data-ttu-id="4a827-153">Aqui estão exemplos de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4a827-153">Here are examples of the request.</span></span>

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

### <a name="response"></a><span data-ttu-id="4a827-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a827-154">Response</span></span>

<span data-ttu-id="4a827-155">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4a827-155">Here is an example of the response.</span></span> <span data-ttu-id="4a827-156">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="4a827-156">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="4a827-157">As propriedades de resposta irão variar de acordo com o contexto.</span><span class="sxs-lookup"><span data-stu-id="4a827-157">Response properties will vary according to context.</span></span>

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



