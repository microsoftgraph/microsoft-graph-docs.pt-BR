---
title: Criar detectedApp
description: Criar um novo objeto detectedApp.
author: tfitzmac
ms.openlocfilehash: 60c47746e49429e37a5a40a5c86714d209ff6c3d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27355479"
---
# <a name="create-detectedapp"></a><span data-ttu-id="c75fe-103">Criar detectedApp</span><span class="sxs-lookup"><span data-stu-id="c75fe-103">Create detectedApp</span></span>

> <span data-ttu-id="c75fe-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c75fe-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c75fe-105">Criar um novo objeto [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="c75fe-105">Create a new [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c75fe-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c75fe-106">Prerequisites</span></span>
<span data-ttu-id="c75fe-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c75fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c75fe-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c75fe-109">Permission type</span></span>|<span data-ttu-id="c75fe-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c75fe-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c75fe-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c75fe-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c75fe-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c75fe-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c75fe-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c75fe-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c75fe-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c75fe-114">Not supported.</span></span>|
|<span data-ttu-id="c75fe-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c75fe-115">Application</span></span>|<span data-ttu-id="c75fe-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c75fe-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c75fe-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c75fe-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/detectedApps
```

## <a name="request-headers"></a><span data-ttu-id="c75fe-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c75fe-118">Request headers</span></span>
|<span data-ttu-id="c75fe-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c75fe-119">Header</span></span>|<span data-ttu-id="c75fe-120">Valor</span><span class="sxs-lookup"><span data-stu-id="c75fe-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c75fe-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c75fe-121">Authorization</span></span>|<span data-ttu-id="c75fe-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c75fe-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c75fe-123">Accept</span><span class="sxs-lookup"><span data-stu-id="c75fe-123">Accept</span></span>|<span data-ttu-id="c75fe-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c75fe-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c75fe-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c75fe-125">Request body</span></span>
<span data-ttu-id="c75fe-126">No corpo da solicitação, forneça uma representação JSON do objeto detectedApp.</span><span class="sxs-lookup"><span data-stu-id="c75fe-126">In the request body, supply a JSON representation for the detectedApp object.</span></span>

<span data-ttu-id="c75fe-127">A tabela a seguir mostra as propriedades que são necessárias ao criar detectedApp.</span><span class="sxs-lookup"><span data-stu-id="c75fe-127">The following table shows the properties that are required when you create the detectedApp.</span></span>

|<span data-ttu-id="c75fe-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c75fe-128">Property</span></span>|<span data-ttu-id="c75fe-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="c75fe-129">Type</span></span>|<span data-ttu-id="c75fe-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="c75fe-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c75fe-131">id</span><span class="sxs-lookup"><span data-stu-id="c75fe-131">id</span></span>|<span data-ttu-id="c75fe-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c75fe-132">String</span></span>|<span data-ttu-id="c75fe-133">O identificador exclusivo do aplicativo detectado.</span><span class="sxs-lookup"><span data-stu-id="c75fe-133">The unique Identifier for the detected application.</span></span> <span data-ttu-id="c75fe-134">Ele é gerado automaticamente pelo Intune no momento em que o aplicativo é criado.</span><span class="sxs-lookup"><span data-stu-id="c75fe-134">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="c75fe-135">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c75fe-135">Read-only.</span></span>|
|<span data-ttu-id="c75fe-136">displayName</span><span class="sxs-lookup"><span data-stu-id="c75fe-136">displayName</span></span>|<span data-ttu-id="c75fe-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c75fe-137">String</span></span>|<span data-ttu-id="c75fe-138">Nome do aplicativo descoberto.</span><span class="sxs-lookup"><span data-stu-id="c75fe-138">Name of the discovered application.</span></span> <span data-ttu-id="c75fe-139">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="c75fe-139">Read-only</span></span>|
|<span data-ttu-id="c75fe-140">version</span><span class="sxs-lookup"><span data-stu-id="c75fe-140">version</span></span>|<span data-ttu-id="c75fe-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c75fe-141">String</span></span>|<span data-ttu-id="c75fe-142">Versão do aplicativo descoberto.</span><span class="sxs-lookup"><span data-stu-id="c75fe-142">Version of the discovered application.</span></span> <span data-ttu-id="c75fe-143">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="c75fe-143">Read-only</span></span>|
|<span data-ttu-id="c75fe-144">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="c75fe-144">sizeInByte</span></span>|<span data-ttu-id="c75fe-145">Int64</span><span class="sxs-lookup"><span data-stu-id="c75fe-145">Int64</span></span>|<span data-ttu-id="c75fe-146">Tamanho do aplicativo descoberto, em bytes.</span><span class="sxs-lookup"><span data-stu-id="c75fe-146">Discovered application size in bytes.</span></span> <span data-ttu-id="c75fe-147">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="c75fe-147">Read-only</span></span>|
|<span data-ttu-id="c75fe-148">deviceCount</span><span class="sxs-lookup"><span data-stu-id="c75fe-148">deviceCount</span></span>|<span data-ttu-id="c75fe-149">Int32</span><span class="sxs-lookup"><span data-stu-id="c75fe-149">Int32</span></span>|<span data-ttu-id="c75fe-150">O número de dispositivos que instalaram esse aplicativo</span><span class="sxs-lookup"><span data-stu-id="c75fe-150">The number of devices that have installed this application</span></span>|



## <a name="response"></a><span data-ttu-id="c75fe-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="c75fe-151">Response</span></span>
<span data-ttu-id="c75fe-152">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [detectedApp](../resources/intune-devices-detectedapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c75fe-152">If successful, this method returns a `201 Created` response code and a [detectedApp](../resources/intune-devices-detectedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c75fe-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c75fe-153">Example</span></span>
### <a name="request"></a><span data-ttu-id="c75fe-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c75fe-154">Request</span></span>
<span data-ttu-id="c75fe-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c75fe-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/detectedApps
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

### <a name="response"></a><span data-ttu-id="c75fe-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="c75fe-156">Response</span></span>
<span data-ttu-id="c75fe-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c75fe-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



