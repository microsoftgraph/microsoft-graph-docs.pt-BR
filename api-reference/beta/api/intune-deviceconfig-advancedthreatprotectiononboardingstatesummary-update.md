---
title: Atualizar Navegaçãoadvancedthreatprotectiononboardingstatesummary
description: Atualiza as propriedades de um objeto Navegaçãoadvancedthreatprotectiononboardingstatesummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e7031ca604c5d0a6391e68f0a4cb6c7972a2d148
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39954045"
---
# <a name="update-advancedthreatprotectiononboardingstatesummary"></a><span data-ttu-id="df2b2-103">Atualizar Navegaçãoadvancedthreatprotectiononboardingstatesummary</span><span class="sxs-lookup"><span data-stu-id="df2b2-103">Update advancedThreatProtectionOnboardingStateSummary</span></span>

> <span data-ttu-id="df2b2-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="df2b2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="df2b2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="df2b2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df2b2-106">Atualiza as propriedades de um objeto [navegaçãoadvancedthreatprotectiononboardingstatesummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="df2b2-106">Update the properties of a [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="df2b2-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="df2b2-107">Prerequisites</span></span>
<span data-ttu-id="df2b2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df2b2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df2b2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="df2b2-110">Permission type</span></span>|<span data-ttu-id="df2b2-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="df2b2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="df2b2-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="df2b2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="df2b2-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df2b2-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="df2b2-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="df2b2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="df2b2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="df2b2-115">Not supported.</span></span>|
|<span data-ttu-id="df2b2-116">Application</span><span class="sxs-lookup"><span data-stu-id="df2b2-116">Application</span></span>|<span data-ttu-id="df2b2-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df2b2-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="df2b2-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="df2b2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/advancedThreatProtectionOnboardingStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="df2b2-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="df2b2-119">Request headers</span></span>
|<span data-ttu-id="df2b2-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="df2b2-120">Header</span></span>|<span data-ttu-id="df2b2-121">Valor</span><span class="sxs-lookup"><span data-stu-id="df2b2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="df2b2-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="df2b2-122">Authorization</span></span>|<span data-ttu-id="df2b2-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="df2b2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="df2b2-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="df2b2-124">Accept</span></span>|<span data-ttu-id="df2b2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="df2b2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="df2b2-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="df2b2-126">Request body</span></span>
<span data-ttu-id="df2b2-127">No corpo da solicitação, forneça uma representação JSON do objeto [navegaçãoadvancedthreatprotectiononboardingstatesummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="df2b2-127">In the request body, supply a JSON representation for the [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object.</span></span>

<span data-ttu-id="df2b2-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [navegaçãoadvancedthreatprotectiononboardingstatesummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="df2b2-128">The following table shows the properties that are required when you create the [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md).</span></span>

|<span data-ttu-id="df2b2-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="df2b2-129">Property</span></span>|<span data-ttu-id="df2b2-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="df2b2-130">Type</span></span>|<span data-ttu-id="df2b2-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="df2b2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df2b2-132">id</span><span class="sxs-lookup"><span data-stu-id="df2b2-132">id</span></span>|<span data-ttu-id="df2b2-133">String</span><span class="sxs-lookup"><span data-stu-id="df2b2-133">String</span></span>|<span data-ttu-id="df2b2-134">Identificador exclusivo</span><span class="sxs-lookup"><span data-stu-id="df2b2-134">Unique Identifier</span></span>|
|<span data-ttu-id="df2b2-135">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="df2b2-135">unknownDeviceCount</span></span>|<span data-ttu-id="df2b2-136">Int32</span><span class="sxs-lookup"><span data-stu-id="df2b2-136">Int32</span></span>|<span data-ttu-id="df2b2-137">Número de dispositivos desconhecidos</span><span class="sxs-lookup"><span data-stu-id="df2b2-137">Number of unknown devices</span></span>|
|<span data-ttu-id="df2b2-138">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="df2b2-138">notApplicableDeviceCount</span></span>|<span data-ttu-id="df2b2-139">Int32</span><span class="sxs-lookup"><span data-stu-id="df2b2-139">Int32</span></span>|<span data-ttu-id="df2b2-140">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="df2b2-140">Number of not applicable devices</span></span>|
|<span data-ttu-id="df2b2-141">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="df2b2-141">compliantDeviceCount</span></span>|<span data-ttu-id="df2b2-142">Int32</span><span class="sxs-lookup"><span data-stu-id="df2b2-142">Int32</span></span>|<span data-ttu-id="df2b2-143">Número de dispositivos em conformidade</span><span class="sxs-lookup"><span data-stu-id="df2b2-143">Number of compliant devices</span></span>|
|<span data-ttu-id="df2b2-144">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="df2b2-144">remediatedDeviceCount</span></span>|<span data-ttu-id="df2b2-145">Int32</span><span class="sxs-lookup"><span data-stu-id="df2b2-145">Int32</span></span>|<span data-ttu-id="df2b2-146">Número de dispositivos corrigidos</span><span class="sxs-lookup"><span data-stu-id="df2b2-146">Number of remediated devices</span></span>|
|<span data-ttu-id="df2b2-147">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="df2b2-147">nonCompliantDeviceCount</span></span>|<span data-ttu-id="df2b2-148">Int32</span><span class="sxs-lookup"><span data-stu-id="df2b2-148">Int32</span></span>|<span data-ttu-id="df2b2-149">Número de dispositivos sem conformidade</span><span class="sxs-lookup"><span data-stu-id="df2b2-149">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="df2b2-150">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="df2b2-150">errorDeviceCount</span></span>|<span data-ttu-id="df2b2-151">Int32</span><span class="sxs-lookup"><span data-stu-id="df2b2-151">Int32</span></span>|<span data-ttu-id="df2b2-152">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="df2b2-152">Number of error devices</span></span>|
|<span data-ttu-id="df2b2-153">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="df2b2-153">conflictDeviceCount</span></span>|<span data-ttu-id="df2b2-154">Int32</span><span class="sxs-lookup"><span data-stu-id="df2b2-154">Int32</span></span>|<span data-ttu-id="df2b2-155">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="df2b2-155">Number of conflict devices</span></span>|
|<span data-ttu-id="df2b2-156">notAssignedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="df2b2-156">notAssignedDeviceCount</span></span>|<span data-ttu-id="df2b2-157">Int32</span><span class="sxs-lookup"><span data-stu-id="df2b2-157">Int32</span></span>|<span data-ttu-id="df2b2-158">Número de dispositivos não atribuídos</span><span class="sxs-lookup"><span data-stu-id="df2b2-158">Number of not assigned devices</span></span>|



## <a name="response"></a><span data-ttu-id="df2b2-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="df2b2-159">Response</span></span>
<span data-ttu-id="df2b2-160">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [navegaçãoadvancedthreatprotectiononboardingstatesummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="df2b2-160">If successful, this method returns a `200 OK` response code and an updated [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df2b2-161">Exemplo</span><span class="sxs-lookup"><span data-stu-id="df2b2-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="df2b2-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="df2b2-162">Request</span></span>
<span data-ttu-id="df2b2-163">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="df2b2-163">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/advancedThreatProtectionOnboardingStateSummary
Content-type: application/json
Content-length: 331

{
  "@odata.type": "#microsoft.graph.advancedThreatProtectionOnboardingStateSummary",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3,
  "notAssignedDeviceCount": 6
}
```

### <a name="response"></a><span data-ttu-id="df2b2-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="df2b2-164">Response</span></span>
<span data-ttu-id="df2b2-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="df2b2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 380

{
  "@odata.type": "#microsoft.graph.advancedThreatProtectionOnboardingStateSummary",
  "id": "74089602-9602-7408-0296-087402960874",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3,
  "notAssignedDeviceCount": 6
}
```





