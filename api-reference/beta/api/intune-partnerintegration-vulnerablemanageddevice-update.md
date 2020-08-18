---
title: Atualizar vulnerableManagedDevice
description: Atualiza as propriedades de um objeto vulnerableManagedDevice.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6b4bea3922bd8d8a4a5222470323545657cfcf2f
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/18/2020
ms.locfileid: "46793172"
---
# <a name="update-vulnerablemanageddevice"></a><span data-ttu-id="e4989-103">Atualizar vulnerableManagedDevice</span><span class="sxs-lookup"><span data-stu-id="e4989-103">Update vulnerableManagedDevice</span></span>

<span data-ttu-id="e4989-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4989-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e4989-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e4989-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e4989-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e4989-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4989-107">Atualiza as propriedades de um objeto [vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md) .</span><span class="sxs-lookup"><span data-stu-id="e4989-107">Update the properties of a [vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e4989-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e4989-108">Prerequisites</span></span>
<span data-ttu-id="e4989-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4989-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4989-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e4989-111">Permission type</span></span>|<span data-ttu-id="e4989-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e4989-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e4989-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e4989-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e4989-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4989-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e4989-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e4989-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4989-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e4989-116">Not supported.</span></span>|
|<span data-ttu-id="e4989-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e4989-117">Application</span></span>|<span data-ttu-id="e4989-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4989-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e4989-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e4989-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH ** Entity URI for microsoft.management.services.api.vulnerableManagedDevice not found
```

## <a name="request-headers"></a><span data-ttu-id="e4989-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e4989-120">Request headers</span></span>
|<span data-ttu-id="e4989-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e4989-121">Header</span></span>|<span data-ttu-id="e4989-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e4989-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e4989-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e4989-123">Authorization</span></span>|<span data-ttu-id="e4989-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e4989-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e4989-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e4989-125">Accept</span></span>|<span data-ttu-id="e4989-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e4989-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4989-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e4989-127">Request body</span></span>
<span data-ttu-id="e4989-128">No corpo da solicitação, forneça uma representação JSON do objeto [vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md) .</span><span class="sxs-lookup"><span data-stu-id="e4989-128">In the request body, supply a JSON representation for the [vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md) object.</span></span>

<span data-ttu-id="e4989-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="e4989-129">The following table shows the properties that are required when you create the [vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md).</span></span>

|<span data-ttu-id="e4989-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e4989-130">Property</span></span>|<span data-ttu-id="e4989-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e4989-131">Type</span></span>|<span data-ttu-id="e4989-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4989-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4989-133">id</span><span class="sxs-lookup"><span data-stu-id="e4989-133">id</span></span>|<span data-ttu-id="e4989-134">String</span><span class="sxs-lookup"><span data-stu-id="e4989-134">String</span></span>|<span data-ttu-id="e4989-135">A chave da entidade e a ID do dispositivo AAD.</span><span class="sxs-lookup"><span data-stu-id="e4989-135">The entity key, and AAD device ID.</span></span>|
|<span data-ttu-id="e4989-136">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="e4989-136">managedDeviceId</span></span>|<span data-ttu-id="e4989-137">String</span><span class="sxs-lookup"><span data-stu-id="e4989-137">String</span></span>|<span data-ttu-id="e4989-138">A ID do dispositivo gerenciado do Intune.</span><span class="sxs-lookup"><span data-stu-id="e4989-138">The Intune managed device ID.</span></span>|
|<span data-ttu-id="e4989-139">displayName</span><span class="sxs-lookup"><span data-stu-id="e4989-139">displayName</span></span>|<span data-ttu-id="e4989-140">String</span><span class="sxs-lookup"><span data-stu-id="e4989-140">String</span></span>|<span data-ttu-id="e4989-141">O nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e4989-141">The device name.</span></span>|
|<span data-ttu-id="e4989-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="e4989-142">lastSyncDateTime</span></span>|<span data-ttu-id="e4989-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4989-143">DateTimeOffset</span></span>|<span data-ttu-id="e4989-144">A data da última sincronização.</span><span class="sxs-lookup"><span data-stu-id="e4989-144">The last sync date.</span></span>|



## <a name="response"></a><span data-ttu-id="e4989-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4989-145">Response</span></span>
<span data-ttu-id="e4989-146">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e4989-146">If successful, this method returns a `200 OK` response code and an updated [vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4989-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e4989-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="e4989-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e4989-148">Request</span></span>
<span data-ttu-id="e4989-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e4989-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta** Entity URI for microsoft.management.services.api.vulnerableManagedDevice not found
Content-type: application/json
Content-length: 214

{
  "@odata.type": "#microsoft.graph.vulnerableManagedDevice",
  "managedDeviceId": "Managed Device Id value",
  "displayName": "Display Name value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00"
}
```

### <a name="response"></a><span data-ttu-id="e4989-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4989-150">Response</span></span>
<span data-ttu-id="e4989-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e4989-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 263

{
  "@odata.type": "#microsoft.graph.vulnerableManagedDevice",
  "id": "e59891d4-91d4-e598-d491-98e5d49198e5",
  "managedDeviceId": "Managed Device Id value",
  "displayName": "Display Name value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00"
}
```



