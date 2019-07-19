---
title: Atualizar deviceManagementScriptRunSummary
description: Atualiza as propriedades de um objeto deviceManagementScriptRunSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 58963f558c56b4c26cffb329052d97ce942df999
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34958834"
---
# <a name="update-devicemanagementscriptrunsummary"></a><span data-ttu-id="bcdcd-103">Atualizar deviceManagementScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="bcdcd-103">Update deviceManagementScriptRunSummary</span></span>

> <span data-ttu-id="bcdcd-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bcdcd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bcdcd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bcdcd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bcdcd-106">Atualiza as propriedades de um objeto [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="bcdcd-106">Update the properties of a [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bcdcd-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bcdcd-107">Prerequisites</span></span>
<span data-ttu-id="bcdcd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bcdcd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bcdcd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bcdcd-110">Permission type</span></span>|<span data-ttu-id="bcdcd-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bcdcd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bcdcd-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bcdcd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bcdcd-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bcdcd-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="bcdcd-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bcdcd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bcdcd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bcdcd-115">Not supported.</span></span>|
|<span data-ttu-id="bcdcd-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bcdcd-116">Application</span></span>|<span data-ttu-id="bcdcd-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bcdcd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bcdcd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bcdcd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/runSummary
```

## <a name="request-headers"></a><span data-ttu-id="bcdcd-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bcdcd-119">Request headers</span></span>
|<span data-ttu-id="bcdcd-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bcdcd-120">Header</span></span>|<span data-ttu-id="bcdcd-121">Valor</span><span class="sxs-lookup"><span data-stu-id="bcdcd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bcdcd-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="bcdcd-122">Authorization</span></span>|<span data-ttu-id="bcdcd-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bcdcd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bcdcd-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bcdcd-124">Accept</span></span>|<span data-ttu-id="bcdcd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bcdcd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bcdcd-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bcdcd-126">Request body</span></span>
<span data-ttu-id="bcdcd-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="bcdcd-127">In the request body, supply a JSON representation for the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>

<span data-ttu-id="bcdcd-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md).</span><span class="sxs-lookup"><span data-stu-id="bcdcd-128">The following table shows the properties that are required when you create the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md).</span></span>

|<span data-ttu-id="bcdcd-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bcdcd-129">Property</span></span>|<span data-ttu-id="bcdcd-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="bcdcd-130">Type</span></span>|<span data-ttu-id="bcdcd-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="bcdcd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bcdcd-132">id</span><span class="sxs-lookup"><span data-stu-id="bcdcd-132">id</span></span>|<span data-ttu-id="bcdcd-133">String</span><span class="sxs-lookup"><span data-stu-id="bcdcd-133">String</span></span>|<span data-ttu-id="bcdcd-134">Chave da entidade de Resumo de execução do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bcdcd-134">Key of the device management script run summary entity.</span></span>|
|<span data-ttu-id="bcdcd-135">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bcdcd-135">successDeviceCount</span></span>|<span data-ttu-id="bcdcd-136">Int32</span><span class="sxs-lookup"><span data-stu-id="bcdcd-136">Int32</span></span>|<span data-ttu-id="bcdcd-137">Contagem de dispositivos com êxito.</span><span class="sxs-lookup"><span data-stu-id="bcdcd-137">Success device count.</span></span>|
|<span data-ttu-id="bcdcd-138">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bcdcd-138">errorDeviceCount</span></span>|<span data-ttu-id="bcdcd-139">Int32</span><span class="sxs-lookup"><span data-stu-id="bcdcd-139">Int32</span></span>|<span data-ttu-id="bcdcd-140">Contagem de dispositivos de erro.</span><span class="sxs-lookup"><span data-stu-id="bcdcd-140">Error device count.</span></span>|
|<span data-ttu-id="bcdcd-141">successUserCount</span><span class="sxs-lookup"><span data-stu-id="bcdcd-141">successUserCount</span></span>|<span data-ttu-id="bcdcd-142">Int32</span><span class="sxs-lookup"><span data-stu-id="bcdcd-142">Int32</span></span>|<span data-ttu-id="bcdcd-143">Contagem de usuários com sucesso.</span><span class="sxs-lookup"><span data-stu-id="bcdcd-143">Success user count.</span></span>|
|<span data-ttu-id="bcdcd-144">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="bcdcd-144">errorUserCount</span></span>|<span data-ttu-id="bcdcd-145">Int32</span><span class="sxs-lookup"><span data-stu-id="bcdcd-145">Int32</span></span>|<span data-ttu-id="bcdcd-146">Erro contagem de usuários.</span><span class="sxs-lookup"><span data-stu-id="bcdcd-146">Error user count.</span></span>|



## <a name="response"></a><span data-ttu-id="bcdcd-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="bcdcd-147">Response</span></span>
<span data-ttu-id="bcdcd-148">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bcdcd-148">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bcdcd-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bcdcd-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="bcdcd-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bcdcd-150">Request</span></span>
<span data-ttu-id="bcdcd-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bcdcd-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/runSummary
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

### <a name="response"></a><span data-ttu-id="bcdcd-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="bcdcd-152">Response</span></span>
<span data-ttu-id="bcdcd-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bcdcd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





