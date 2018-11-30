---
title: Atualizar advancedThreatProtectionOnboardingStateSummary
description: Atualize as propriedades de um objeto advancedThreatProtectionOnboardingStateSummary.
ms.openlocfilehash: e39a6086f78db393a3e75a99b475cc5db02ddb3d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039719"
---
# <a name="update-advancedthreatprotectiononboardingstatesummary"></a><span data-ttu-id="c722d-103">Atualizar advancedThreatProtectionOnboardingStateSummary</span><span class="sxs-lookup"><span data-stu-id="c722d-103">Update advancedThreatProtectionOnboardingStateSummary</span></span>

> <span data-ttu-id="c722d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c722d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c722d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c722d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c722d-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c722d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c722d-107">Atualize as propriedades de um objeto [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="c722d-107">Update the properties of a [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c722d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c722d-108">Prerequisites</span></span>
<span data-ttu-id="c722d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c722d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c722d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c722d-111">Permission type</span></span>|<span data-ttu-id="c722d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c722d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c722d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c722d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c722d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c722d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c722d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c722d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c722d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c722d-116">Not supported.</span></span>|
|<span data-ttu-id="c722d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c722d-117">Application</span></span>|<span data-ttu-id="c722d-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c722d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c722d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c722d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/advancedThreatProtectionOnboardingStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="c722d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c722d-120">Request headers</span></span>
|<span data-ttu-id="c722d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c722d-121">Header</span></span>|<span data-ttu-id="c722d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c722d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c722d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c722d-123">Authorization</span></span>|<span data-ttu-id="c722d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c722d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c722d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c722d-125">Accept</span></span>|<span data-ttu-id="c722d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c722d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c722d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c722d-127">Request body</span></span>
<span data-ttu-id="c722d-128">No corpo da solicitação, fornece uma representação JSON para o objeto [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="c722d-128">In the request body, supply a JSON representation for the [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object.</span></span>

<span data-ttu-id="c722d-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="c722d-129">The following table shows the properties that are required when you create the [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md).</span></span>

|<span data-ttu-id="c722d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c722d-130">Property</span></span>|<span data-ttu-id="c722d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c722d-131">Type</span></span>|<span data-ttu-id="c722d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c722d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c722d-133">id</span><span class="sxs-lookup"><span data-stu-id="c722d-133">id</span></span>|<span data-ttu-id="c722d-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c722d-134">String</span></span>|<span data-ttu-id="c722d-135">Identificador exclusivo</span><span class="sxs-lookup"><span data-stu-id="c722d-135">Unique Identifier</span></span>|
|<span data-ttu-id="c722d-136">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c722d-136">unknownDeviceCount</span></span>|<span data-ttu-id="c722d-137">Int32</span><span class="sxs-lookup"><span data-stu-id="c722d-137">Int32</span></span>|<span data-ttu-id="c722d-138">Número de dispositivos desconhecidos</span><span class="sxs-lookup"><span data-stu-id="c722d-138">Number of unknown devices</span></span>|
|<span data-ttu-id="c722d-139">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c722d-139">notApplicableDeviceCount</span></span>|<span data-ttu-id="c722d-140">Int32</span><span class="sxs-lookup"><span data-stu-id="c722d-140">Int32</span></span>|<span data-ttu-id="c722d-141">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="c722d-141">Number of not applicable devices</span></span>|
|<span data-ttu-id="c722d-142">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c722d-142">compliantDeviceCount</span></span>|<span data-ttu-id="c722d-143">Int32</span><span class="sxs-lookup"><span data-stu-id="c722d-143">Int32</span></span>|<span data-ttu-id="c722d-144">Número de dispositivos em conformidade</span><span class="sxs-lookup"><span data-stu-id="c722d-144">Number of compliant devices</span></span>|
|<span data-ttu-id="c722d-145">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c722d-145">remediatedDeviceCount</span></span>|<span data-ttu-id="c722d-146">Int32</span><span class="sxs-lookup"><span data-stu-id="c722d-146">Int32</span></span>|<span data-ttu-id="c722d-147">Número de dispositivos corrigidos</span><span class="sxs-lookup"><span data-stu-id="c722d-147">Number of remediated devices</span></span>|
|<span data-ttu-id="c722d-148">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c722d-148">nonCompliantDeviceCount</span></span>|<span data-ttu-id="c722d-149">Int32</span><span class="sxs-lookup"><span data-stu-id="c722d-149">Int32</span></span>|<span data-ttu-id="c722d-150">Número de dispositivos sem conformidade</span><span class="sxs-lookup"><span data-stu-id="c722d-150">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="c722d-151">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c722d-151">errorDeviceCount</span></span>|<span data-ttu-id="c722d-152">Int32</span><span class="sxs-lookup"><span data-stu-id="c722d-152">Int32</span></span>|<span data-ttu-id="c722d-153">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="c722d-153">Number of error devices</span></span>|
|<span data-ttu-id="c722d-154">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c722d-154">conflictDeviceCount</span></span>|<span data-ttu-id="c722d-155">Int32</span><span class="sxs-lookup"><span data-stu-id="c722d-155">Int32</span></span>|<span data-ttu-id="c722d-156">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="c722d-156">Number of conflict devices</span></span>|
|<span data-ttu-id="c722d-157">notAssignedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c722d-157">notAssignedDeviceCount</span></span>|<span data-ttu-id="c722d-158">Int32</span><span class="sxs-lookup"><span data-stu-id="c722d-158">Int32</span></span>|<span data-ttu-id="c722d-159">Número de dispositivos não atribuídos</span><span class="sxs-lookup"><span data-stu-id="c722d-159">Number of not assigned devices</span></span>|



## <a name="response"></a><span data-ttu-id="c722d-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="c722d-160">Response</span></span>
<span data-ttu-id="c722d-161">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c722d-161">If successful, this method returns a `200 OK` response code and an updated [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c722d-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c722d-162">Example</span></span>
### <a name="request"></a><span data-ttu-id="c722d-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c722d-163">Request</span></span>
<span data-ttu-id="c722d-164">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c722d-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/advancedThreatProtectionOnboardingStateSummary
Content-type: application/json
Content-length: 246

{
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

### <a name="response"></a><span data-ttu-id="c722d-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="c722d-165">Response</span></span>
<span data-ttu-id="c722d-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c722d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





