---
title: Atualizar deviceManagementScriptRunSummary
description: Atualiza as propriedades de um objeto deviceManagementScriptRunSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 79938a72b84627cfa27c32e163034562d6737079
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37180451"
---
# <a name="update-devicemanagementscriptrunsummary"></a><span data-ttu-id="b1808-103">Atualizar deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="b1808-103">Update deviceManagementScriptRunSummary</span></span>

> <span data-ttu-id="b1808-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b1808-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b1808-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b1808-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1808-106">Atualiza as propriedades de um objeto [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="b1808-106">Update the properties of a [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b1808-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b1808-107">Prerequisites</span></span>
<span data-ttu-id="b1808-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1808-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1808-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b1808-110">Permission type</span></span>|<span data-ttu-id="b1808-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b1808-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b1808-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b1808-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b1808-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1808-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b1808-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b1808-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b1808-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b1808-115">Not supported.</span></span>|
|<span data-ttu-id="b1808-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b1808-116">Application</span></span>|<span data-ttu-id="b1808-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1808-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1808-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b1808-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/runSummary
```

## <a name="request-headers"></a><span data-ttu-id="b1808-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b1808-119">Request headers</span></span>
|<span data-ttu-id="b1808-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b1808-120">Header</span></span>|<span data-ttu-id="b1808-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b1808-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b1808-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b1808-122">Authorization</span></span>|<span data-ttu-id="b1808-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b1808-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b1808-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b1808-124">Accept</span></span>|<span data-ttu-id="b1808-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b1808-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1808-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b1808-126">Request body</span></span>
<span data-ttu-id="b1808-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="b1808-127">In the request body, supply a JSON representation for the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>

<span data-ttu-id="b1808-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md).</span><span class="sxs-lookup"><span data-stu-id="b1808-128">The following table shows the properties that are required when you create the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md).</span></span>

|<span data-ttu-id="b1808-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b1808-129">Property</span></span>|<span data-ttu-id="b1808-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b1808-130">Type</span></span>|<span data-ttu-id="b1808-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1808-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1808-132">id</span><span class="sxs-lookup"><span data-stu-id="b1808-132">id</span></span>|<span data-ttu-id="b1808-133">String</span><span class="sxs-lookup"><span data-stu-id="b1808-133">String</span></span>|<span data-ttu-id="b1808-134">Chave da entidade de Resumo de execução do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b1808-134">Key of the device management script run summary entity.</span></span> <span data-ttu-id="b1808-135">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b1808-135">This property is read-only.</span></span>|
|<span data-ttu-id="b1808-136">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b1808-136">successDeviceCount</span></span>|<span data-ttu-id="b1808-137">Int32</span><span class="sxs-lookup"><span data-stu-id="b1808-137">Int32</span></span>|<span data-ttu-id="b1808-138">Contagem de dispositivos com êxito.</span><span class="sxs-lookup"><span data-stu-id="b1808-138">Success device count.</span></span>|
|<span data-ttu-id="b1808-139">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b1808-139">errorDeviceCount</span></span>|<span data-ttu-id="b1808-140">Int32</span><span class="sxs-lookup"><span data-stu-id="b1808-140">Int32</span></span>|<span data-ttu-id="b1808-141">Contagem de dispositivos de erro.</span><span class="sxs-lookup"><span data-stu-id="b1808-141">Error device count.</span></span>|
|<span data-ttu-id="b1808-142">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b1808-142">compliantDeviceCount</span></span>|<span data-ttu-id="b1808-143">Int32</span><span class="sxs-lookup"><span data-stu-id="b1808-143">Int32</span></span>|<span data-ttu-id="b1808-144">Contagem de dispositivos em conformidade.</span><span class="sxs-lookup"><span data-stu-id="b1808-144">Compliant device count.</span></span>|
|<span data-ttu-id="b1808-145">notCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b1808-145">notCompliantDeviceCount</span></span>|<span data-ttu-id="b1808-146">Int32</span><span class="sxs-lookup"><span data-stu-id="b1808-146">Int32</span></span>|<span data-ttu-id="b1808-147">Contagem de dispositivos não compatíveis.</span><span class="sxs-lookup"><span data-stu-id="b1808-147">Not Compliant device count.</span></span>|
|<span data-ttu-id="b1808-148">pendingDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b1808-148">pendingDeviceCount</span></span>|<span data-ttu-id="b1808-149">Int32</span><span class="sxs-lookup"><span data-stu-id="b1808-149">Int32</span></span>|<span data-ttu-id="b1808-150">Contagem de dispositivos pendentes.</span><span class="sxs-lookup"><span data-stu-id="b1808-150">Pending device count.</span></span>|
|<span data-ttu-id="b1808-151">successUserCount</span><span class="sxs-lookup"><span data-stu-id="b1808-151">successUserCount</span></span>|<span data-ttu-id="b1808-152">Int32</span><span class="sxs-lookup"><span data-stu-id="b1808-152">Int32</span></span>|<span data-ttu-id="b1808-153">Contagem de usuários com sucesso.</span><span class="sxs-lookup"><span data-stu-id="b1808-153">Success user count.</span></span>|
|<span data-ttu-id="b1808-154">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="b1808-154">errorUserCount</span></span>|<span data-ttu-id="b1808-155">Int32</span><span class="sxs-lookup"><span data-stu-id="b1808-155">Int32</span></span>|<span data-ttu-id="b1808-156">Erro contagem de usuários.</span><span class="sxs-lookup"><span data-stu-id="b1808-156">Error user count.</span></span>|



## <a name="response"></a><span data-ttu-id="b1808-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1808-157">Response</span></span>
<span data-ttu-id="b1808-158">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b1808-158">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1808-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b1808-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="b1808-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b1808-160">Request</span></span>
<span data-ttu-id="b1808-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b1808-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b1808-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1808-162">Response</span></span>
<span data-ttu-id="b1808-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b1808-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




