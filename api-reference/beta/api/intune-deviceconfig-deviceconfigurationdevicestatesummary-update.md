---
title: Atualizar deviceConfigurationDeviceStateSummary
description: Atualizar as propriedades de um objeto deviceConfigurationDeviceStateSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a386bf3ad82d66a2fe6f2babdadc667fb6abba35
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36345950"
---
# <a name="update-deviceconfigurationdevicestatesummary"></a><span data-ttu-id="acef5-103">Atualizar deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="acef5-103">Update deviceConfigurationDeviceStateSummary</span></span>

> <span data-ttu-id="acef5-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="acef5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="acef5-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="acef5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="acef5-106">Atualizar as propriedades de um objeto [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="acef5-106">Update the properties of a [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="acef5-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="acef5-107">Prerequisites</span></span>
<span data-ttu-id="acef5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="acef5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="acef5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="acef5-110">Permission type</span></span>|<span data-ttu-id="acef5-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="acef5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="acef5-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="acef5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="acef5-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="acef5-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="acef5-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="acef5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="acef5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="acef5-115">Not supported.</span></span>|
|<span data-ttu-id="acef5-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="acef5-116">Application</span></span>|<span data-ttu-id="acef5-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="acef5-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="acef5-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="acef5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationDeviceStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="acef5-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="acef5-119">Request headers</span></span>
|<span data-ttu-id="acef5-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="acef5-120">Header</span></span>|<span data-ttu-id="acef5-121">Valor</span><span class="sxs-lookup"><span data-stu-id="acef5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="acef5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="acef5-122">Authorization</span></span>|<span data-ttu-id="acef5-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="acef5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="acef5-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="acef5-124">Accept</span></span>|<span data-ttu-id="acef5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="acef5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="acef5-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="acef5-126">Request body</span></span>
<span data-ttu-id="acef5-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="acef5-127">In the request body, supply a JSON representation for the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

<span data-ttu-id="acef5-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="acef5-128">The following table shows the properties that are required when you create the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span></span>

|<span data-ttu-id="acef5-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="acef5-129">Property</span></span>|<span data-ttu-id="acef5-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="acef5-130">Type</span></span>|<span data-ttu-id="acef5-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="acef5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="acef5-132">id</span><span class="sxs-lookup"><span data-stu-id="acef5-132">id</span></span>|<span data-ttu-id="acef5-133">String</span><span class="sxs-lookup"><span data-stu-id="acef5-133">String</span></span>|<span data-ttu-id="acef5-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="acef5-134">Key of the entity.</span></span>|
|<span data-ttu-id="acef5-135">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="acef5-135">unknownDeviceCount</span></span>|<span data-ttu-id="acef5-136">Int32</span><span class="sxs-lookup"><span data-stu-id="acef5-136">Int32</span></span>|<span data-ttu-id="acef5-137">Número de dispositivos desconhecidos</span><span class="sxs-lookup"><span data-stu-id="acef5-137">Number of unknown devices</span></span>|
|<span data-ttu-id="acef5-138">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="acef5-138">notApplicableDeviceCount</span></span>|<span data-ttu-id="acef5-139">Int32</span><span class="sxs-lookup"><span data-stu-id="acef5-139">Int32</span></span>|<span data-ttu-id="acef5-140">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="acef5-140">Number of not applicable devices</span></span>|
|<span data-ttu-id="acef5-141">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="acef5-141">compliantDeviceCount</span></span>|<span data-ttu-id="acef5-142">Int32</span><span class="sxs-lookup"><span data-stu-id="acef5-142">Int32</span></span>|<span data-ttu-id="acef5-143">Número de dispositivos em conformidade</span><span class="sxs-lookup"><span data-stu-id="acef5-143">Number of compliant devices</span></span>|
|<span data-ttu-id="acef5-144">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="acef5-144">remediatedDeviceCount</span></span>|<span data-ttu-id="acef5-145">Int32</span><span class="sxs-lookup"><span data-stu-id="acef5-145">Int32</span></span>|<span data-ttu-id="acef5-146">Número de dispositivos corrigidos</span><span class="sxs-lookup"><span data-stu-id="acef5-146">Number of remediated devices</span></span>|
|<span data-ttu-id="acef5-147">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="acef5-147">nonCompliantDeviceCount</span></span>|<span data-ttu-id="acef5-148">Int32</span><span class="sxs-lookup"><span data-stu-id="acef5-148">Int32</span></span>|<span data-ttu-id="acef5-149">Número de dispositivos sem conformidade</span><span class="sxs-lookup"><span data-stu-id="acef5-149">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="acef5-150">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="acef5-150">errorDeviceCount</span></span>|<span data-ttu-id="acef5-151">Int32</span><span class="sxs-lookup"><span data-stu-id="acef5-151">Int32</span></span>|<span data-ttu-id="acef5-152">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="acef5-152">Number of error devices</span></span>|
|<span data-ttu-id="acef5-153">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="acef5-153">conflictDeviceCount</span></span>|<span data-ttu-id="acef5-154">Int32</span><span class="sxs-lookup"><span data-stu-id="acef5-154">Int32</span></span>|<span data-ttu-id="acef5-155">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="acef5-155">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="acef5-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="acef5-156">Response</span></span>
<span data-ttu-id="acef5-157">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="acef5-157">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="acef5-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="acef5-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="acef5-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="acef5-159">Request</span></span>
<span data-ttu-id="acef5-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="acef5-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationDeviceStateSummaries
Content-type: application/json
Content-length: 290

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStateSummary",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="acef5-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="acef5-161">Response</span></span>
<span data-ttu-id="acef5-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="acef5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 339

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStateSummary",
  "id": "5db26f5a-6f5a-5db2-5a6f-b25d5a6fb25d",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```






