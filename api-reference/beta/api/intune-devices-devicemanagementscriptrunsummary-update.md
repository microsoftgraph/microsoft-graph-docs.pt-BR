---
title: Atualizar deviceManagementScriptRunSummary
description: Atualiza as propriedades de um objeto deviceManagementScriptRunSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c2bce7d7de77f5fabcb1f56747114ab58cf8ed55
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48689563"
---
# <a name="update-devicemanagementscriptrunsummary"></a><span data-ttu-id="fbc42-103">Atualizar deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="fbc42-103">Update deviceManagementScriptRunSummary</span></span>

<span data-ttu-id="fbc42-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fbc42-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fbc42-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fbc42-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fbc42-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fbc42-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fbc42-107">Atualiza as propriedades de um objeto [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="fbc42-107">Update the properties of a [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fbc42-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fbc42-108">Prerequisites</span></span>
<span data-ttu-id="fbc42-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fbc42-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fbc42-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fbc42-111">Permission type</span></span>|<span data-ttu-id="fbc42-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fbc42-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fbc42-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fbc42-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fbc42-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fbc42-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="fbc42-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fbc42-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fbc42-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fbc42-116">Not supported.</span></span>|
|<span data-ttu-id="fbc42-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fbc42-117">Application</span></span>|<span data-ttu-id="fbc42-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fbc42-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fbc42-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fbc42-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceShellScripts/{deviceShellScriptId}/runSummary
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/runSummary
PATCH /deviceManagement/deviceCustomAttributeShellScripts/{deviceCustomAttributeShellScriptId}/runSummary
```

## <a name="request-headers"></a><span data-ttu-id="fbc42-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fbc42-120">Request headers</span></span>
|<span data-ttu-id="fbc42-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fbc42-121">Header</span></span>|<span data-ttu-id="fbc42-122">Valor</span><span class="sxs-lookup"><span data-stu-id="fbc42-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fbc42-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fbc42-123">Authorization</span></span>|<span data-ttu-id="fbc42-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fbc42-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fbc42-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fbc42-125">Accept</span></span>|<span data-ttu-id="fbc42-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fbc42-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fbc42-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fbc42-127">Request body</span></span>
<span data-ttu-id="fbc42-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="fbc42-128">In the request body, supply a JSON representation for the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>

<span data-ttu-id="fbc42-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md).</span><span class="sxs-lookup"><span data-stu-id="fbc42-129">The following table shows the properties that are required when you create the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md).</span></span>

|<span data-ttu-id="fbc42-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fbc42-130">Property</span></span>|<span data-ttu-id="fbc42-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="fbc42-131">Type</span></span>|<span data-ttu-id="fbc42-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="fbc42-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fbc42-133">id</span><span class="sxs-lookup"><span data-stu-id="fbc42-133">id</span></span>|<span data-ttu-id="fbc42-134">String</span><span class="sxs-lookup"><span data-stu-id="fbc42-134">String</span></span>|<span data-ttu-id="fbc42-135">Chave da entidade de Resumo de execução do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fbc42-135">Key of the device management script run summary entity.</span></span> <span data-ttu-id="fbc42-136">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fbc42-136">This property is read-only.</span></span>|
|<span data-ttu-id="fbc42-137">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fbc42-137">successDeviceCount</span></span>|<span data-ttu-id="fbc42-138">Int32</span><span class="sxs-lookup"><span data-stu-id="fbc42-138">Int32</span></span>|<span data-ttu-id="fbc42-139">Contagem de dispositivos com êxito.</span><span class="sxs-lookup"><span data-stu-id="fbc42-139">Success device count.</span></span>|
|<span data-ttu-id="fbc42-140">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fbc42-140">errorDeviceCount</span></span>|<span data-ttu-id="fbc42-141">Int32</span><span class="sxs-lookup"><span data-stu-id="fbc42-141">Int32</span></span>|<span data-ttu-id="fbc42-142">Contagem de dispositivos de erro.</span><span class="sxs-lookup"><span data-stu-id="fbc42-142">Error device count.</span></span>|
|<span data-ttu-id="fbc42-143">successUserCount</span><span class="sxs-lookup"><span data-stu-id="fbc42-143">successUserCount</span></span>|<span data-ttu-id="fbc42-144">Int32</span><span class="sxs-lookup"><span data-stu-id="fbc42-144">Int32</span></span>|<span data-ttu-id="fbc42-145">Contagem de usuários com sucesso.</span><span class="sxs-lookup"><span data-stu-id="fbc42-145">Success user count.</span></span>|
|<span data-ttu-id="fbc42-146">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="fbc42-146">errorUserCount</span></span>|<span data-ttu-id="fbc42-147">Int32</span><span class="sxs-lookup"><span data-stu-id="fbc42-147">Int32</span></span>|<span data-ttu-id="fbc42-148">Erro contagem de usuários.</span><span class="sxs-lookup"><span data-stu-id="fbc42-148">Error user count.</span></span>|



## <a name="response"></a><span data-ttu-id="fbc42-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="fbc42-149">Response</span></span>
<span data-ttu-id="fbc42-150">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fbc42-150">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fbc42-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fbc42-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="fbc42-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fbc42-152">Request</span></span>
<span data-ttu-id="fbc42-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fbc42-153">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/runSummary
Content-type: application/json
Content-length: 179

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptRunSummary",
  "successDeviceCount": 2,
  "errorDeviceCount": 0,
  "successUserCount": 0,
  "errorUserCount": 14
}
```

### <a name="response"></a><span data-ttu-id="fbc42-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="fbc42-154">Response</span></span>
<span data-ttu-id="fbc42-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fbc42-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 228

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptRunSummary",
  "id": "514d5d38-5d38-514d-385d-4d51385d4d51",
  "successDeviceCount": 2,
  "errorDeviceCount": 0,
  "successUserCount": 0,
  "errorUserCount": 14
}
```





