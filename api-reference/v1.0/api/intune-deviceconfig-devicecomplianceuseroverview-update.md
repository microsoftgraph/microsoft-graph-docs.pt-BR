---
title: Atualizar deviceComplianceUserOverview
description: Atualizar as propriedades de um objeto deviceComplianceUserOverview.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d173a8194457c068d038ac377d06928849101c36
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855605"
---
# <a name="update-devicecomplianceuseroverview"></a><span data-ttu-id="8cc6c-103">Atualizar deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="8cc6c-103">Update deviceComplianceUserOverview</span></span>

> <span data-ttu-id="8cc6c-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8cc6c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8cc6c-105">Atualizar as propriedades de um objeto [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="8cc6c-105">Update the properties of a [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8cc6c-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8cc6c-106">Prerequisites</span></span>
<span data-ttu-id="8cc6c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8cc6c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8cc6c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8cc6c-109">Permission type</span></span>|<span data-ttu-id="8cc6c-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8cc6c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8cc6c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8cc6c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8cc6c-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8cc6c-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8cc6c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8cc6c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8cc6c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8cc6c-114">Not supported.</span></span>|
|<span data-ttu-id="8cc6c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8cc6c-115">Application</span></span>|<span data-ttu-id="8cc6c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8cc6c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8cc6c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8cc6c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="8cc6c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8cc6c-118">Request headers</span></span>
|<span data-ttu-id="8cc6c-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8cc6c-119">Header</span></span>|<span data-ttu-id="8cc6c-120">Valor</span><span class="sxs-lookup"><span data-stu-id="8cc6c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8cc6c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="8cc6c-121">Authorization</span></span>|<span data-ttu-id="8cc6c-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8cc6c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8cc6c-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8cc6c-123">Accept</span></span>|<span data-ttu-id="8cc6c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8cc6c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8cc6c-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8cc6c-125">Request body</span></span>
<span data-ttu-id="8cc6c-126">No corpo da solicitação, forneça uma representação JSON do objeto [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="8cc6c-126">In the request body, supply a JSON representation for the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>

<span data-ttu-id="8cc6c-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="8cc6c-127">The following table shows the properties that are required when you create the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md).</span></span>

|<span data-ttu-id="8cc6c-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8cc6c-128">Property</span></span>|<span data-ttu-id="8cc6c-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="8cc6c-129">Type</span></span>|<span data-ttu-id="8cc6c-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="8cc6c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8cc6c-131">id</span><span class="sxs-lookup"><span data-stu-id="8cc6c-131">id</span></span>|<span data-ttu-id="8cc6c-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8cc6c-132">String</span></span>|<span data-ttu-id="8cc6c-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="8cc6c-133">Key of the entity.</span></span>|
|<span data-ttu-id="8cc6c-134">pendingCount</span><span class="sxs-lookup"><span data-stu-id="8cc6c-134">pendingCount</span></span>|<span data-ttu-id="8cc6c-135">Int32</span><span class="sxs-lookup"><span data-stu-id="8cc6c-135">Int32</span></span>|<span data-ttu-id="8cc6c-136">Número de usuários pendentes</span><span class="sxs-lookup"><span data-stu-id="8cc6c-136">Number of pending Users</span></span>|
|<span data-ttu-id="8cc6c-137">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="8cc6c-137">notApplicableCount</span></span>|<span data-ttu-id="8cc6c-138">Int32</span><span class="sxs-lookup"><span data-stu-id="8cc6c-138">Int32</span></span>|<span data-ttu-id="8cc6c-139">Número de usuários não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="8cc6c-139">Number of not applicable users</span></span>|
|<span data-ttu-id="8cc6c-140">successCount</span><span class="sxs-lookup"><span data-stu-id="8cc6c-140">successCount</span></span>|<span data-ttu-id="8cc6c-141">Int32</span><span class="sxs-lookup"><span data-stu-id="8cc6c-141">Int32</span></span>|<span data-ttu-id="8cc6c-142">Número de usuários bem-sucedidos</span><span class="sxs-lookup"><span data-stu-id="8cc6c-142">Number of succeeded Users</span></span>|
|<span data-ttu-id="8cc6c-143">errorCount</span><span class="sxs-lookup"><span data-stu-id="8cc6c-143">errorCount</span></span>|<span data-ttu-id="8cc6c-144">Int32</span><span class="sxs-lookup"><span data-stu-id="8cc6c-144">Int32</span></span>|<span data-ttu-id="8cc6c-145">Número de usuários com erro</span><span class="sxs-lookup"><span data-stu-id="8cc6c-145">Number of error Users</span></span>|
|<span data-ttu-id="8cc6c-146">failedCount</span><span class="sxs-lookup"><span data-stu-id="8cc6c-146">failedCount</span></span>|<span data-ttu-id="8cc6c-147">Int32</span><span class="sxs-lookup"><span data-stu-id="8cc6c-147">Int32</span></span>|<span data-ttu-id="8cc6c-148">Número de usuários com falhas</span><span class="sxs-lookup"><span data-stu-id="8cc6c-148">Number of failed Users</span></span>|
|<span data-ttu-id="8cc6c-149">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="8cc6c-149">lastUpdateDateTime</span></span>|<span data-ttu-id="8cc6c-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8cc6c-150">DateTimeOffset</span></span>|<span data-ttu-id="8cc6c-151">Hora da última atualização</span><span class="sxs-lookup"><span data-stu-id="8cc6c-151">Last update time</span></span>|
|<span data-ttu-id="8cc6c-152">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="8cc6c-152">configurationVersion</span></span>|<span data-ttu-id="8cc6c-153">Int32</span><span class="sxs-lookup"><span data-stu-id="8cc6c-153">Int32</span></span>|<span data-ttu-id="8cc6c-154">Versão da política para essa visão geral</span><span class="sxs-lookup"><span data-stu-id="8cc6c-154">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="8cc6c-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="8cc6c-155">Response</span></span>
<span data-ttu-id="8cc6c-156">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8cc6c-156">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8cc6c-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8cc6c-157">Example</span></span>
### <a name="request"></a><span data-ttu-id="8cc6c-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8cc6c-158">Request</span></span>
<span data-ttu-id="8cc6c-159">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8cc6c-159">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatusOverview
Content-type: application/json
Content-length: 279

{
  "@odata.type": "#microsoft.graph.deviceComplianceUserOverview",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="8cc6c-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="8cc6c-160">Response</span></span>
<span data-ttu-id="8cc6c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8cc6c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 328

{
  "@odata.type": "#microsoft.graph.deviceComplianceUserOverview",
  "id": "2d4f5bf4-5bf4-2d4f-f45b-4f2df45b4f2d",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```



