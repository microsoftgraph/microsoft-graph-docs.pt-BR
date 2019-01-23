---
title: Criar windowsInformationProtectionWipeAction
description: Crie um novo objeto de windowsInformationProtectionWipeAction.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 43b1ffff119e86faa73276770916d5ac26b1ba1a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431234"
---
# <a name="create-windowsinformationprotectionwipeaction"></a><span data-ttu-id="60b51-103">Criar windowsInformationProtectionWipeAction</span><span class="sxs-lookup"><span data-stu-id="60b51-103">Create windowsInformationProtectionWipeAction</span></span>

> <span data-ttu-id="60b51-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="60b51-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="60b51-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="60b51-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="60b51-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="60b51-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="60b51-107">Crie um novo objeto de [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) .</span><span class="sxs-lookup"><span data-stu-id="60b51-107">Create a new [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="60b51-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="60b51-108">Prerequisites</span></span>
<span data-ttu-id="60b51-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="60b51-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="60b51-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="60b51-111">Permission type</span></span>|<span data-ttu-id="60b51-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="60b51-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="60b51-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="60b51-113">Delegated (work or school account)</span></span>|<span data-ttu-id="60b51-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60b51-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="60b51-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="60b51-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="60b51-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="60b51-116">Not supported.</span></span>|
|<span data-ttu-id="60b51-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="60b51-117">Application</span></span>|<span data-ttu-id="60b51-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="60b51-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="60b51-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="60b51-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsInformationProtectionWipeActions
```

## <a name="request-headers"></a><span data-ttu-id="60b51-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="60b51-120">Request headers</span></span>
|<span data-ttu-id="60b51-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="60b51-121">Header</span></span>|<span data-ttu-id="60b51-122">Valor</span><span class="sxs-lookup"><span data-stu-id="60b51-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="60b51-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="60b51-123">Authorization</span></span>|<span data-ttu-id="60b51-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="60b51-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="60b51-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="60b51-125">Accept</span></span>|<span data-ttu-id="60b51-126">application/json</span><span class="sxs-lookup"><span data-stu-id="60b51-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="60b51-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="60b51-127">Request body</span></span>
<span data-ttu-id="60b51-128">No corpo da solicitação, fornece uma representação JSON para o objeto windowsInformationProtectionWipeAction.</span><span class="sxs-lookup"><span data-stu-id="60b51-128">In the request body, supply a JSON representation for the windowsInformationProtectionWipeAction object.</span></span>

<span data-ttu-id="60b51-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o windowsInformationProtectionWipeAction.</span><span class="sxs-lookup"><span data-stu-id="60b51-129">The following table shows the properties that are required when you create the windowsInformationProtectionWipeAction.</span></span>

|<span data-ttu-id="60b51-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="60b51-130">Property</span></span>|<span data-ttu-id="60b51-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="60b51-131">Type</span></span>|<span data-ttu-id="60b51-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="60b51-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60b51-133">id</span><span class="sxs-lookup"><span data-stu-id="60b51-133">id</span></span>|<span data-ttu-id="60b51-134">String</span><span class="sxs-lookup"><span data-stu-id="60b51-134">String</span></span>|<span data-ttu-id="60b51-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="60b51-135">Key of the entity.</span></span>|
|<span data-ttu-id="60b51-136">status</span><span class="sxs-lookup"><span data-stu-id="60b51-136">status</span></span>|[<span data-ttu-id="60b51-137">actionState</span><span class="sxs-lookup"><span data-stu-id="60b51-137">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="60b51-138">Apagar o status da ação.</span><span class="sxs-lookup"><span data-stu-id="60b51-138">Wipe action status.</span></span> <span data-ttu-id="60b51-139">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="60b51-139">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="60b51-140">targetedUserId</span><span class="sxs-lookup"><span data-stu-id="60b51-140">targetedUserId</span></span>|<span data-ttu-id="60b51-141">String</span><span class="sxs-lookup"><span data-stu-id="60b51-141">String</span></span>|<span data-ttu-id="60b51-142">A identificação do usuário que está sendo direcionada por essa ação de limpeza.</span><span class="sxs-lookup"><span data-stu-id="60b51-142">The UserId being targeted by this wipe action.</span></span>|
|<span data-ttu-id="60b51-143">targetedDeviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="60b51-143">targetedDeviceRegistrationId</span></span>|<span data-ttu-id="60b51-144">String</span><span class="sxs-lookup"><span data-stu-id="60b51-144">String</span></span>|<span data-ttu-id="60b51-145">O DeviceRegistrationId sendo direcionada por essa ação de limpeza.</span><span class="sxs-lookup"><span data-stu-id="60b51-145">The DeviceRegistrationId being targeted by this wipe action.</span></span>|
|<span data-ttu-id="60b51-146">targetedDeviceName</span><span class="sxs-lookup"><span data-stu-id="60b51-146">targetedDeviceName</span></span>|<span data-ttu-id="60b51-147">String</span><span class="sxs-lookup"><span data-stu-id="60b51-147">String</span></span>|<span data-ttu-id="60b51-148">Nome do dispositivo de destino.</span><span class="sxs-lookup"><span data-stu-id="60b51-148">Targeted device name.</span></span>|
|<span data-ttu-id="60b51-149">targetedDeviceMacAddress</span><span class="sxs-lookup"><span data-stu-id="60b51-149">targetedDeviceMacAddress</span></span>|<span data-ttu-id="60b51-150">String</span><span class="sxs-lookup"><span data-stu-id="60b51-150">String</span></span>|<span data-ttu-id="60b51-151">Dispositivo direcionado endereço Mac.</span><span class="sxs-lookup"><span data-stu-id="60b51-151">Targeted device Mac address.</span></span>|



## <a name="response"></a><span data-ttu-id="60b51-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="60b51-152">Response</span></span>
<span data-ttu-id="60b51-153">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="60b51-153">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60b51-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="60b51-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="60b51-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="60b51-155">Request</span></span>
<span data-ttu-id="60b51-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="60b51-156">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionWipeActions
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

### <a name="response"></a><span data-ttu-id="60b51-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="60b51-157">Response</span></span>
<span data-ttu-id="60b51-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="60b51-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




