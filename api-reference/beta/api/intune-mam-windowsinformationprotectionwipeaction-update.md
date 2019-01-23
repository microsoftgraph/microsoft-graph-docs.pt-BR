---
title: Atualizar windowsInformationProtectionWipeAction
description: Atualize as propriedades de um objeto windowsInformationProtectionWipeAction.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f49b79d6ebd12d81332613c646623d68dc0b09a2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429118"
---
# <a name="update-windowsinformationprotectionwipeaction"></a><span data-ttu-id="cf3d3-103">Atualizar windowsInformationProtectionWipeAction</span><span class="sxs-lookup"><span data-stu-id="cf3d3-103">Update windowsInformationProtectionWipeAction</span></span>

> <span data-ttu-id="cf3d3-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="cf3d3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="cf3d3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="cf3d3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cf3d3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="cf3d3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf3d3-107">Atualize as propriedades de um objeto [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) .</span><span class="sxs-lookup"><span data-stu-id="cf3d3-107">Update the properties of a [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cf3d3-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cf3d3-108">Prerequisites</span></span>
<span data-ttu-id="cf3d3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="cf3d3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="cf3d3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cf3d3-111">Permission type</span></span>|<span data-ttu-id="cf3d3-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cf3d3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf3d3-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cf3d3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cf3d3-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf3d3-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cf3d3-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cf3d3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf3d3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cf3d3-116">Not supported.</span></span>|
|<span data-ttu-id="cf3d3-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cf3d3-117">Application</span></span>|<span data-ttu-id="cf3d3-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cf3d3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf3d3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cf3d3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsInformationProtectionWipeActions/{windowsInformationProtectionWipeActionId}
```

## <a name="request-headers"></a><span data-ttu-id="cf3d3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cf3d3-120">Request headers</span></span>
|<span data-ttu-id="cf3d3-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cf3d3-121">Header</span></span>|<span data-ttu-id="cf3d3-122">Valor</span><span class="sxs-lookup"><span data-stu-id="cf3d3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf3d3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="cf3d3-123">Authorization</span></span>|<span data-ttu-id="cf3d3-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cf3d3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf3d3-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cf3d3-125">Accept</span></span>|<span data-ttu-id="cf3d3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cf3d3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf3d3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cf3d3-127">Request body</span></span>
<span data-ttu-id="cf3d3-128">No corpo da solicitação, fornece uma representação JSON para o objeto [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) .</span><span class="sxs-lookup"><span data-stu-id="cf3d3-128">In the request body, supply a JSON representation for the [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object.</span></span>

<span data-ttu-id="cf3d3-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md).</span><span class="sxs-lookup"><span data-stu-id="cf3d3-129">The following table shows the properties that are required when you create the [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md).</span></span>

|<span data-ttu-id="cf3d3-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cf3d3-130">Property</span></span>|<span data-ttu-id="cf3d3-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="cf3d3-131">Type</span></span>|<span data-ttu-id="cf3d3-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf3d3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf3d3-133">id</span><span class="sxs-lookup"><span data-stu-id="cf3d3-133">id</span></span>|<span data-ttu-id="cf3d3-134">String</span><span class="sxs-lookup"><span data-stu-id="cf3d3-134">String</span></span>|<span data-ttu-id="cf3d3-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="cf3d3-135">Key of the entity.</span></span>|
|<span data-ttu-id="cf3d3-136">status</span><span class="sxs-lookup"><span data-stu-id="cf3d3-136">status</span></span>|[<span data-ttu-id="cf3d3-137">actionState</span><span class="sxs-lookup"><span data-stu-id="cf3d3-137">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="cf3d3-138">Apagar o status da ação.</span><span class="sxs-lookup"><span data-stu-id="cf3d3-138">Wipe action status.</span></span> <span data-ttu-id="cf3d3-139">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="cf3d3-139">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="cf3d3-140">targetedUserId</span><span class="sxs-lookup"><span data-stu-id="cf3d3-140">targetedUserId</span></span>|<span data-ttu-id="cf3d3-141">String</span><span class="sxs-lookup"><span data-stu-id="cf3d3-141">String</span></span>|<span data-ttu-id="cf3d3-142">A identificação do usuário que está sendo direcionada por essa ação de limpeza.</span><span class="sxs-lookup"><span data-stu-id="cf3d3-142">The UserId being targeted by this wipe action.</span></span>|
|<span data-ttu-id="cf3d3-143">targetedDeviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="cf3d3-143">targetedDeviceRegistrationId</span></span>|<span data-ttu-id="cf3d3-144">String</span><span class="sxs-lookup"><span data-stu-id="cf3d3-144">String</span></span>|<span data-ttu-id="cf3d3-145">O DeviceRegistrationId sendo direcionada por essa ação de limpeza.</span><span class="sxs-lookup"><span data-stu-id="cf3d3-145">The DeviceRegistrationId being targeted by this wipe action.</span></span>|
|<span data-ttu-id="cf3d3-146">targetedDeviceName</span><span class="sxs-lookup"><span data-stu-id="cf3d3-146">targetedDeviceName</span></span>|<span data-ttu-id="cf3d3-147">String</span><span class="sxs-lookup"><span data-stu-id="cf3d3-147">String</span></span>|<span data-ttu-id="cf3d3-148">Nome do dispositivo de destino.</span><span class="sxs-lookup"><span data-stu-id="cf3d3-148">Targeted device name.</span></span>|
|<span data-ttu-id="cf3d3-149">targetedDeviceMacAddress</span><span class="sxs-lookup"><span data-stu-id="cf3d3-149">targetedDeviceMacAddress</span></span>|<span data-ttu-id="cf3d3-150">String</span><span class="sxs-lookup"><span data-stu-id="cf3d3-150">String</span></span>|<span data-ttu-id="cf3d3-151">Dispositivo direcionado endereço Mac.</span><span class="sxs-lookup"><span data-stu-id="cf3d3-151">Targeted device Mac address.</span></span>|



## <a name="response"></a><span data-ttu-id="cf3d3-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf3d3-152">Response</span></span>
<span data-ttu-id="cf3d3-153">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cf3d3-153">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf3d3-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cf3d3-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="cf3d3-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cf3d3-155">Request</span></span>
<span data-ttu-id="cf3d3-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cf3d3-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionWipeActions/{windowsInformationProtectionWipeActionId}
Content-type: application/json
Content-length: 350

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionWipeAction",
  "status": "pending",
  "targetedUserId": "Targeted User Id value",
  "targetedDeviceRegistrationId": "Targeted Device Registration Id value",
  "targetedDeviceName": "Targeted Device Name value",
  "targetedDeviceMacAddress": "Targeted Device Mac Address value"
}
```

### <a name="response"></a><span data-ttu-id="cf3d3-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf3d3-157">Response</span></span>
<span data-ttu-id="cf3d3-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cf3d3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 399

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionWipeAction",
  "id": "2620a996-a996-2620-96a9-202696a92026",
  "status": "pending",
  "targetedUserId": "Targeted User Id value",
  "targetedDeviceRegistrationId": "Targeted Device Registration Id value",
  "targetedDeviceName": "Targeted Device Name value",
  "targetedDeviceMacAddress": "Targeted Device Mac Address value"
}
```




