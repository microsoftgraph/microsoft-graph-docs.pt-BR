---
title: Criar vulnerableManagedDevice
description: Criar um novo objeto vulnerableManagedDevice.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8b5cb5d836ff6eb98df7915cd05a308f7b1626b3
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48709198"
---
# <a name="create-vulnerablemanageddevice"></a><span data-ttu-id="65fe2-103">Criar vulnerableManagedDevice</span><span class="sxs-lookup"><span data-stu-id="65fe2-103">Create vulnerableManagedDevice</span></span>

<span data-ttu-id="65fe2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65fe2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="65fe2-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="65fe2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="65fe2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="65fe2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65fe2-107">Criar um novo objeto [vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md) .</span><span class="sxs-lookup"><span data-stu-id="65fe2-107">Create a new [vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="65fe2-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="65fe2-108">Prerequisites</span></span>
<span data-ttu-id="65fe2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="65fe2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65fe2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="65fe2-111">Permission type</span></span>|<span data-ttu-id="65fe2-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="65fe2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="65fe2-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="65fe2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="65fe2-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65fe2-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="65fe2-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="65fe2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="65fe2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="65fe2-116">Not supported.</span></span>|
|<span data-ttu-id="65fe2-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="65fe2-117">Application</span></span>|<span data-ttu-id="65fe2-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65fe2-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="65fe2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="65fe2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST ** Collection URI for microsoft.management.services.api.vulnerableManagedDevice not found
```

## <a name="request-headers"></a><span data-ttu-id="65fe2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="65fe2-120">Request headers</span></span>
|<span data-ttu-id="65fe2-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="65fe2-121">Header</span></span>|<span data-ttu-id="65fe2-122">Valor</span><span class="sxs-lookup"><span data-stu-id="65fe2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="65fe2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="65fe2-123">Authorization</span></span>|<span data-ttu-id="65fe2-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="65fe2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="65fe2-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="65fe2-125">Accept</span></span>|<span data-ttu-id="65fe2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="65fe2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="65fe2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="65fe2-127">Request body</span></span>
<span data-ttu-id="65fe2-128">No corpo da solicitação, forneça uma representação JSON do objeto vulnerableManagedDevice.</span><span class="sxs-lookup"><span data-stu-id="65fe2-128">In the request body, supply a JSON representation for the vulnerableManagedDevice object.</span></span>

<span data-ttu-id="65fe2-129">A tabela a seguir mostra as propriedades que são necessárias ao criar vulnerableManagedDevice.</span><span class="sxs-lookup"><span data-stu-id="65fe2-129">The following table shows the properties that are required when you create the vulnerableManagedDevice.</span></span>

|<span data-ttu-id="65fe2-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="65fe2-130">Property</span></span>|<span data-ttu-id="65fe2-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="65fe2-131">Type</span></span>|<span data-ttu-id="65fe2-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="65fe2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65fe2-133">id</span><span class="sxs-lookup"><span data-stu-id="65fe2-133">id</span></span>|<span data-ttu-id="65fe2-134">String</span><span class="sxs-lookup"><span data-stu-id="65fe2-134">String</span></span>|<span data-ttu-id="65fe2-135">A chave da entidade e a ID do dispositivo AAD.</span><span class="sxs-lookup"><span data-stu-id="65fe2-135">The entity key, and AAD device ID.</span></span>|
|<span data-ttu-id="65fe2-136">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="65fe2-136">managedDeviceId</span></span>|<span data-ttu-id="65fe2-137">String</span><span class="sxs-lookup"><span data-stu-id="65fe2-137">String</span></span>|<span data-ttu-id="65fe2-138">A ID do dispositivo gerenciado do Intune.</span><span class="sxs-lookup"><span data-stu-id="65fe2-138">The Intune managed device ID.</span></span>|
|<span data-ttu-id="65fe2-139">displayName</span><span class="sxs-lookup"><span data-stu-id="65fe2-139">displayName</span></span>|<span data-ttu-id="65fe2-140">String</span><span class="sxs-lookup"><span data-stu-id="65fe2-140">String</span></span>|<span data-ttu-id="65fe2-141">O nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="65fe2-141">The device name.</span></span>|
|<span data-ttu-id="65fe2-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="65fe2-142">lastSyncDateTime</span></span>|<span data-ttu-id="65fe2-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65fe2-143">DateTimeOffset</span></span>|<span data-ttu-id="65fe2-144">A data da última sincronização.</span><span class="sxs-lookup"><span data-stu-id="65fe2-144">The last sync date.</span></span>|



## <a name="response"></a><span data-ttu-id="65fe2-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="65fe2-145">Response</span></span>
<span data-ttu-id="65fe2-146">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="65fe2-146">If successful, this method returns a `201 Created` response code and a [vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65fe2-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="65fe2-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="65fe2-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="65fe2-148">Request</span></span>
<span data-ttu-id="65fe2-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="65fe2-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta** Collection URI for microsoft.management.services.api.vulnerableManagedDevice not found
Content-type: application/json
Content-length: 214

{
  "@odata.type": "#microsoft.graph.vulnerableManagedDevice",
  "managedDeviceId": "Managed Device Id value",
  "displayName": "Display Name value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00"
}
```

### <a name="response"></a><span data-ttu-id="65fe2-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="65fe2-150">Response</span></span>
<span data-ttu-id="65fe2-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="65fe2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





