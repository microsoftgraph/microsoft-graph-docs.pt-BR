---
title: Atualizar deviceManagementScriptRunSummary
description: Atualiza as propriedades de um objeto deviceManagementScriptRunSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f07a228ce685ae2ec3fcb502131eac5a6d9271af
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36310287"
---
# <a name="update-devicemanagementscriptrunsummary"></a><span data-ttu-id="f014e-103">Atualizar deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="f014e-103">Update deviceManagementScriptRunSummary</span></span>

> <span data-ttu-id="f014e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f014e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f014e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f014e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f014e-106">Atualiza as propriedades de um objeto [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="f014e-106">Update the properties of a [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f014e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f014e-107">Prerequisites</span></span>
<span data-ttu-id="f014e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f014e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f014e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f014e-110">Permission type</span></span>|<span data-ttu-id="f014e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f014e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f014e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f014e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f014e-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f014e-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f014e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f014e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f014e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f014e-115">Not supported.</span></span>|
|<span data-ttu-id="f014e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f014e-116">Application</span></span>|<span data-ttu-id="f014e-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f014e-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f014e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f014e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/runSummary
```

## <a name="request-headers"></a><span data-ttu-id="f014e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f014e-119">Request headers</span></span>
|<span data-ttu-id="f014e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f014e-120">Header</span></span>|<span data-ttu-id="f014e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f014e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f014e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f014e-122">Authorization</span></span>|<span data-ttu-id="f014e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f014e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f014e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f014e-124">Accept</span></span>|<span data-ttu-id="f014e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f014e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f014e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f014e-126">Request body</span></span>
<span data-ttu-id="f014e-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="f014e-127">In the request body, supply a JSON representation for the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>

<span data-ttu-id="f014e-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md).</span><span class="sxs-lookup"><span data-stu-id="f014e-128">The following table shows the properties that are required when you create the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md).</span></span>

|<span data-ttu-id="f014e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f014e-129">Property</span></span>|<span data-ttu-id="f014e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f014e-130">Type</span></span>|<span data-ttu-id="f014e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f014e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f014e-132">id</span><span class="sxs-lookup"><span data-stu-id="f014e-132">id</span></span>|<span data-ttu-id="f014e-133">String</span><span class="sxs-lookup"><span data-stu-id="f014e-133">String</span></span>|<span data-ttu-id="f014e-134">Chave da entidade de Resumo de execução do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f014e-134">Key of the device management script run summary entity.</span></span>|
|<span data-ttu-id="f014e-135">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f014e-135">successDeviceCount</span></span>|<span data-ttu-id="f014e-136">Int32</span><span class="sxs-lookup"><span data-stu-id="f014e-136">Int32</span></span>|<span data-ttu-id="f014e-137">Contagem de dispositivos com êxito.</span><span class="sxs-lookup"><span data-stu-id="f014e-137">Success device count.</span></span>|
|<span data-ttu-id="f014e-138">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f014e-138">errorDeviceCount</span></span>|<span data-ttu-id="f014e-139">Int32</span><span class="sxs-lookup"><span data-stu-id="f014e-139">Int32</span></span>|<span data-ttu-id="f014e-140">Contagem de dispositivos de erro.</span><span class="sxs-lookup"><span data-stu-id="f014e-140">Error device count.</span></span>|
|<span data-ttu-id="f014e-141">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f014e-141">compliantDeviceCount</span></span>|<span data-ttu-id="f014e-142">Int32</span><span class="sxs-lookup"><span data-stu-id="f014e-142">Int32</span></span>|<span data-ttu-id="f014e-143">Contagem de dispositivos em conformidade.</span><span class="sxs-lookup"><span data-stu-id="f014e-143">Compliant device count.</span></span>|
|<span data-ttu-id="f014e-144">notCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f014e-144">notCompliantDeviceCount</span></span>|<span data-ttu-id="f014e-145">Int32</span><span class="sxs-lookup"><span data-stu-id="f014e-145">Int32</span></span>|<span data-ttu-id="f014e-146">Contagem de dispositivos não compatíveis.</span><span class="sxs-lookup"><span data-stu-id="f014e-146">Not Compliant device count.</span></span>|
|<span data-ttu-id="f014e-147">pendingDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f014e-147">pendingDeviceCount</span></span>|<span data-ttu-id="f014e-148">Int32</span><span class="sxs-lookup"><span data-stu-id="f014e-148">Int32</span></span>|<span data-ttu-id="f014e-149">Contagem de dispositivos pendentes.</span><span class="sxs-lookup"><span data-stu-id="f014e-149">Pending device count.</span></span>|
|<span data-ttu-id="f014e-150">successUserCount</span><span class="sxs-lookup"><span data-stu-id="f014e-150">successUserCount</span></span>|<span data-ttu-id="f014e-151">Int32</span><span class="sxs-lookup"><span data-stu-id="f014e-151">Int32</span></span>|<span data-ttu-id="f014e-152">Contagem de usuários com sucesso.</span><span class="sxs-lookup"><span data-stu-id="f014e-152">Success user count.</span></span>|
|<span data-ttu-id="f014e-153">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="f014e-153">errorUserCount</span></span>|<span data-ttu-id="f014e-154">Int32</span><span class="sxs-lookup"><span data-stu-id="f014e-154">Int32</span></span>|<span data-ttu-id="f014e-155">Erro contagem de usuários.</span><span class="sxs-lookup"><span data-stu-id="f014e-155">Error user count.</span></span>|



## <a name="response"></a><span data-ttu-id="f014e-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="f014e-156">Response</span></span>
<span data-ttu-id="f014e-157">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f014e-157">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f014e-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f014e-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="f014e-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f014e-159">Request</span></span>
<span data-ttu-id="f014e-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f014e-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/runSummary
Content-type: application/json
Content-length: 270

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptRunSummary",
  "successDeviceCount": 2,
  "errorDeviceCount": 0,
  "compliantDeviceCount": 4,
  "notCompliantDeviceCount": 7,
  "pendingDeviceCount": 2,
  "successUserCount": 0,
  "errorUserCount": 14
}
```

### <a name="response"></a><span data-ttu-id="f014e-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="f014e-161">Response</span></span>
<span data-ttu-id="f014e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f014e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 319

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptRunSummary",
  "id": "514d5d38-5d38-514d-385d-4d51385d4d51",
  "successDeviceCount": 2,
  "errorDeviceCount": 0,
  "compliantDeviceCount": 4,
  "notCompliantDeviceCount": 7,
  "pendingDeviceCount": 2,
  "successUserCount": 0,
  "errorUserCount": 14
}
```






