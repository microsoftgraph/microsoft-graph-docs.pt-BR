---
title: Atualizar deviceComplianceUserOverview
description: Atualizar as propriedades de um objeto deviceComplianceUserOverview.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 379e4f534af1857c909c5e06f73f6572d143997a
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33927584"
---
# <a name="update-devicecomplianceuseroverview"></a><span data-ttu-id="809be-103">Atualizar deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="809be-103">Update deviceComplianceUserOverview</span></span>

> <span data-ttu-id="809be-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="809be-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="809be-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="809be-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="809be-106">Atualizar as propriedades de um objeto [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="809be-106">Update the properties of a [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="809be-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="809be-107">Prerequisites</span></span>
<span data-ttu-id="809be-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="809be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="809be-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="809be-110">Permission type</span></span>|<span data-ttu-id="809be-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="809be-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="809be-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="809be-112">Delegated (work or school account)</span></span>|<span data-ttu-id="809be-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="809be-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="809be-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="809be-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="809be-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="809be-115">Not supported.</span></span>|
|<span data-ttu-id="809be-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="809be-116">Application</span></span>|<span data-ttu-id="809be-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="809be-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="809be-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="809be-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="809be-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="809be-119">Request headers</span></span>
|<span data-ttu-id="809be-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="809be-120">Header</span></span>|<span data-ttu-id="809be-121">Valor</span><span class="sxs-lookup"><span data-stu-id="809be-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="809be-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="809be-122">Authorization</span></span>|<span data-ttu-id="809be-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="809be-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="809be-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="809be-124">Accept</span></span>|<span data-ttu-id="809be-125">application/json</span><span class="sxs-lookup"><span data-stu-id="809be-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="809be-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="809be-126">Request body</span></span>
<span data-ttu-id="809be-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="809be-127">In the request body, supply a JSON representation for the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>

<span data-ttu-id="809be-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="809be-128">The following table shows the properties that are required when you create the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md).</span></span>

|<span data-ttu-id="809be-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="809be-129">Property</span></span>|<span data-ttu-id="809be-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="809be-130">Type</span></span>|<span data-ttu-id="809be-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="809be-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="809be-132">id</span><span class="sxs-lookup"><span data-stu-id="809be-132">id</span></span>|<span data-ttu-id="809be-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="809be-133">String</span></span>|<span data-ttu-id="809be-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="809be-134">Key of the entity.</span></span>|
|<span data-ttu-id="809be-135">pendingCount</span><span class="sxs-lookup"><span data-stu-id="809be-135">pendingCount</span></span>|<span data-ttu-id="809be-136">Int32</span><span class="sxs-lookup"><span data-stu-id="809be-136">Int32</span></span>|<span data-ttu-id="809be-137">Número de usuários pendentes</span><span class="sxs-lookup"><span data-stu-id="809be-137">Number of pending Users</span></span>|
|<span data-ttu-id="809be-138">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="809be-138">notApplicableCount</span></span>|<span data-ttu-id="809be-139">Int32</span><span class="sxs-lookup"><span data-stu-id="809be-139">Int32</span></span>|<span data-ttu-id="809be-140">Número de usuários não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="809be-140">Number of not applicable users</span></span>|
|<span data-ttu-id="809be-141">successCount</span><span class="sxs-lookup"><span data-stu-id="809be-141">successCount</span></span>|<span data-ttu-id="809be-142">Int32</span><span class="sxs-lookup"><span data-stu-id="809be-142">Int32</span></span>|<span data-ttu-id="809be-143">Número de usuários bem-sucedidos</span><span class="sxs-lookup"><span data-stu-id="809be-143">Number of succeeded Users</span></span>|
|<span data-ttu-id="809be-144">errorCount</span><span class="sxs-lookup"><span data-stu-id="809be-144">errorCount</span></span>|<span data-ttu-id="809be-145">Int32</span><span class="sxs-lookup"><span data-stu-id="809be-145">Int32</span></span>|<span data-ttu-id="809be-146">Número de usuários com erro</span><span class="sxs-lookup"><span data-stu-id="809be-146">Number of error Users</span></span>|
|<span data-ttu-id="809be-147">failedCount</span><span class="sxs-lookup"><span data-stu-id="809be-147">failedCount</span></span>|<span data-ttu-id="809be-148">Int32</span><span class="sxs-lookup"><span data-stu-id="809be-148">Int32</span></span>|<span data-ttu-id="809be-149">Número de usuários com falhas</span><span class="sxs-lookup"><span data-stu-id="809be-149">Number of failed Users</span></span>|
|<span data-ttu-id="809be-150">conflictCount</span><span class="sxs-lookup"><span data-stu-id="809be-150">conflictCount</span></span>|<span data-ttu-id="809be-151">Int32</span><span class="sxs-lookup"><span data-stu-id="809be-151">Int32</span></span>|<span data-ttu-id="809be-152">Número de usuários em conflito</span><span class="sxs-lookup"><span data-stu-id="809be-152">Number of users in conflict</span></span>|
|<span data-ttu-id="809be-153">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="809be-153">lastUpdateDateTime</span></span>|<span data-ttu-id="809be-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="809be-154">DateTimeOffset</span></span>|<span data-ttu-id="809be-155">Hora da última atualização</span><span class="sxs-lookup"><span data-stu-id="809be-155">Last update time</span></span>|
|<span data-ttu-id="809be-156">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="809be-156">configurationVersion</span></span>|<span data-ttu-id="809be-157">Int32</span><span class="sxs-lookup"><span data-stu-id="809be-157">Int32</span></span>|<span data-ttu-id="809be-158">Versão da política para essa visão geral</span><span class="sxs-lookup"><span data-stu-id="809be-158">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="809be-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="809be-159">Response</span></span>
<span data-ttu-id="809be-160">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="809be-160">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="809be-161">Exemplo</span><span class="sxs-lookup"><span data-stu-id="809be-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="809be-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="809be-162">Request</span></span>
<span data-ttu-id="809be-163">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="809be-163">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatusOverview
Content-type: application/json
Content-length: 303

{
  "@odata.type": "#microsoft.graph.deviceComplianceUserOverview",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "conflictCount": 13,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="809be-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="809be-164">Response</span></span>
<span data-ttu-id="809be-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="809be-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 352

{
  "@odata.type": "#microsoft.graph.deviceComplianceUserOverview",
  "id": "2d4f5bf4-5bf4-2d4f-f45b-4f2df45b4f2d",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "conflictCount": 13,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```




