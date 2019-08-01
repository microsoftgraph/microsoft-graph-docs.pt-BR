---
title: Atualizar deviceConfigurationDeviceStateSummary
description: Atualizar as propriedades de um objeto deviceConfigurationDeviceStateSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: add8609cf9ce7a8f791e350626a3accee8d74b5b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36017515"
---
# <a name="update-deviceconfigurationdevicestatesummary"></a><span data-ttu-id="678d5-103">Atualizar deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="678d5-103">Update deviceConfigurationDeviceStateSummary</span></span>

> <span data-ttu-id="678d5-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="678d5-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="678d5-105">Atualizar as propriedades de um objeto [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="678d5-105">Update the properties of a [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="678d5-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="678d5-106">Prerequisites</span></span>
<span data-ttu-id="678d5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="678d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="678d5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="678d5-109">Permission type</span></span>|<span data-ttu-id="678d5-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="678d5-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="678d5-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="678d5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="678d5-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="678d5-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="678d5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="678d5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="678d5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="678d5-114">Not supported.</span></span>|
|<span data-ttu-id="678d5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="678d5-115">Application</span></span>|<span data-ttu-id="678d5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="678d5-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="678d5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="678d5-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationDeviceStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="678d5-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="678d5-118">Request headers</span></span>
|<span data-ttu-id="678d5-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="678d5-119">Header</span></span>|<span data-ttu-id="678d5-120">Valor</span><span class="sxs-lookup"><span data-stu-id="678d5-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="678d5-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="678d5-121">Authorization</span></span>|<span data-ttu-id="678d5-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="678d5-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="678d5-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="678d5-123">Accept</span></span>|<span data-ttu-id="678d5-124">application/json</span><span class="sxs-lookup"><span data-stu-id="678d5-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="678d5-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="678d5-125">Request body</span></span>
<span data-ttu-id="678d5-126">No corpo da solicitação, forneça uma representação JSON do objeto [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="678d5-126">In the request body, supply a JSON representation for the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

<span data-ttu-id="678d5-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="678d5-127">The following table shows the properties that are required when you create the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span></span>

|<span data-ttu-id="678d5-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="678d5-128">Property</span></span>|<span data-ttu-id="678d5-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="678d5-129">Type</span></span>|<span data-ttu-id="678d5-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="678d5-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="678d5-131">id</span><span class="sxs-lookup"><span data-stu-id="678d5-131">id</span></span>|<span data-ttu-id="678d5-132">String</span><span class="sxs-lookup"><span data-stu-id="678d5-132">String</span></span>|<span data-ttu-id="678d5-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="678d5-133">Key of the entity.</span></span>|
|<span data-ttu-id="678d5-134">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="678d5-134">unknownDeviceCount</span></span>|<span data-ttu-id="678d5-135">Int32</span><span class="sxs-lookup"><span data-stu-id="678d5-135">Int32</span></span>|<span data-ttu-id="678d5-136">Número de dispositivos desconhecidos</span><span class="sxs-lookup"><span data-stu-id="678d5-136">Number of unknown devices</span></span>|
|<span data-ttu-id="678d5-137">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="678d5-137">notApplicableDeviceCount</span></span>|<span data-ttu-id="678d5-138">Int32</span><span class="sxs-lookup"><span data-stu-id="678d5-138">Int32</span></span>|<span data-ttu-id="678d5-139">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="678d5-139">Number of not applicable devices</span></span>|
|<span data-ttu-id="678d5-140">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="678d5-140">compliantDeviceCount</span></span>|<span data-ttu-id="678d5-141">Int32</span><span class="sxs-lookup"><span data-stu-id="678d5-141">Int32</span></span>|<span data-ttu-id="678d5-142">Número de dispositivos em conformidade</span><span class="sxs-lookup"><span data-stu-id="678d5-142">Number of compliant devices</span></span>|
|<span data-ttu-id="678d5-143">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="678d5-143">remediatedDeviceCount</span></span>|<span data-ttu-id="678d5-144">Int32</span><span class="sxs-lookup"><span data-stu-id="678d5-144">Int32</span></span>|<span data-ttu-id="678d5-145">Número de dispositivos corrigidos</span><span class="sxs-lookup"><span data-stu-id="678d5-145">Number of remediated devices</span></span>|
|<span data-ttu-id="678d5-146">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="678d5-146">nonCompliantDeviceCount</span></span>|<span data-ttu-id="678d5-147">Int32</span><span class="sxs-lookup"><span data-stu-id="678d5-147">Int32</span></span>|<span data-ttu-id="678d5-148">Número de dispositivos sem conformidade</span><span class="sxs-lookup"><span data-stu-id="678d5-148">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="678d5-149">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="678d5-149">errorDeviceCount</span></span>|<span data-ttu-id="678d5-150">Int32</span><span class="sxs-lookup"><span data-stu-id="678d5-150">Int32</span></span>|<span data-ttu-id="678d5-151">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="678d5-151">Number of error devices</span></span>|
|<span data-ttu-id="678d5-152">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="678d5-152">conflictDeviceCount</span></span>|<span data-ttu-id="678d5-153">Int32</span><span class="sxs-lookup"><span data-stu-id="678d5-153">Int32</span></span>|<span data-ttu-id="678d5-154">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="678d5-154">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="678d5-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="678d5-155">Response</span></span>
<span data-ttu-id="678d5-156">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="678d5-156">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="678d5-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="678d5-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="678d5-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="678d5-158">Request</span></span>
<span data-ttu-id="678d5-159">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="678d5-159">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurationDeviceStateSummaries
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

### <a name="response"></a><span data-ttu-id="678d5-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="678d5-160">Response</span></span>
<span data-ttu-id="678d5-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="678d5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



