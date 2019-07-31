---
title: Atualizar deviceComplianceUserOverview
description: Atualizar as propriedades de um objeto deviceComplianceUserOverview.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a7b7ea835fb373c9a650807ca5e456e7b5030fd6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35949514"
---
# <a name="update-devicecomplianceuseroverview"></a><span data-ttu-id="cd589-103">Atualizar deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="cd589-103">Update deviceComplianceUserOverview</span></span>

> <span data-ttu-id="cd589-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cd589-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cd589-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cd589-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cd589-106">Atualizar as propriedades de um objeto [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="cd589-106">Update the properties of a [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cd589-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cd589-107">Prerequisites</span></span>
<span data-ttu-id="cd589-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd589-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd589-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cd589-110">Permission type</span></span>|<span data-ttu-id="cd589-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cd589-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cd589-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cd589-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cd589-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd589-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cd589-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cd589-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cd589-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cd589-115">Not supported.</span></span>|
|<span data-ttu-id="cd589-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cd589-116">Application</span></span>|<span data-ttu-id="cd589-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cd589-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cd589-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cd589-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="cd589-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cd589-119">Request headers</span></span>
|<span data-ttu-id="cd589-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cd589-120">Header</span></span>|<span data-ttu-id="cd589-121">Valor</span><span class="sxs-lookup"><span data-stu-id="cd589-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cd589-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="cd589-122">Authorization</span></span>|<span data-ttu-id="cd589-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cd589-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cd589-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cd589-124">Accept</span></span>|<span data-ttu-id="cd589-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cd589-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd589-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cd589-126">Request body</span></span>
<span data-ttu-id="cd589-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="cd589-127">In the request body, supply a JSON representation for the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>

<span data-ttu-id="cd589-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="cd589-128">The following table shows the properties that are required when you create the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md).</span></span>

|<span data-ttu-id="cd589-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cd589-129">Property</span></span>|<span data-ttu-id="cd589-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="cd589-130">Type</span></span>|<span data-ttu-id="cd589-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="cd589-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd589-132">id</span><span class="sxs-lookup"><span data-stu-id="cd589-132">id</span></span>|<span data-ttu-id="cd589-133">String</span><span class="sxs-lookup"><span data-stu-id="cd589-133">String</span></span>|<span data-ttu-id="cd589-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="cd589-134">Key of the entity.</span></span>|
|<span data-ttu-id="cd589-135">pendingCount</span><span class="sxs-lookup"><span data-stu-id="cd589-135">pendingCount</span></span>|<span data-ttu-id="cd589-136">Int32</span><span class="sxs-lookup"><span data-stu-id="cd589-136">Int32</span></span>|<span data-ttu-id="cd589-137">Número de usuários pendentes</span><span class="sxs-lookup"><span data-stu-id="cd589-137">Number of pending Users</span></span>|
|<span data-ttu-id="cd589-138">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="cd589-138">notApplicableCount</span></span>|<span data-ttu-id="cd589-139">Int32</span><span class="sxs-lookup"><span data-stu-id="cd589-139">Int32</span></span>|<span data-ttu-id="cd589-140">Número de usuários não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="cd589-140">Number of not applicable users</span></span>|
|<span data-ttu-id="cd589-141">successCount</span><span class="sxs-lookup"><span data-stu-id="cd589-141">successCount</span></span>|<span data-ttu-id="cd589-142">Int32</span><span class="sxs-lookup"><span data-stu-id="cd589-142">Int32</span></span>|<span data-ttu-id="cd589-143">Número de usuários bem-sucedidos</span><span class="sxs-lookup"><span data-stu-id="cd589-143">Number of succeeded Users</span></span>|
|<span data-ttu-id="cd589-144">errorCount</span><span class="sxs-lookup"><span data-stu-id="cd589-144">errorCount</span></span>|<span data-ttu-id="cd589-145">Int32</span><span class="sxs-lookup"><span data-stu-id="cd589-145">Int32</span></span>|<span data-ttu-id="cd589-146">Número de usuários com erro</span><span class="sxs-lookup"><span data-stu-id="cd589-146">Number of error Users</span></span>|
|<span data-ttu-id="cd589-147">failedCount</span><span class="sxs-lookup"><span data-stu-id="cd589-147">failedCount</span></span>|<span data-ttu-id="cd589-148">Int32</span><span class="sxs-lookup"><span data-stu-id="cd589-148">Int32</span></span>|<span data-ttu-id="cd589-149">Número de usuários com falhas</span><span class="sxs-lookup"><span data-stu-id="cd589-149">Number of failed Users</span></span>|
|<span data-ttu-id="cd589-150">conflictCount</span><span class="sxs-lookup"><span data-stu-id="cd589-150">conflictCount</span></span>|<span data-ttu-id="cd589-151">Int32</span><span class="sxs-lookup"><span data-stu-id="cd589-151">Int32</span></span>|<span data-ttu-id="cd589-152">Número de usuários em conflito</span><span class="sxs-lookup"><span data-stu-id="cd589-152">Number of users in conflict</span></span>|
|<span data-ttu-id="cd589-153">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="cd589-153">lastUpdateDateTime</span></span>|<span data-ttu-id="cd589-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd589-154">DateTimeOffset</span></span>|<span data-ttu-id="cd589-155">Hora da última atualização</span><span class="sxs-lookup"><span data-stu-id="cd589-155">Last update time</span></span>|
|<span data-ttu-id="cd589-156">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="cd589-156">configurationVersion</span></span>|<span data-ttu-id="cd589-157">Int32</span><span class="sxs-lookup"><span data-stu-id="cd589-157">Int32</span></span>|<span data-ttu-id="cd589-158">Versão da política para essa visão geral</span><span class="sxs-lookup"><span data-stu-id="cd589-158">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="cd589-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="cd589-159">Response</span></span>
<span data-ttu-id="cd589-160">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cd589-160">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd589-161">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cd589-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="cd589-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cd589-162">Request</span></span>
<span data-ttu-id="cd589-163">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cd589-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cd589-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="cd589-164">Response</span></span>
<span data-ttu-id="cd589-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cd589-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





