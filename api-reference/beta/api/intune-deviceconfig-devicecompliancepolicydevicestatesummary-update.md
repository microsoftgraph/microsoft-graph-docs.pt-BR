---
title: Atualizar deviceCompliancePolicyDeviceStateSummary
description: Atualizar as propriedades de um objeto deviceCompliancePolicyDeviceStateSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2a8df64bd2b6c5976481b00eedf3212d115eba23
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27933362"
---
# <a name="update-devicecompliancepolicydevicestatesummary"></a><span data-ttu-id="8a96c-103">Atualizar deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="8a96c-103">Update deviceCompliancePolicyDeviceStateSummary</span></span>

> <span data-ttu-id="8a96c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8a96c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8a96c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8a96c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8a96c-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8a96c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8a96c-107">Atualizar as propriedades de um objeto [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="8a96c-107">Update the properties of a [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8a96c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8a96c-108">Prerequisites</span></span>
<span data-ttu-id="8a96c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a96c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a96c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8a96c-111">Permission type</span></span>|<span data-ttu-id="8a96c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8a96c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8a96c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8a96c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8a96c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a96c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8a96c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8a96c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8a96c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8a96c-116">Not supported.</span></span>|
|<span data-ttu-id="8a96c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8a96c-117">Application</span></span>|<span data-ttu-id="8a96c-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8a96c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8a96c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8a96c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicyDeviceStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="8a96c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8a96c-120">Request headers</span></span>
|<span data-ttu-id="8a96c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8a96c-121">Header</span></span>|<span data-ttu-id="8a96c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8a96c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8a96c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8a96c-123">Authorization</span></span>|<span data-ttu-id="8a96c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8a96c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8a96c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8a96c-125">Accept</span></span>|<span data-ttu-id="8a96c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8a96c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8a96c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8a96c-127">Request body</span></span>
<span data-ttu-id="8a96c-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="8a96c-128">In the request body, supply a JSON representation for the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>

<span data-ttu-id="8a96c-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="8a96c-129">The following table shows the properties that are required when you create the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span></span>

|<span data-ttu-id="8a96c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8a96c-130">Property</span></span>|<span data-ttu-id="8a96c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="8a96c-131">Type</span></span>|<span data-ttu-id="8a96c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="8a96c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a96c-133">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="8a96c-133">inGracePeriodCount</span></span>|<span data-ttu-id="8a96c-134">Int32</span><span class="sxs-lookup"><span data-stu-id="8a96c-134">Int32</span></span>|<span data-ttu-id="8a96c-135">Quantidade de dispositivos que estão no período de cortesia</span><span class="sxs-lookup"><span data-stu-id="8a96c-135">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="8a96c-136">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="8a96c-136">configManagerCount</span></span>|<span data-ttu-id="8a96c-137">Int32</span><span class="sxs-lookup"><span data-stu-id="8a96c-137">Int32</span></span>|<span data-ttu-id="8a96c-138">Quantidade de dispositivos que estão em conformidade gerenciada pelo System Center Configuration Manager</span><span class="sxs-lookup"><span data-stu-id="8a96c-138">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="8a96c-139">id</span><span class="sxs-lookup"><span data-stu-id="8a96c-139">id</span></span>|<span data-ttu-id="8a96c-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8a96c-140">String</span></span>|<span data-ttu-id="8a96c-141">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="8a96c-141">Key of the entity.</span></span>|
|<span data-ttu-id="8a96c-142">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8a96c-142">unknownDeviceCount</span></span>|<span data-ttu-id="8a96c-143">Int32</span><span class="sxs-lookup"><span data-stu-id="8a96c-143">Int32</span></span>|<span data-ttu-id="8a96c-144">Número de dispositivos desconhecidos</span><span class="sxs-lookup"><span data-stu-id="8a96c-144">Number of unknown devices</span></span>|
|<span data-ttu-id="8a96c-145">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8a96c-145">notApplicableDeviceCount</span></span>|<span data-ttu-id="8a96c-146">Int32</span><span class="sxs-lookup"><span data-stu-id="8a96c-146">Int32</span></span>|<span data-ttu-id="8a96c-147">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="8a96c-147">Number of not applicable devices</span></span>|
|<span data-ttu-id="8a96c-148">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8a96c-148">compliantDeviceCount</span></span>|<span data-ttu-id="8a96c-149">Int32</span><span class="sxs-lookup"><span data-stu-id="8a96c-149">Int32</span></span>|<span data-ttu-id="8a96c-150">Número de dispositivos em conformidade</span><span class="sxs-lookup"><span data-stu-id="8a96c-150">Number of compliant devices</span></span>|
|<span data-ttu-id="8a96c-151">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8a96c-151">remediatedDeviceCount</span></span>|<span data-ttu-id="8a96c-152">Int32</span><span class="sxs-lookup"><span data-stu-id="8a96c-152">Int32</span></span>|<span data-ttu-id="8a96c-153">Número de dispositivos corrigidos</span><span class="sxs-lookup"><span data-stu-id="8a96c-153">Number of remediated devices</span></span>|
|<span data-ttu-id="8a96c-154">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8a96c-154">nonCompliantDeviceCount</span></span>|<span data-ttu-id="8a96c-155">Int32</span><span class="sxs-lookup"><span data-stu-id="8a96c-155">Int32</span></span>|<span data-ttu-id="8a96c-156">Número de dispositivos sem conformidade</span><span class="sxs-lookup"><span data-stu-id="8a96c-156">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="8a96c-157">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8a96c-157">errorDeviceCount</span></span>|<span data-ttu-id="8a96c-158">Int32</span><span class="sxs-lookup"><span data-stu-id="8a96c-158">Int32</span></span>|<span data-ttu-id="8a96c-159">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="8a96c-159">Number of error devices</span></span>|
|<span data-ttu-id="8a96c-160">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8a96c-160">conflictDeviceCount</span></span>|<span data-ttu-id="8a96c-161">Int32</span><span class="sxs-lookup"><span data-stu-id="8a96c-161">Int32</span></span>|<span data-ttu-id="8a96c-162">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="8a96c-162">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="8a96c-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a96c-163">Response</span></span>
<span data-ttu-id="8a96c-164">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8a96c-164">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a96c-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8a96c-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="8a96c-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8a96c-166">Request</span></span>
<span data-ttu-id="8a96c-167">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8a96c-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicyDeviceStateSummary
Content-type: application/json
Content-length: 270

{
  "inGracePeriodCount": 2,
  "configManagerCount": 2,
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="8a96c-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a96c-168">Response</span></span>
<span data-ttu-id="8a96c-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8a96c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 398

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyDeviceStateSummary",
  "inGracePeriodCount": 2,
  "configManagerCount": 2,
  "id": "8c4de8a7-e8a7-8c4d-a7e8-4d8ca7e84d8c",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```





