---
title: Atualizar Navegaçãoadvancedthreatprotectiononboardingstatesummary
description: Atualiza as propriedades de um objeto Navegaçãoadvancedthreatprotectiononboardingstatesummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0be5ec3f75cc57c008ff53f7e0f50a6e5a79f567
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31790540"
---
# <a name="update-advancedthreatprotectiononboardingstatesummary"></a><span data-ttu-id="80595-103">Atualizar Navegaçãoadvancedthreatprotectiononboardingstatesummary</span><span class="sxs-lookup"><span data-stu-id="80595-103">Update advancedThreatProtectionOnboardingStateSummary</span></span>

> <span data-ttu-id="80595-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="80595-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="80595-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="80595-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="80595-106">Atualiza as propriedades de um objeto [navegaçãoadvancedthreatprotectiononboardingstatesummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="80595-106">Update the properties of a [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="80595-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="80595-107">Prerequisites</span></span>
<span data-ttu-id="80595-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80595-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80595-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="80595-110">Permission type</span></span>|<span data-ttu-id="80595-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="80595-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="80595-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="80595-112">Delegated (work or school account)</span></span>|<span data-ttu-id="80595-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80595-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="80595-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="80595-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="80595-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="80595-115">Not supported.</span></span>|
|<span data-ttu-id="80595-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="80595-116">Application</span></span>|<span data-ttu-id="80595-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="80595-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="80595-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="80595-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/advancedThreatProtectionOnboardingStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="80595-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="80595-119">Request headers</span></span>
|<span data-ttu-id="80595-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="80595-120">Header</span></span>|<span data-ttu-id="80595-121">Valor</span><span class="sxs-lookup"><span data-stu-id="80595-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="80595-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="80595-122">Authorization</span></span>|<span data-ttu-id="80595-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="80595-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="80595-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="80595-124">Accept</span></span>|<span data-ttu-id="80595-125">application/json</span><span class="sxs-lookup"><span data-stu-id="80595-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="80595-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="80595-126">Request body</span></span>
<span data-ttu-id="80595-127">No corpo da solicitação, forneça uma representação JSON do objeto [navegaçãoadvancedthreatprotectiononboardingstatesummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="80595-127">In the request body, supply a JSON representation for the [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object.</span></span>

<span data-ttu-id="80595-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [navegaçãoadvancedthreatprotectiononboardingstatesummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="80595-128">The following table shows the properties that are required when you create the [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md).</span></span>

|<span data-ttu-id="80595-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="80595-129">Property</span></span>|<span data-ttu-id="80595-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="80595-130">Type</span></span>|<span data-ttu-id="80595-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="80595-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80595-132">id</span><span class="sxs-lookup"><span data-stu-id="80595-132">id</span></span>|<span data-ttu-id="80595-133">String</span><span class="sxs-lookup"><span data-stu-id="80595-133">String</span></span>|<span data-ttu-id="80595-134">Identificador exclusivo</span><span class="sxs-lookup"><span data-stu-id="80595-134">Unique Identifier</span></span>|
|<span data-ttu-id="80595-135">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="80595-135">unknownDeviceCount</span></span>|<span data-ttu-id="80595-136">Int32</span><span class="sxs-lookup"><span data-stu-id="80595-136">Int32</span></span>|<span data-ttu-id="80595-137">Número de dispositivos desconhecidos</span><span class="sxs-lookup"><span data-stu-id="80595-137">Number of unknown devices</span></span>|
|<span data-ttu-id="80595-138">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="80595-138">notApplicableDeviceCount</span></span>|<span data-ttu-id="80595-139">Int32</span><span class="sxs-lookup"><span data-stu-id="80595-139">Int32</span></span>|<span data-ttu-id="80595-140">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="80595-140">Number of not applicable devices</span></span>|
|<span data-ttu-id="80595-141">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="80595-141">compliantDeviceCount</span></span>|<span data-ttu-id="80595-142">Int32</span><span class="sxs-lookup"><span data-stu-id="80595-142">Int32</span></span>|<span data-ttu-id="80595-143">Número de dispositivos em conformidade</span><span class="sxs-lookup"><span data-stu-id="80595-143">Number of compliant devices</span></span>|
|<span data-ttu-id="80595-144">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="80595-144">remediatedDeviceCount</span></span>|<span data-ttu-id="80595-145">Int32</span><span class="sxs-lookup"><span data-stu-id="80595-145">Int32</span></span>|<span data-ttu-id="80595-146">Número de dispositivos corrigidos</span><span class="sxs-lookup"><span data-stu-id="80595-146">Number of remediated devices</span></span>|
|<span data-ttu-id="80595-147">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="80595-147">nonCompliantDeviceCount</span></span>|<span data-ttu-id="80595-148">Int32</span><span class="sxs-lookup"><span data-stu-id="80595-148">Int32</span></span>|<span data-ttu-id="80595-149">Número de dispositivos sem conformidade</span><span class="sxs-lookup"><span data-stu-id="80595-149">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="80595-150">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="80595-150">errorDeviceCount</span></span>|<span data-ttu-id="80595-151">Int32</span><span class="sxs-lookup"><span data-stu-id="80595-151">Int32</span></span>|<span data-ttu-id="80595-152">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="80595-152">Number of error devices</span></span>|
|<span data-ttu-id="80595-153">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="80595-153">conflictDeviceCount</span></span>|<span data-ttu-id="80595-154">Int32</span><span class="sxs-lookup"><span data-stu-id="80595-154">Int32</span></span>|<span data-ttu-id="80595-155">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="80595-155">Number of conflict devices</span></span>|
|<span data-ttu-id="80595-156">notAssignedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="80595-156">notAssignedDeviceCount</span></span>|<span data-ttu-id="80595-157">Int32</span><span class="sxs-lookup"><span data-stu-id="80595-157">Int32</span></span>|<span data-ttu-id="80595-158">Número de dispositivos não atribuídos</span><span class="sxs-lookup"><span data-stu-id="80595-158">Number of not assigned devices</span></span>|



## <a name="response"></a><span data-ttu-id="80595-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="80595-159">Response</span></span>
<span data-ttu-id="80595-160">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [navegaçãoadvancedthreatprotectiononboardingstatesummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="80595-160">If successful, this method returns a `200 OK` response code and an updated [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80595-161">Exemplo</span><span class="sxs-lookup"><span data-stu-id="80595-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="80595-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="80595-162">Request</span></span>
<span data-ttu-id="80595-163">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="80595-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="80595-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="80595-164">Response</span></span>
<span data-ttu-id="80595-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="80595-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





