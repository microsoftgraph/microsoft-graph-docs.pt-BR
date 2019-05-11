---
title: Atualizar windowsInformationProtectionWipeAction
description: Atualiza as propriedades de um objeto windowsInformationProtectionWipeAction.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3d04d5bb4c1061840cce33a45494c66b7de7e417
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33900570"
---
# <a name="update-windowsinformationprotectionwipeaction"></a><span data-ttu-id="f3ac1-103">Atualizar windowsInformationProtectionWipeAction</span><span class="sxs-lookup"><span data-stu-id="f3ac1-103">Update windowsInformationProtectionWipeAction</span></span>

> <span data-ttu-id="f3ac1-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f3ac1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3ac1-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f3ac1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3ac1-106">Atualiza as propriedades de um objeto [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) .</span><span class="sxs-lookup"><span data-stu-id="f3ac1-106">Update the properties of a [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f3ac1-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f3ac1-107">Prerequisites</span></span>
<span data-ttu-id="f3ac1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3ac1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3ac1-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f3ac1-110">Permission type</span></span>|<span data-ttu-id="f3ac1-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f3ac1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3ac1-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f3ac1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f3ac1-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3ac1-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f3ac1-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f3ac1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3ac1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f3ac1-115">Not supported.</span></span>|
|<span data-ttu-id="f3ac1-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f3ac1-116">Application</span></span>|<span data-ttu-id="f3ac1-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f3ac1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3ac1-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f3ac1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsInformationProtectionWipeActions/{windowsInformationProtectionWipeActionId}
```

## <a name="request-headers"></a><span data-ttu-id="f3ac1-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f3ac1-119">Request headers</span></span>
|<span data-ttu-id="f3ac1-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f3ac1-120">Header</span></span>|<span data-ttu-id="f3ac1-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f3ac1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f3ac1-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f3ac1-122">Authorization</span></span>|<span data-ttu-id="f3ac1-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f3ac1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f3ac1-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f3ac1-124">Accept</span></span>|<span data-ttu-id="f3ac1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f3ac1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3ac1-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f3ac1-126">Request body</span></span>
<span data-ttu-id="f3ac1-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) .</span><span class="sxs-lookup"><span data-stu-id="f3ac1-127">In the request body, supply a JSON representation for the [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object.</span></span>

<span data-ttu-id="f3ac1-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md).</span><span class="sxs-lookup"><span data-stu-id="f3ac1-128">The following table shows the properties that are required when you create the [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md).</span></span>

|<span data-ttu-id="f3ac1-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f3ac1-129">Property</span></span>|<span data-ttu-id="f3ac1-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f3ac1-130">Type</span></span>|<span data-ttu-id="f3ac1-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3ac1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3ac1-132">id</span><span class="sxs-lookup"><span data-stu-id="f3ac1-132">id</span></span>|<span data-ttu-id="f3ac1-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f3ac1-133">String</span></span>|<span data-ttu-id="f3ac1-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f3ac1-134">Key of the entity.</span></span>|
|<span data-ttu-id="f3ac1-135">status</span><span class="sxs-lookup"><span data-stu-id="f3ac1-135">status</span></span>|[<span data-ttu-id="f3ac1-136">actionState</span><span class="sxs-lookup"><span data-stu-id="f3ac1-136">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="f3ac1-137">Status de ação de apagamento.</span><span class="sxs-lookup"><span data-stu-id="f3ac1-137">Wipe action status.</span></span> <span data-ttu-id="f3ac1-138">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="f3ac1-138">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="f3ac1-139">targetedUserId</span><span class="sxs-lookup"><span data-stu-id="f3ac1-139">targetedUserId</span></span>|<span data-ttu-id="f3ac1-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f3ac1-140">String</span></span>|<span data-ttu-id="f3ac1-141">O UserId que está sendo direcionado para esta ação de apagamento.</span><span class="sxs-lookup"><span data-stu-id="f3ac1-141">The UserId being targeted by this wipe action.</span></span>|
|<span data-ttu-id="f3ac1-142">targetedDeviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="f3ac1-142">targetedDeviceRegistrationId</span></span>|<span data-ttu-id="f3ac1-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f3ac1-143">String</span></span>|<span data-ttu-id="f3ac1-144">O DeviceRegistrationId que está sendo direcionado para esta ação de apagamento.</span><span class="sxs-lookup"><span data-stu-id="f3ac1-144">The DeviceRegistrationId being targeted by this wipe action.</span></span>|
|<span data-ttu-id="f3ac1-145">targetedDeviceName</span><span class="sxs-lookup"><span data-stu-id="f3ac1-145">targetedDeviceName</span></span>|<span data-ttu-id="f3ac1-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f3ac1-146">String</span></span>|<span data-ttu-id="f3ac1-147">Nome do dispositivo de destino.</span><span class="sxs-lookup"><span data-stu-id="f3ac1-147">Targeted device name.</span></span>|
|<span data-ttu-id="f3ac1-148">targetedDeviceMacAddress</span><span class="sxs-lookup"><span data-stu-id="f3ac1-148">targetedDeviceMacAddress</span></span>|<span data-ttu-id="f3ac1-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f3ac1-149">String</span></span>|<span data-ttu-id="f3ac1-150">Endereço MAC do dispositivo de destino.</span><span class="sxs-lookup"><span data-stu-id="f3ac1-150">Targeted device Mac address.</span></span>|
|<span data-ttu-id="f3ac1-151">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="f3ac1-151">lastCheckInDateTime</span></span>|<span data-ttu-id="f3ac1-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3ac1-152">DateTimeOffset</span></span>|<span data-ttu-id="f3ac1-153">Hora da última verificação do dispositivo direcionado por esta ação de apagamento.</span><span class="sxs-lookup"><span data-stu-id="f3ac1-153">Last checkin time of the device that was targeted by this wipe action.</span></span>|



## <a name="response"></a><span data-ttu-id="f3ac1-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3ac1-154">Response</span></span>
<span data-ttu-id="f3ac1-155">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f3ac1-155">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3ac1-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f3ac1-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="f3ac1-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f3ac1-157">Request</span></span>
<span data-ttu-id="f3ac1-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f3ac1-158">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionWipeActions/{windowsInformationProtectionWipeActionId}
Content-type: application/json
Content-length: 412

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionWipeAction",
  "status": "pending",
  "targetedUserId": "Targeted User Id value",
  "targetedDeviceRegistrationId": "Targeted Device Registration Id value",
  "targetedDeviceName": "Targeted Device Name value",
  "targetedDeviceMacAddress": "Targeted Device Mac Address value",
  "lastCheckInDateTime": "2016-12-31T23:59:56.413532-08:00"
}
```

### <a name="response"></a><span data-ttu-id="f3ac1-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3ac1-159">Response</span></span>
<span data-ttu-id="f3ac1-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f3ac1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 461

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionWipeAction",
  "id": "2620a996-a996-2620-96a9-202696a92026",
  "status": "pending",
  "targetedUserId": "Targeted User Id value",
  "targetedDeviceRegistrationId": "Targeted Device Registration Id value",
  "targetedDeviceName": "Targeted Device Name value",
  "targetedDeviceMacAddress": "Targeted Device Mac Address value",
  "lastCheckInDateTime": "2016-12-31T23:59:56.413532-08:00"
}
```




