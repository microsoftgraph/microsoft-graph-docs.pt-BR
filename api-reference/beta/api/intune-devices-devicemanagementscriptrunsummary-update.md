---
title: Atualizar deviceManagementScriptRunSummary
description: Atualiza as propriedades de um objeto deviceManagementScriptRunSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 707f3dd56ea68de21116fd9558be0d260344ab04
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39944915"
---
# <a name="update-devicemanagementscriptrunsummary"></a><span data-ttu-id="267d5-103">Atualizar deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="267d5-103">Update deviceManagementScriptRunSummary</span></span>

> <span data-ttu-id="267d5-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="267d5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="267d5-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="267d5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="267d5-106">Atualiza as propriedades de um objeto [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="267d5-106">Update the properties of a [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="267d5-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="267d5-107">Prerequisites</span></span>
<span data-ttu-id="267d5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="267d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="267d5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="267d5-110">Permission type</span></span>|<span data-ttu-id="267d5-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="267d5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="267d5-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="267d5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="267d5-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="267d5-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="267d5-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="267d5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="267d5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="267d5-115">Not supported.</span></span>|
|<span data-ttu-id="267d5-116">Application</span><span class="sxs-lookup"><span data-stu-id="267d5-116">Application</span></span>|<span data-ttu-id="267d5-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="267d5-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="267d5-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="267d5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceShellScripts/{deviceShellScriptId}/runSummary
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/runSummary
```

## <a name="request-headers"></a><span data-ttu-id="267d5-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="267d5-119">Request headers</span></span>
|<span data-ttu-id="267d5-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="267d5-120">Header</span></span>|<span data-ttu-id="267d5-121">Valor</span><span class="sxs-lookup"><span data-stu-id="267d5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="267d5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="267d5-122">Authorization</span></span>|<span data-ttu-id="267d5-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="267d5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="267d5-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="267d5-124">Accept</span></span>|<span data-ttu-id="267d5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="267d5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="267d5-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="267d5-126">Request body</span></span>
<span data-ttu-id="267d5-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="267d5-127">In the request body, supply a JSON representation for the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>

<span data-ttu-id="267d5-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md).</span><span class="sxs-lookup"><span data-stu-id="267d5-128">The following table shows the properties that are required when you create the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md).</span></span>

|<span data-ttu-id="267d5-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="267d5-129">Property</span></span>|<span data-ttu-id="267d5-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="267d5-130">Type</span></span>|<span data-ttu-id="267d5-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="267d5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="267d5-132">id</span><span class="sxs-lookup"><span data-stu-id="267d5-132">id</span></span>|<span data-ttu-id="267d5-133">String</span><span class="sxs-lookup"><span data-stu-id="267d5-133">String</span></span>|<span data-ttu-id="267d5-134">Chave da entidade de Resumo de execução do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="267d5-134">Key of the device management script run summary entity.</span></span> <span data-ttu-id="267d5-135">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="267d5-135">This property is read-only.</span></span>|
|<span data-ttu-id="267d5-136">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="267d5-136">successDeviceCount</span></span>|<span data-ttu-id="267d5-137">Int32</span><span class="sxs-lookup"><span data-stu-id="267d5-137">Int32</span></span>|<span data-ttu-id="267d5-138">Contagem de dispositivos com êxito.</span><span class="sxs-lookup"><span data-stu-id="267d5-138">Success device count.</span></span>|
|<span data-ttu-id="267d5-139">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="267d5-139">errorDeviceCount</span></span>|<span data-ttu-id="267d5-140">Int32</span><span class="sxs-lookup"><span data-stu-id="267d5-140">Int32</span></span>|<span data-ttu-id="267d5-141">Contagem de dispositivos de erro.</span><span class="sxs-lookup"><span data-stu-id="267d5-141">Error device count.</span></span>|
|<span data-ttu-id="267d5-142">successUserCount</span><span class="sxs-lookup"><span data-stu-id="267d5-142">successUserCount</span></span>|<span data-ttu-id="267d5-143">Int32</span><span class="sxs-lookup"><span data-stu-id="267d5-143">Int32</span></span>|<span data-ttu-id="267d5-144">Contagem de usuários com sucesso.</span><span class="sxs-lookup"><span data-stu-id="267d5-144">Success user count.</span></span>|
|<span data-ttu-id="267d5-145">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="267d5-145">errorUserCount</span></span>|<span data-ttu-id="267d5-146">Int32</span><span class="sxs-lookup"><span data-stu-id="267d5-146">Int32</span></span>|<span data-ttu-id="267d5-147">Erro contagem de usuários.</span><span class="sxs-lookup"><span data-stu-id="267d5-147">Error user count.</span></span>|



## <a name="response"></a><span data-ttu-id="267d5-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="267d5-148">Response</span></span>
<span data-ttu-id="267d5-149">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="267d5-149">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="267d5-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="267d5-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="267d5-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="267d5-151">Request</span></span>
<span data-ttu-id="267d5-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="267d5-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="267d5-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="267d5-153">Response</span></span>
<span data-ttu-id="267d5-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="267d5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





