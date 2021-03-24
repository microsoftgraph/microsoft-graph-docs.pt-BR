---
title: Atualizar deviceComplianceUserOverview
description: Atualizar as propriedades de um objeto deviceComplianceUserOverview.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f3b723c5adf2149808707d506dc5c62922c5ad8d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51128114"
---
# <a name="update-devicecomplianceuseroverview"></a><span data-ttu-id="0d0a8-103">Atualizar deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="0d0a8-103">Update deviceComplianceUserOverview</span></span>

<span data-ttu-id="0d0a8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d0a8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0d0a8-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0d0a8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0d0a8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0d0a8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0d0a8-107">Atualizar as propriedades de um objeto [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="0d0a8-107">Update the properties of a [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0d0a8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0d0a8-108">Prerequisites</span></span>
<span data-ttu-id="0d0a8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d0a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d0a8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0d0a8-111">Permission type</span></span>|<span data-ttu-id="0d0a8-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0d0a8-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0d0a8-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0d0a8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0d0a8-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d0a8-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0d0a8-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0d0a8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0d0a8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0d0a8-116">Not supported.</span></span>|
|<span data-ttu-id="0d0a8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0d0a8-117">Application</span></span>|<span data-ttu-id="0d0a8-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d0a8-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0d0a8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0d0a8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="0d0a8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0d0a8-120">Request headers</span></span>
|<span data-ttu-id="0d0a8-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0d0a8-121">Header</span></span>|<span data-ttu-id="0d0a8-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0d0a8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0d0a8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0d0a8-123">Authorization</span></span>|<span data-ttu-id="0d0a8-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0d0a8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0d0a8-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0d0a8-125">Accept</span></span>|<span data-ttu-id="0d0a8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0d0a8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0d0a8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0d0a8-127">Request body</span></span>
<span data-ttu-id="0d0a8-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="0d0a8-128">In the request body, supply a JSON representation for the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>

<span data-ttu-id="0d0a8-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="0d0a8-129">The following table shows the properties that are required when you create the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md).</span></span>

|<span data-ttu-id="0d0a8-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0d0a8-130">Property</span></span>|<span data-ttu-id="0d0a8-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0d0a8-131">Type</span></span>|<span data-ttu-id="0d0a8-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0d0a8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d0a8-133">id</span><span class="sxs-lookup"><span data-stu-id="0d0a8-133">id</span></span>|<span data-ttu-id="0d0a8-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0d0a8-134">String</span></span>|<span data-ttu-id="0d0a8-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0d0a8-135">Key of the entity.</span></span>|
|<span data-ttu-id="0d0a8-136">pendingCount</span><span class="sxs-lookup"><span data-stu-id="0d0a8-136">pendingCount</span></span>|<span data-ttu-id="0d0a8-137">Int32</span><span class="sxs-lookup"><span data-stu-id="0d0a8-137">Int32</span></span>|<span data-ttu-id="0d0a8-138">Número de usuários pendentes</span><span class="sxs-lookup"><span data-stu-id="0d0a8-138">Number of pending Users</span></span>|
|<span data-ttu-id="0d0a8-139">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="0d0a8-139">notApplicableCount</span></span>|<span data-ttu-id="0d0a8-140">Int32</span><span class="sxs-lookup"><span data-stu-id="0d0a8-140">Int32</span></span>|<span data-ttu-id="0d0a8-141">Número de usuários não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="0d0a8-141">Number of not applicable users</span></span>|
|<span data-ttu-id="0d0a8-142">successCount</span><span class="sxs-lookup"><span data-stu-id="0d0a8-142">successCount</span></span>|<span data-ttu-id="0d0a8-143">Int32</span><span class="sxs-lookup"><span data-stu-id="0d0a8-143">Int32</span></span>|<span data-ttu-id="0d0a8-144">Número de usuários bem-sucedidos</span><span class="sxs-lookup"><span data-stu-id="0d0a8-144">Number of succeeded Users</span></span>|
|<span data-ttu-id="0d0a8-145">errorCount</span><span class="sxs-lookup"><span data-stu-id="0d0a8-145">errorCount</span></span>|<span data-ttu-id="0d0a8-146">Int32</span><span class="sxs-lookup"><span data-stu-id="0d0a8-146">Int32</span></span>|<span data-ttu-id="0d0a8-147">Número de usuários com erro</span><span class="sxs-lookup"><span data-stu-id="0d0a8-147">Number of error Users</span></span>|
|<span data-ttu-id="0d0a8-148">failedCount</span><span class="sxs-lookup"><span data-stu-id="0d0a8-148">failedCount</span></span>|<span data-ttu-id="0d0a8-149">Int32</span><span class="sxs-lookup"><span data-stu-id="0d0a8-149">Int32</span></span>|<span data-ttu-id="0d0a8-150">Número de usuários com falhas</span><span class="sxs-lookup"><span data-stu-id="0d0a8-150">Number of failed Users</span></span>|
|<span data-ttu-id="0d0a8-151">conflictCount</span><span class="sxs-lookup"><span data-stu-id="0d0a8-151">conflictCount</span></span>|<span data-ttu-id="0d0a8-152">Int32</span><span class="sxs-lookup"><span data-stu-id="0d0a8-152">Int32</span></span>|<span data-ttu-id="0d0a8-153">Número de usuários em conflito</span><span class="sxs-lookup"><span data-stu-id="0d0a8-153">Number of users in conflict</span></span>|
|<span data-ttu-id="0d0a8-154">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="0d0a8-154">lastUpdateDateTime</span></span>|<span data-ttu-id="0d0a8-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d0a8-155">DateTimeOffset</span></span>|<span data-ttu-id="0d0a8-156">Hora da última atualização</span><span class="sxs-lookup"><span data-stu-id="0d0a8-156">Last update time</span></span>|
|<span data-ttu-id="0d0a8-157">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="0d0a8-157">configurationVersion</span></span>|<span data-ttu-id="0d0a8-158">Int32</span><span class="sxs-lookup"><span data-stu-id="0d0a8-158">Int32</span></span>|<span data-ttu-id="0d0a8-159">Versão da política para essa visão geral</span><span class="sxs-lookup"><span data-stu-id="0d0a8-159">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="0d0a8-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d0a8-160">Response</span></span>
<span data-ttu-id="0d0a8-161">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0d0a8-161">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d0a8-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0d0a8-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="0d0a8-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0d0a8-163">Request</span></span>
<span data-ttu-id="0d0a8-164">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0d0a8-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0d0a8-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d0a8-165">Response</span></span>
<span data-ttu-id="0d0a8-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0d0a8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




