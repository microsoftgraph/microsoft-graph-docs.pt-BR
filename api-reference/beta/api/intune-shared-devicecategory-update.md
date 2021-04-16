---
title: Atualizar deviceCategory
description: Atualizar as propriedades de um objeto deviceCategory.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: dfb3fa9ba4e5599f0666f50bf30d7e555c67f8d6
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51863405"
---
# <a name="update-devicecategory"></a><span data-ttu-id="552b8-103">Atualizar deviceCategory</span><span class="sxs-lookup"><span data-stu-id="552b8-103">Update deviceCategory</span></span>

<span data-ttu-id="552b8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="552b8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="552b8-105">**Importante:** APIs na versão /beta do Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="552b8-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="552b8-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="552b8-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="552b8-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="552b8-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="552b8-108">Atualizar as propriedades de um objeto [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="552b8-108">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="552b8-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="552b8-109">Prerequisites</span></span>

<span data-ttu-id="552b8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="552b8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="552b8-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="552b8-112">Permission type</span></span>|<span data-ttu-id="552b8-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="552b8-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="552b8-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="552b8-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="552b8-115">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="552b8-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="552b8-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="552b8-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="552b8-117">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="552b8-117">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="552b8-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="552b8-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="552b8-119">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="552b8-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="552b8-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="552b8-120">Not supported.</span></span>|
|<span data-ttu-id="552b8-121">Application</span><span class="sxs-lookup"><span data-stu-id="552b8-121">Application</span></span>||
| <span data-ttu-id="552b8-122">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="552b8-122">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="552b8-123">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="552b8-123">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="552b8-124">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="552b8-124">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="552b8-125">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="552b8-125">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="552b8-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="552b8-126">HTTP Request</span></span>

<span data-ttu-id="552b8-127">**Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="552b8-127">**Device management**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
```

<span data-ttu-id="552b8-128">**Ao abordar**</span><span class="sxs-lookup"><span data-stu-id="552b8-128">**On-boarding**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="552b8-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="552b8-129">Request headers</span></span>

|<span data-ttu-id="552b8-130">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="552b8-130">Header</span></span>|<span data-ttu-id="552b8-131">Valor</span><span class="sxs-lookup"><span data-stu-id="552b8-131">Value</span></span>|
|:---|:---|
|<span data-ttu-id="552b8-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="552b8-132">Authorization</span></span>|<span data-ttu-id="552b8-133">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="552b8-133">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="552b8-134">Aceitar</span><span class="sxs-lookup"><span data-stu-id="552b8-134">Accept</span></span>|<span data-ttu-id="552b8-135">application/json</span><span class="sxs-lookup"><span data-stu-id="552b8-135">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="552b8-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="552b8-136">Request body</span></span>

<span data-ttu-id="552b8-137">No corpo da solicitação, forneça uma representação JSON do objeto [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="552b8-137">In the request body, supply a JSON representation for the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

<span data-ttu-id="552b8-138">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="552b8-138">The following table shows the properties that are required when you create the [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>

|<span data-ttu-id="552b8-139">Propriedade</span><span class="sxs-lookup"><span data-stu-id="552b8-139">Property</span></span>|<span data-ttu-id="552b8-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="552b8-140">Type</span></span>|<span data-ttu-id="552b8-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="552b8-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="552b8-142">id</span><span class="sxs-lookup"><span data-stu-id="552b8-142">id</span></span>|<span data-ttu-id="552b8-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="552b8-143">String</span></span>|<span data-ttu-id="552b8-144">O identificador exclusivo da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="552b8-144">Unique identifier for the device category.</span></span> <span data-ttu-id="552b8-145">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="552b8-145">Read-only.</span></span>|
|<span data-ttu-id="552b8-146">**Integração**</span><span class="sxs-lookup"><span data-stu-id="552b8-146">**Onboarding**</span></span>|
|<span data-ttu-id="552b8-147">description</span><span class="sxs-lookup"><span data-stu-id="552b8-147">description</span></span>|<span data-ttu-id="552b8-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="552b8-148">String</span></span>|<span data-ttu-id="552b8-149">Descrição opcional da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="552b8-149">Optional description for the device category.</span></span>|
|<span data-ttu-id="552b8-150">displayName</span><span class="sxs-lookup"><span data-stu-id="552b8-150">displayName</span></span>|<span data-ttu-id="552b8-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="552b8-151">String</span></span>|<span data-ttu-id="552b8-152">Nome de exibição da categoria de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="552b8-152">Display name for the device category.</span></span>|

## <a name="response"></a><span data-ttu-id="552b8-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="552b8-153">Response</span></span>

<span data-ttu-id="552b8-154">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceCategory](../resources/intune-shared-devicecategory.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="552b8-154">If successful, this method returns a `200 OK` response code and an updated [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="552b8-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="552b8-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="552b8-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="552b8-156">Request</span></span>

<span data-ttu-id="552b8-157">Aqui estão exemplos da solicitação.</span><span class="sxs-lookup"><span data-stu-id="552b8-157">Here are examples of the request.</span></span>

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

### <a name="response"></a><span data-ttu-id="552b8-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="552b8-158">Response</span></span>

<span data-ttu-id="552b8-159">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="552b8-159">Here is an example of the response.</span></span> <span data-ttu-id="552b8-160">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="552b8-160">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="552b8-161">As propriedades de resposta variam de acordo com o contexto.</span><span class="sxs-lookup"><span data-stu-id="552b8-161">Response properties will vary according to context.</span></span>

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










