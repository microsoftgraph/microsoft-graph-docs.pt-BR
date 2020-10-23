---
title: Atualizar deviceConfigurationDeviceStateSummary
description: Atualizar as propriedades de um objeto deviceConfigurationDeviceStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bcadb2b004f04067adf3655b5b69c2ed2bf0d68f
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728813"
---
# <a name="update-deviceconfigurationdevicestatesummary"></a><span data-ttu-id="9fbac-103">Atualizar deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="9fbac-103">Update deviceConfigurationDeviceStateSummary</span></span>

<span data-ttu-id="9fbac-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9fbac-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9fbac-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9fbac-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9fbac-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9fbac-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9fbac-107">Atualizar as propriedades de um objeto [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="9fbac-107">Update the properties of a [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9fbac-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9fbac-108">Prerequisites</span></span>
<span data-ttu-id="9fbac-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9fbac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9fbac-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9fbac-111">Permission type</span></span>|<span data-ttu-id="9fbac-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9fbac-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9fbac-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9fbac-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9fbac-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9fbac-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9fbac-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9fbac-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9fbac-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9fbac-116">Not supported.</span></span>|
|<span data-ttu-id="9fbac-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9fbac-117">Application</span></span>|<span data-ttu-id="9fbac-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9fbac-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9fbac-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9fbac-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationDeviceStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="9fbac-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9fbac-120">Request headers</span></span>
|<span data-ttu-id="9fbac-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9fbac-121">Header</span></span>|<span data-ttu-id="9fbac-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9fbac-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9fbac-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9fbac-123">Authorization</span></span>|<span data-ttu-id="9fbac-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9fbac-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9fbac-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9fbac-125">Accept</span></span>|<span data-ttu-id="9fbac-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9fbac-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9fbac-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9fbac-127">Request body</span></span>
<span data-ttu-id="9fbac-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="9fbac-128">In the request body, supply a JSON representation for the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

<span data-ttu-id="9fbac-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="9fbac-129">The following table shows the properties that are required when you create the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span></span>

|<span data-ttu-id="9fbac-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9fbac-130">Property</span></span>|<span data-ttu-id="9fbac-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9fbac-131">Type</span></span>|<span data-ttu-id="9fbac-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9fbac-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9fbac-133">id</span><span class="sxs-lookup"><span data-stu-id="9fbac-133">id</span></span>|<span data-ttu-id="9fbac-134">String</span><span class="sxs-lookup"><span data-stu-id="9fbac-134">String</span></span>|<span data-ttu-id="9fbac-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9fbac-135">Key of the entity.</span></span>|
|<span data-ttu-id="9fbac-136">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9fbac-136">unknownDeviceCount</span></span>|<span data-ttu-id="9fbac-137">Int32</span><span class="sxs-lookup"><span data-stu-id="9fbac-137">Int32</span></span>|<span data-ttu-id="9fbac-138">Número de dispositivos desconhecidos</span><span class="sxs-lookup"><span data-stu-id="9fbac-138">Number of unknown devices</span></span>|
|<span data-ttu-id="9fbac-139">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9fbac-139">notApplicableDeviceCount</span></span>|<span data-ttu-id="9fbac-140">Int32</span><span class="sxs-lookup"><span data-stu-id="9fbac-140">Int32</span></span>|<span data-ttu-id="9fbac-141">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="9fbac-141">Number of not applicable devices</span></span>|
|<span data-ttu-id="9fbac-142">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9fbac-142">compliantDeviceCount</span></span>|<span data-ttu-id="9fbac-143">Int32</span><span class="sxs-lookup"><span data-stu-id="9fbac-143">Int32</span></span>|<span data-ttu-id="9fbac-144">Número de dispositivos em conformidade</span><span class="sxs-lookup"><span data-stu-id="9fbac-144">Number of compliant devices</span></span>|
|<span data-ttu-id="9fbac-145">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9fbac-145">remediatedDeviceCount</span></span>|<span data-ttu-id="9fbac-146">Int32</span><span class="sxs-lookup"><span data-stu-id="9fbac-146">Int32</span></span>|<span data-ttu-id="9fbac-147">Número de dispositivos corrigidos</span><span class="sxs-lookup"><span data-stu-id="9fbac-147">Number of remediated devices</span></span>|
|<span data-ttu-id="9fbac-148">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9fbac-148">nonCompliantDeviceCount</span></span>|<span data-ttu-id="9fbac-149">Int32</span><span class="sxs-lookup"><span data-stu-id="9fbac-149">Int32</span></span>|<span data-ttu-id="9fbac-150">Número de dispositivos sem conformidade</span><span class="sxs-lookup"><span data-stu-id="9fbac-150">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="9fbac-151">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9fbac-151">errorDeviceCount</span></span>|<span data-ttu-id="9fbac-152">Int32</span><span class="sxs-lookup"><span data-stu-id="9fbac-152">Int32</span></span>|<span data-ttu-id="9fbac-153">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="9fbac-153">Number of error devices</span></span>|
|<span data-ttu-id="9fbac-154">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9fbac-154">conflictDeviceCount</span></span>|<span data-ttu-id="9fbac-155">Int32</span><span class="sxs-lookup"><span data-stu-id="9fbac-155">Int32</span></span>|<span data-ttu-id="9fbac-156">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="9fbac-156">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="9fbac-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="9fbac-157">Response</span></span>
<span data-ttu-id="9fbac-158">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9fbac-158">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9fbac-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9fbac-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="9fbac-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9fbac-160">Request</span></span>
<span data-ttu-id="9fbac-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9fbac-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9fbac-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="9fbac-162">Response</span></span>
<span data-ttu-id="9fbac-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9fbac-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





