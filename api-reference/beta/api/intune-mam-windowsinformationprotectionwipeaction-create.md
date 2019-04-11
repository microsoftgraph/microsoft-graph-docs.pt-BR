---
title: Criar windowsInformationProtectionWipeAction
description: Criar um novo objeto windowsInformationProtectionWipeAction.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a99aa4c89e80df93637cde6e3dc4bdd88018c76a
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31790155"
---
# <a name="create-windowsinformationprotectionwipeaction"></a><span data-ttu-id="b2595-103">Criar windowsInformationProtectionWipeAction</span><span class="sxs-lookup"><span data-stu-id="b2595-103">Create windowsInformationProtectionWipeAction</span></span>

> <span data-ttu-id="b2595-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b2595-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b2595-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b2595-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2595-106">Criar um novo objeto [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) .</span><span class="sxs-lookup"><span data-stu-id="b2595-106">Create a new [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b2595-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b2595-107">Prerequisites</span></span>
<span data-ttu-id="b2595-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2595-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2595-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b2595-110">Permission type</span></span>|<span data-ttu-id="b2595-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b2595-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2595-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b2595-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b2595-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2595-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b2595-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b2595-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2595-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b2595-115">Not supported.</span></span>|
|<span data-ttu-id="b2595-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b2595-116">Application</span></span>|<span data-ttu-id="b2595-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b2595-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2595-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b2595-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsInformationProtectionWipeActions
```

## <a name="request-headers"></a><span data-ttu-id="b2595-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b2595-119">Request headers</span></span>
|<span data-ttu-id="b2595-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b2595-120">Header</span></span>|<span data-ttu-id="b2595-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b2595-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b2595-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b2595-122">Authorization</span></span>|<span data-ttu-id="b2595-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b2595-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b2595-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b2595-124">Accept</span></span>|<span data-ttu-id="b2595-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b2595-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2595-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b2595-126">Request body</span></span>
<span data-ttu-id="b2595-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsInformationProtectionWipeAction.</span><span class="sxs-lookup"><span data-stu-id="b2595-127">In the request body, supply a JSON representation for the windowsInformationProtectionWipeAction object.</span></span>

<span data-ttu-id="b2595-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsInformationProtectionWipeAction.</span><span class="sxs-lookup"><span data-stu-id="b2595-128">The following table shows the properties that are required when you create the windowsInformationProtectionWipeAction.</span></span>

|<span data-ttu-id="b2595-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b2595-129">Property</span></span>|<span data-ttu-id="b2595-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b2595-130">Type</span></span>|<span data-ttu-id="b2595-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2595-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2595-132">id</span><span class="sxs-lookup"><span data-stu-id="b2595-132">id</span></span>|<span data-ttu-id="b2595-133">String</span><span class="sxs-lookup"><span data-stu-id="b2595-133">String</span></span>|<span data-ttu-id="b2595-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b2595-134">Key of the entity.</span></span>|
|<span data-ttu-id="b2595-135">status</span><span class="sxs-lookup"><span data-stu-id="b2595-135">status</span></span>|[<span data-ttu-id="b2595-136">actionState</span><span class="sxs-lookup"><span data-stu-id="b2595-136">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="b2595-137">Status de ação de apagamento.</span><span class="sxs-lookup"><span data-stu-id="b2595-137">Wipe action status.</span></span> <span data-ttu-id="b2595-138">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="b2595-138">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="b2595-139">targetedUserId</span><span class="sxs-lookup"><span data-stu-id="b2595-139">targetedUserId</span></span>|<span data-ttu-id="b2595-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2595-140">String</span></span>|<span data-ttu-id="b2595-141">O UserId que está sendo direcionado para esta ação de apagamento.</span><span class="sxs-lookup"><span data-stu-id="b2595-141">The UserId being targeted by this wipe action.</span></span>|
|<span data-ttu-id="b2595-142">targetedDeviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="b2595-142">targetedDeviceRegistrationId</span></span>|<span data-ttu-id="b2595-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2595-143">String</span></span>|<span data-ttu-id="b2595-144">O DeviceRegistrationId que está sendo direcionado para esta ação de apagamento.</span><span class="sxs-lookup"><span data-stu-id="b2595-144">The DeviceRegistrationId being targeted by this wipe action.</span></span>|
|<span data-ttu-id="b2595-145">targetedDeviceName</span><span class="sxs-lookup"><span data-stu-id="b2595-145">targetedDeviceName</span></span>|<span data-ttu-id="b2595-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2595-146">String</span></span>|<span data-ttu-id="b2595-147">Nome do dispositivo de destino.</span><span class="sxs-lookup"><span data-stu-id="b2595-147">Targeted device name.</span></span>|
|<span data-ttu-id="b2595-148">targetedDeviceMacAddress</span><span class="sxs-lookup"><span data-stu-id="b2595-148">targetedDeviceMacAddress</span></span>|<span data-ttu-id="b2595-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2595-149">String</span></span>|<span data-ttu-id="b2595-150">Endereço MAC do dispositivo de destino.</span><span class="sxs-lookup"><span data-stu-id="b2595-150">Targeted device Mac address.</span></span>|
|<span data-ttu-id="b2595-151">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="b2595-151">lastCheckInDateTime</span></span>|<span data-ttu-id="b2595-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2595-152">DateTimeOffset</span></span>|<span data-ttu-id="b2595-153">Hora da última verificação do dispositivo direcionado por esta ação de apagamento.</span><span class="sxs-lookup"><span data-stu-id="b2595-153">Last checkin time of the device that was targeted by this wipe action.</span></span>|



## <a name="response"></a><span data-ttu-id="b2595-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2595-154">Response</span></span>
<span data-ttu-id="b2595-155">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b2595-155">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2595-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b2595-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="b2595-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b2595-157">Request</span></span>
<span data-ttu-id="b2595-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b2595-158">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionWipeActions
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

### <a name="response"></a><span data-ttu-id="b2595-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2595-159">Response</span></span>
<span data-ttu-id="b2595-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b2595-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





