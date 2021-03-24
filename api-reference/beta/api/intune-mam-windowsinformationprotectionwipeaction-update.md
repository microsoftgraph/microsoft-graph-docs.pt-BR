---
title: Atualizar windowsInformationProtectionWipeAction
description: Atualize as propriedades de um objeto windowsInformationProtectionWipeAction.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5b2df26a5aa357d1ebfe6a125049e3a69b1022ae
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51141803"
---
# <a name="update-windowsinformationprotectionwipeaction"></a><span data-ttu-id="781a1-103">Atualizar windowsInformationProtectionWipeAction</span><span class="sxs-lookup"><span data-stu-id="781a1-103">Update windowsInformationProtectionWipeAction</span></span>

<span data-ttu-id="781a1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="781a1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="781a1-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="781a1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="781a1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="781a1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="781a1-107">Atualize as propriedades de um [objeto windowsInformationProtectionWipeAction.](../resources/intune-mam-windowsinformationprotectionwipeaction.md)</span><span class="sxs-lookup"><span data-stu-id="781a1-107">Update the properties of a [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="781a1-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="781a1-108">Prerequisites</span></span>
<span data-ttu-id="781a1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="781a1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="781a1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="781a1-111">Permission type</span></span>|<span data-ttu-id="781a1-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="781a1-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="781a1-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="781a1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="781a1-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="781a1-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="781a1-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="781a1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="781a1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="781a1-116">Not supported.</span></span>|
|<span data-ttu-id="781a1-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="781a1-117">Application</span></span>|<span data-ttu-id="781a1-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="781a1-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="781a1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="781a1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsInformationProtectionWipeActions/{windowsInformationProtectionWipeActionId}
```

## <a name="request-headers"></a><span data-ttu-id="781a1-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="781a1-120">Request headers</span></span>
|<span data-ttu-id="781a1-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="781a1-121">Header</span></span>|<span data-ttu-id="781a1-122">Valor</span><span class="sxs-lookup"><span data-stu-id="781a1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="781a1-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="781a1-123">Authorization</span></span>|<span data-ttu-id="781a1-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="781a1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="781a1-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="781a1-125">Accept</span></span>|<span data-ttu-id="781a1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="781a1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="781a1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="781a1-127">Request body</span></span>
<span data-ttu-id="781a1-128">No corpo da solicitação, fornece uma representação JSON para o [objeto windowsInformationProtectionWipeAction.](../resources/intune-mam-windowsinformationprotectionwipeaction.md)</span><span class="sxs-lookup"><span data-stu-id="781a1-128">In the request body, supply a JSON representation for the [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object.</span></span>

<span data-ttu-id="781a1-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md).</span><span class="sxs-lookup"><span data-stu-id="781a1-129">The following table shows the properties that are required when you create the [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md).</span></span>

|<span data-ttu-id="781a1-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="781a1-130">Property</span></span>|<span data-ttu-id="781a1-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="781a1-131">Type</span></span>|<span data-ttu-id="781a1-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="781a1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="781a1-133">id</span><span class="sxs-lookup"><span data-stu-id="781a1-133">id</span></span>|<span data-ttu-id="781a1-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="781a1-134">String</span></span>|<span data-ttu-id="781a1-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="781a1-135">Key of the entity.</span></span>|
|<span data-ttu-id="781a1-136">status</span><span class="sxs-lookup"><span data-stu-id="781a1-136">status</span></span>|[<span data-ttu-id="781a1-137">actionState</span><span class="sxs-lookup"><span data-stu-id="781a1-137">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="781a1-138">Limpar o status da ação.</span><span class="sxs-lookup"><span data-stu-id="781a1-138">Wipe action status.</span></span> <span data-ttu-id="781a1-139">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="781a1-139">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="781a1-140">targetedUserId</span><span class="sxs-lookup"><span data-stu-id="781a1-140">targetedUserId</span></span>|<span data-ttu-id="781a1-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="781a1-141">String</span></span>|<span data-ttu-id="781a1-142">O UserId que está sendo direcionado por essa ação de limpeza.</span><span class="sxs-lookup"><span data-stu-id="781a1-142">The UserId being targeted by this wipe action.</span></span>|
|<span data-ttu-id="781a1-143">targetedDeviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="781a1-143">targetedDeviceRegistrationId</span></span>|<span data-ttu-id="781a1-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="781a1-144">String</span></span>|<span data-ttu-id="781a1-145">O DeviceRegistrationId que está sendo direcionado por essa ação de limpeza.</span><span class="sxs-lookup"><span data-stu-id="781a1-145">The DeviceRegistrationId being targeted by this wipe action.</span></span>|
|<span data-ttu-id="781a1-146">targetedDeviceName</span><span class="sxs-lookup"><span data-stu-id="781a1-146">targetedDeviceName</span></span>|<span data-ttu-id="781a1-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="781a1-147">String</span></span>|<span data-ttu-id="781a1-148">Nome do dispositivo direcionado.</span><span class="sxs-lookup"><span data-stu-id="781a1-148">Targeted device name.</span></span>|
|<span data-ttu-id="781a1-149">targetedDeviceMacAddress</span><span class="sxs-lookup"><span data-stu-id="781a1-149">targetedDeviceMacAddress</span></span>|<span data-ttu-id="781a1-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="781a1-150">String</span></span>|<span data-ttu-id="781a1-151">Endereço Mac do dispositivo direcionado.</span><span class="sxs-lookup"><span data-stu-id="781a1-151">Targeted device Mac address.</span></span>|
|<span data-ttu-id="781a1-152">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="781a1-152">lastCheckInDateTime</span></span>|<span data-ttu-id="781a1-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="781a1-153">DateTimeOffset</span></span>|<span data-ttu-id="781a1-154">Última verificação no momento do dispositivo que foi direcionado por essa ação de limpeza.</span><span class="sxs-lookup"><span data-stu-id="781a1-154">Last checkin time of the device that was targeted by this wipe action.</span></span>|



## <a name="response"></a><span data-ttu-id="781a1-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="781a1-155">Response</span></span>
<span data-ttu-id="781a1-156">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="781a1-156">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="781a1-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="781a1-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="781a1-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="781a1-158">Request</span></span>
<span data-ttu-id="781a1-159">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="781a1-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="781a1-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="781a1-160">Response</span></span>
<span data-ttu-id="781a1-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="781a1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




