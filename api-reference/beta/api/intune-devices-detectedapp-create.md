---
title: Criar detectedApp
description: Criar um novo objeto detectedApp.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 24151e64b23e1e0d57485fab82d63eff839eb84a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29393099"
---
# <a name="create-detectedapp"></a><span data-ttu-id="30964-103">Criar detectedApp</span><span class="sxs-lookup"><span data-stu-id="30964-103">Create detectedApp</span></span>

> <span data-ttu-id="30964-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="30964-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="30964-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="30964-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="30964-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="30964-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="30964-107">Criar um novo objeto [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="30964-107">Create a new [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="30964-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="30964-108">Prerequisites</span></span>
<span data-ttu-id="30964-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="30964-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="30964-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="30964-111">Permission type</span></span>|<span data-ttu-id="30964-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="30964-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="30964-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="30964-113">Delegated (work or school account)</span></span>|<span data-ttu-id="30964-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30964-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="30964-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="30964-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="30964-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="30964-116">Not supported.</span></span>|
|<span data-ttu-id="30964-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="30964-117">Application</span></span>|<span data-ttu-id="30964-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="30964-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="30964-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="30964-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/detectedApps
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps
```

## <a name="request-headers"></a><span data-ttu-id="30964-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="30964-120">Request headers</span></span>
|<span data-ttu-id="30964-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="30964-121">Header</span></span>|<span data-ttu-id="30964-122">Valor</span><span class="sxs-lookup"><span data-stu-id="30964-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="30964-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="30964-123">Authorization</span></span>|<span data-ttu-id="30964-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="30964-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="30964-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="30964-125">Accept</span></span>|<span data-ttu-id="30964-126">application/json</span><span class="sxs-lookup"><span data-stu-id="30964-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="30964-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="30964-127">Request body</span></span>
<span data-ttu-id="30964-128">No corpo da solicitação, forneça uma representação JSON do objeto detectedApp.</span><span class="sxs-lookup"><span data-stu-id="30964-128">In the request body, supply a JSON representation for the detectedApp object.</span></span>

<span data-ttu-id="30964-129">A tabela a seguir mostra as propriedades que são necessárias ao criar detectedApp.</span><span class="sxs-lookup"><span data-stu-id="30964-129">The following table shows the properties that are required when you create the detectedApp.</span></span>

|<span data-ttu-id="30964-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="30964-130">Property</span></span>|<span data-ttu-id="30964-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="30964-131">Type</span></span>|<span data-ttu-id="30964-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="30964-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30964-133">id</span><span class="sxs-lookup"><span data-stu-id="30964-133">id</span></span>|<span data-ttu-id="30964-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="30964-134">String</span></span>|<span data-ttu-id="30964-135">O identificador exclusivo do aplicativo detectado.</span><span class="sxs-lookup"><span data-stu-id="30964-135">The unique Identifier for the detected application.</span></span> <span data-ttu-id="30964-136">Ele é gerado automaticamente pelo Intune no momento em que o aplicativo é criado.</span><span class="sxs-lookup"><span data-stu-id="30964-136">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="30964-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="30964-137">Read-only.</span></span>|
|<span data-ttu-id="30964-138">displayName</span><span class="sxs-lookup"><span data-stu-id="30964-138">displayName</span></span>|<span data-ttu-id="30964-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="30964-139">String</span></span>|<span data-ttu-id="30964-140">Nome do aplicativo descoberto.</span><span class="sxs-lookup"><span data-stu-id="30964-140">Name of the discovered application.</span></span> <span data-ttu-id="30964-141">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="30964-141">Read-only</span></span>|
|<span data-ttu-id="30964-142">version</span><span class="sxs-lookup"><span data-stu-id="30964-142">version</span></span>|<span data-ttu-id="30964-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="30964-143">String</span></span>|<span data-ttu-id="30964-144">Versão do aplicativo descoberto.</span><span class="sxs-lookup"><span data-stu-id="30964-144">Version of the discovered application.</span></span> <span data-ttu-id="30964-145">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="30964-145">Read-only</span></span>|
|<span data-ttu-id="30964-146">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="30964-146">sizeInByte</span></span>|<span data-ttu-id="30964-147">Int64</span><span class="sxs-lookup"><span data-stu-id="30964-147">Int64</span></span>|<span data-ttu-id="30964-148">Tamanho do aplicativo descoberto, em bytes.</span><span class="sxs-lookup"><span data-stu-id="30964-148">Discovered application size in bytes.</span></span> <span data-ttu-id="30964-149">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="30964-149">Read-only</span></span>|
|<span data-ttu-id="30964-150">deviceCount</span><span class="sxs-lookup"><span data-stu-id="30964-150">deviceCount</span></span>|<span data-ttu-id="30964-151">Int32</span><span class="sxs-lookup"><span data-stu-id="30964-151">Int32</span></span>|<span data-ttu-id="30964-152">O número de dispositivos que instalaram esse aplicativo</span><span class="sxs-lookup"><span data-stu-id="30964-152">The number of devices that have installed this application</span></span>|



## <a name="response"></a><span data-ttu-id="30964-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="30964-153">Response</span></span>
<span data-ttu-id="30964-154">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [detectedApp](../resources/intune-devices-detectedapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="30964-154">If successful, this method returns a `201 Created` response code and a [detectedApp](../resources/intune-devices-detectedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30964-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="30964-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="30964-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="30964-156">Request</span></span>
<span data-ttu-id="30964-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="30964-157">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/detectedApps
Content-type: application/json
Content-length: 167

{
  "@odata.type": "#microsoft.graph.detectedApp",
  "displayName": "Display Name value",
  "version": "Version value",
  "sizeInByte": 10,
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="30964-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="30964-158">Response</span></span>
<span data-ttu-id="30964-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="30964-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 216

{
  "@odata.type": "#microsoft.graph.detectedApp",
  "id": "caf60db6-0db6-caf6-b60d-f6cab60df6ca",
  "displayName": "Display Name value",
  "version": "Version value",
  "sizeInByte": 10,
  "deviceCount": 11
}
```




