---
title: Atualizar vulnerableManagedDevice
description: Atualize as propriedades de um objeto vulnerableManagedDevice.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5f054105fcbea0c4d6c9d5ae0411341702d46520
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51158742"
---
# <a name="update-vulnerablemanageddevice"></a><span data-ttu-id="94319-103">Atualizar vulnerableManagedDevice</span><span class="sxs-lookup"><span data-stu-id="94319-103">Update vulnerableManagedDevice</span></span>

<span data-ttu-id="94319-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94319-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="94319-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="94319-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="94319-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="94319-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="94319-107">Atualize as propriedades de [um objeto vulnerableManagedDevice.](../resources/intune-partnerintegration-vulnerablemanageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="94319-107">Update the properties of a [vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="94319-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="94319-108">Prerequisites</span></span>
<span data-ttu-id="94319-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94319-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94319-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="94319-111">Permission type</span></span>|<span data-ttu-id="94319-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="94319-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="94319-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="94319-113">Delegated (work or school account)</span></span>|<span data-ttu-id="94319-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94319-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="94319-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="94319-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="94319-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94319-116">Not supported.</span></span>|
|<span data-ttu-id="94319-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="94319-117">Application</span></span>|<span data-ttu-id="94319-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94319-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="94319-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="94319-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH ** Entity URI for microsoft.management.services.api.vulnerableManagedDevice not found
```

## <a name="request-headers"></a><span data-ttu-id="94319-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="94319-120">Request headers</span></span>
|<span data-ttu-id="94319-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="94319-121">Header</span></span>|<span data-ttu-id="94319-122">Valor</span><span class="sxs-lookup"><span data-stu-id="94319-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="94319-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="94319-123">Authorization</span></span>|<span data-ttu-id="94319-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="94319-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="94319-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="94319-125">Accept</span></span>|<span data-ttu-id="94319-126">application/json</span><span class="sxs-lookup"><span data-stu-id="94319-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="94319-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="94319-127">Request body</span></span>
<span data-ttu-id="94319-128">No corpo da solicitação, fornece uma representação JSON para [o objeto vulnerableManagedDevice.](../resources/intune-partnerintegration-vulnerablemanageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="94319-128">In the request body, supply a JSON representation for the [vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md) object.</span></span>

<span data-ttu-id="94319-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="94319-129">The following table shows the properties that are required when you create the [vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md).</span></span>

|<span data-ttu-id="94319-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="94319-130">Property</span></span>|<span data-ttu-id="94319-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="94319-131">Type</span></span>|<span data-ttu-id="94319-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="94319-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94319-133">id</span><span class="sxs-lookup"><span data-stu-id="94319-133">id</span></span>|<span data-ttu-id="94319-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="94319-134">String</span></span>|<span data-ttu-id="94319-135">A chave de entidade e a ID do dispositivo AAD.</span><span class="sxs-lookup"><span data-stu-id="94319-135">The entity key, and AAD device ID.</span></span>|
|<span data-ttu-id="94319-136">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="94319-136">managedDeviceId</span></span>|<span data-ttu-id="94319-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="94319-137">String</span></span>|<span data-ttu-id="94319-138">A ID do dispositivo gerenciado do Intune.</span><span class="sxs-lookup"><span data-stu-id="94319-138">The Intune managed device ID.</span></span>|
|<span data-ttu-id="94319-139">displayName</span><span class="sxs-lookup"><span data-stu-id="94319-139">displayName</span></span>|<span data-ttu-id="94319-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="94319-140">String</span></span>|<span data-ttu-id="94319-141">O nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="94319-141">The device name.</span></span>|
|<span data-ttu-id="94319-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="94319-142">lastSyncDateTime</span></span>|<span data-ttu-id="94319-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94319-143">DateTimeOffset</span></span>|<span data-ttu-id="94319-144">A última data de sincronização.</span><span class="sxs-lookup"><span data-stu-id="94319-144">The last sync date.</span></span>|



## <a name="response"></a><span data-ttu-id="94319-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="94319-145">Response</span></span>
<span data-ttu-id="94319-146">Se tiver êxito, este método retornará um código de resposta e um objeto `200 OK` [vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="94319-146">If successful, this method returns a `200 OK` response code and an updated [vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94319-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="94319-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="94319-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="94319-148">Request</span></span>
<span data-ttu-id="94319-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="94319-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="94319-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="94319-150">Response</span></span>
<span data-ttu-id="94319-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="94319-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




