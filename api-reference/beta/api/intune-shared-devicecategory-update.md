---
title: Atualizar deviceCategory
description: Atualizar as propriedades de um objeto deviceCategory.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: aec56692e81ca705cf652e2b5c67c734013d2afb
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "38086211"
---
# <a name="update-devicecategory"></a><span data-ttu-id="b29b6-103">Atualizar deviceCategory</span><span class="sxs-lookup"><span data-stu-id="b29b6-103">Update deviceCategory</span></span>

> <span data-ttu-id="b29b6-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b29b6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b29b6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b29b6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b29b6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b29b6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b29b6-107">Atualizar as propriedades de um objeto [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="b29b6-107">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b29b6-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b29b6-108">Prerequisites</span></span>

<span data-ttu-id="b29b6-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b29b6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b29b6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b29b6-111">Permission type</span></span>|<span data-ttu-id="b29b6-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b29b6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b29b6-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b29b6-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="b29b6-114">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="b29b6-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="b29b6-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b29b6-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="b29b6-116">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="b29b6-116">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="b29b6-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b29b6-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b29b6-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b29b6-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b29b6-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b29b6-119">Not supported.</span></span>|
|<span data-ttu-id="b29b6-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b29b6-120">Application</span></span>||
| <span data-ttu-id="b29b6-121">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="b29b6-121">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="b29b6-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b29b6-122">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="b29b6-123">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="b29b6-123">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="b29b6-124">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b29b6-124">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b29b6-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b29b6-125">HTTP Request</span></span>

<span data-ttu-id="b29b6-126">**Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="b29b6-126">**Device management**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
```

<span data-ttu-id="b29b6-127">**Integração**</span><span class="sxs-lookup"><span data-stu-id="b29b6-127">**On-boarding**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="b29b6-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b29b6-128">Request headers</span></span>

|<span data-ttu-id="b29b6-129">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b29b6-129">Header</span></span>|<span data-ttu-id="b29b6-130">Valor</span><span class="sxs-lookup"><span data-stu-id="b29b6-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b29b6-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="b29b6-131">Authorization</span></span>|<span data-ttu-id="b29b6-132">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b29b6-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b29b6-133">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b29b6-133">Accept</span></span>|<span data-ttu-id="b29b6-134">application/json</span><span class="sxs-lookup"><span data-stu-id="b29b6-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b29b6-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b29b6-135">Request body</span></span>

<span data-ttu-id="b29b6-136">No corpo da solicitação, forneça uma representação JSON do objeto [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="b29b6-136">In the request body, supply a JSON representation for the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

<span data-ttu-id="b29b6-137">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="b29b6-137">The following table shows the properties that are required when you create the [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>

|<span data-ttu-id="b29b6-138">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b29b6-138">Property</span></span>|<span data-ttu-id="b29b6-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="b29b6-139">Type</span></span>|<span data-ttu-id="b29b6-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="b29b6-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b29b6-141">id</span><span class="sxs-lookup"><span data-stu-id="b29b6-141">id</span></span>|<span data-ttu-id="b29b6-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b29b6-142">String</span></span>|<span data-ttu-id="b29b6-143">O identificador exclusivo da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b29b6-143">Unique identifier for the device category.</span></span> <span data-ttu-id="b29b6-144">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b29b6-144">Read-only.</span></span>|
|<span data-ttu-id="b29b6-145">**Integração**</span><span class="sxs-lookup"><span data-stu-id="b29b6-145">**Onboarding**</span></span>|
|<span data-ttu-id="b29b6-146">descrição</span><span class="sxs-lookup"><span data-stu-id="b29b6-146">description</span></span>|<span data-ttu-id="b29b6-147">String</span><span class="sxs-lookup"><span data-stu-id="b29b6-147">String</span></span>|<span data-ttu-id="b29b6-148">Descrição opcional da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b29b6-148">Optional description for the device category.</span></span>|
|<span data-ttu-id="b29b6-149">displayName</span><span class="sxs-lookup"><span data-stu-id="b29b6-149">displayName</span></span>|<span data-ttu-id="b29b6-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b29b6-150">String</span></span>|<span data-ttu-id="b29b6-151">Nome de exibição da categoria de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b29b6-151">Display name for the device category.</span></span>|

## <a name="response"></a><span data-ttu-id="b29b6-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="b29b6-152">Response</span></span>

<span data-ttu-id="b29b6-153">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceCategory](../resources/intune-shared-devicecategory.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b29b6-153">If successful, this method returns a `200 OK` response code and an updated [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b29b6-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b29b6-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="b29b6-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b29b6-155">Request</span></span>

<span data-ttu-id="b29b6-156">Aqui estão exemplos de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b29b6-156">Here are examples of the request.</span></span>

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

### <a name="response"></a><span data-ttu-id="b29b6-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="b29b6-157">Response</span></span>

<span data-ttu-id="b29b6-158">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b29b6-158">Here is an example of the response.</span></span> <span data-ttu-id="b29b6-159">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="b29b6-159">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="b29b6-160">As propriedades de resposta irão variar de acordo com o contexto.</span><span class="sxs-lookup"><span data-stu-id="b29b6-160">Response properties will vary according to context.</span></span>

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












