---
title: Atualizar deviceConfigurationDeviceStateSummary
description: Atualizar as propriedades de um objeto deviceConfigurationDeviceStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 25415ec95c43cd9cd6053e2029f585127773b02d
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760626"
---
# <a name="update-deviceconfigurationdevicestatesummary"></a><span data-ttu-id="a8b44-103">Atualizar deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="a8b44-103">Update deviceConfigurationDeviceStateSummary</span></span>

<span data-ttu-id="a8b44-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a8b44-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a8b44-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a8b44-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8b44-106">Atualizar as propriedades de um objeto [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="a8b44-106">Update the properties of a [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a8b44-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a8b44-107">Prerequisites</span></span>
<span data-ttu-id="a8b44-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8b44-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8b44-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a8b44-110">Permission type</span></span>|<span data-ttu-id="a8b44-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a8b44-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a8b44-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a8b44-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a8b44-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8b44-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a8b44-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a8b44-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a8b44-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a8b44-115">Not supported.</span></span>|
|<span data-ttu-id="a8b44-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a8b44-116">Application</span></span>|<span data-ttu-id="a8b44-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8b44-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a8b44-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a8b44-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationDeviceStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="a8b44-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a8b44-119">Request headers</span></span>
|<span data-ttu-id="a8b44-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a8b44-120">Header</span></span>|<span data-ttu-id="a8b44-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a8b44-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a8b44-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a8b44-122">Authorization</span></span>|<span data-ttu-id="a8b44-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a8b44-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a8b44-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a8b44-124">Accept</span></span>|<span data-ttu-id="a8b44-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a8b44-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8b44-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a8b44-126">Request body</span></span>
<span data-ttu-id="a8b44-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="a8b44-127">In the request body, supply a JSON representation for the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

<span data-ttu-id="a8b44-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="a8b44-128">The following table shows the properties that are required when you create the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span></span>

|<span data-ttu-id="a8b44-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a8b44-129">Property</span></span>|<span data-ttu-id="a8b44-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a8b44-130">Type</span></span>|<span data-ttu-id="a8b44-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8b44-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8b44-132">id</span><span class="sxs-lookup"><span data-stu-id="a8b44-132">id</span></span>|<span data-ttu-id="a8b44-133">String</span><span class="sxs-lookup"><span data-stu-id="a8b44-133">String</span></span>|<span data-ttu-id="a8b44-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a8b44-134">Key of the entity.</span></span>|
|<span data-ttu-id="a8b44-135">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a8b44-135">unknownDeviceCount</span></span>|<span data-ttu-id="a8b44-136">Int32</span><span class="sxs-lookup"><span data-stu-id="a8b44-136">Int32</span></span>|<span data-ttu-id="a8b44-137">Número de dispositivos desconhecidos</span><span class="sxs-lookup"><span data-stu-id="a8b44-137">Number of unknown devices</span></span>|
|<span data-ttu-id="a8b44-138">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a8b44-138">notApplicableDeviceCount</span></span>|<span data-ttu-id="a8b44-139">Int32</span><span class="sxs-lookup"><span data-stu-id="a8b44-139">Int32</span></span>|<span data-ttu-id="a8b44-140">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="a8b44-140">Number of not applicable devices</span></span>|
|<span data-ttu-id="a8b44-141">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a8b44-141">compliantDeviceCount</span></span>|<span data-ttu-id="a8b44-142">Int32</span><span class="sxs-lookup"><span data-stu-id="a8b44-142">Int32</span></span>|<span data-ttu-id="a8b44-143">Número de dispositivos em conformidade</span><span class="sxs-lookup"><span data-stu-id="a8b44-143">Number of compliant devices</span></span>|
|<span data-ttu-id="a8b44-144">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a8b44-144">remediatedDeviceCount</span></span>|<span data-ttu-id="a8b44-145">Int32</span><span class="sxs-lookup"><span data-stu-id="a8b44-145">Int32</span></span>|<span data-ttu-id="a8b44-146">Número de dispositivos corrigidos</span><span class="sxs-lookup"><span data-stu-id="a8b44-146">Number of remediated devices</span></span>|
|<span data-ttu-id="a8b44-147">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a8b44-147">nonCompliantDeviceCount</span></span>|<span data-ttu-id="a8b44-148">Int32</span><span class="sxs-lookup"><span data-stu-id="a8b44-148">Int32</span></span>|<span data-ttu-id="a8b44-149">Número de dispositivos sem conformidade</span><span class="sxs-lookup"><span data-stu-id="a8b44-149">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="a8b44-150">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a8b44-150">errorDeviceCount</span></span>|<span data-ttu-id="a8b44-151">Int32</span><span class="sxs-lookup"><span data-stu-id="a8b44-151">Int32</span></span>|<span data-ttu-id="a8b44-152">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="a8b44-152">Number of error devices</span></span>|
|<span data-ttu-id="a8b44-153">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a8b44-153">conflictDeviceCount</span></span>|<span data-ttu-id="a8b44-154">Int32</span><span class="sxs-lookup"><span data-stu-id="a8b44-154">Int32</span></span>|<span data-ttu-id="a8b44-155">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="a8b44-155">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="a8b44-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8b44-156">Response</span></span>
<span data-ttu-id="a8b44-157">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a8b44-157">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8b44-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a8b44-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="a8b44-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a8b44-159">Request</span></span>
<span data-ttu-id="a8b44-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a8b44-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a8b44-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8b44-161">Response</span></span>
<span data-ttu-id="a8b44-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a8b44-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




