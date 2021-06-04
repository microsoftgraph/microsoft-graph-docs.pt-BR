---
title: Atualizar deviceComplianceUserOverview
description: Atualizar as propriedades de um objeto deviceComplianceUserOverview.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 37737ea4c193c10ed97c0a3edf1f7a906f68b861
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752711"
---
# <a name="update-devicecomplianceuseroverview"></a><span data-ttu-id="63421-103">Atualizar deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="63421-103">Update deviceComplianceUserOverview</span></span>

<span data-ttu-id="63421-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63421-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="63421-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="63421-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63421-106">Atualizar as propriedades de um objeto [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="63421-106">Update the properties of a [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="63421-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="63421-107">Prerequisites</span></span>
<span data-ttu-id="63421-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63421-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63421-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="63421-110">Permission type</span></span>|<span data-ttu-id="63421-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="63421-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="63421-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="63421-112">Delegated (work or school account)</span></span>|<span data-ttu-id="63421-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63421-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="63421-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="63421-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="63421-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="63421-115">Not supported.</span></span>|
|<span data-ttu-id="63421-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="63421-116">Application</span></span>|<span data-ttu-id="63421-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63421-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="63421-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="63421-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="63421-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="63421-119">Request headers</span></span>
|<span data-ttu-id="63421-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="63421-120">Header</span></span>|<span data-ttu-id="63421-121">Valor</span><span class="sxs-lookup"><span data-stu-id="63421-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="63421-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="63421-122">Authorization</span></span>|<span data-ttu-id="63421-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="63421-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="63421-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="63421-124">Accept</span></span>|<span data-ttu-id="63421-125">application/json</span><span class="sxs-lookup"><span data-stu-id="63421-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="63421-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="63421-126">Request body</span></span>
<span data-ttu-id="63421-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="63421-127">In the request body, supply a JSON representation for the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>

<span data-ttu-id="63421-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="63421-128">The following table shows the properties that are required when you create the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md).</span></span>

|<span data-ttu-id="63421-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="63421-129">Property</span></span>|<span data-ttu-id="63421-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="63421-130">Type</span></span>|<span data-ttu-id="63421-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="63421-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63421-132">id</span><span class="sxs-lookup"><span data-stu-id="63421-132">id</span></span>|<span data-ttu-id="63421-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="63421-133">String</span></span>|<span data-ttu-id="63421-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="63421-134">Key of the entity.</span></span>|
|<span data-ttu-id="63421-135">pendingCount</span><span class="sxs-lookup"><span data-stu-id="63421-135">pendingCount</span></span>|<span data-ttu-id="63421-136">Int32</span><span class="sxs-lookup"><span data-stu-id="63421-136">Int32</span></span>|<span data-ttu-id="63421-137">Número de usuários pendentes</span><span class="sxs-lookup"><span data-stu-id="63421-137">Number of pending Users</span></span>|
|<span data-ttu-id="63421-138">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="63421-138">notApplicableCount</span></span>|<span data-ttu-id="63421-139">Int32</span><span class="sxs-lookup"><span data-stu-id="63421-139">Int32</span></span>|<span data-ttu-id="63421-140">Número de usuários não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="63421-140">Number of not applicable users</span></span>|
|<span data-ttu-id="63421-141">successCount</span><span class="sxs-lookup"><span data-stu-id="63421-141">successCount</span></span>|<span data-ttu-id="63421-142">Int32</span><span class="sxs-lookup"><span data-stu-id="63421-142">Int32</span></span>|<span data-ttu-id="63421-143">Número de usuários bem-sucedidos</span><span class="sxs-lookup"><span data-stu-id="63421-143">Number of succeeded Users</span></span>|
|<span data-ttu-id="63421-144">errorCount</span><span class="sxs-lookup"><span data-stu-id="63421-144">errorCount</span></span>|<span data-ttu-id="63421-145">Int32</span><span class="sxs-lookup"><span data-stu-id="63421-145">Int32</span></span>|<span data-ttu-id="63421-146">Número de usuários com erro</span><span class="sxs-lookup"><span data-stu-id="63421-146">Number of error Users</span></span>|
|<span data-ttu-id="63421-147">failedCount</span><span class="sxs-lookup"><span data-stu-id="63421-147">failedCount</span></span>|<span data-ttu-id="63421-148">Int32</span><span class="sxs-lookup"><span data-stu-id="63421-148">Int32</span></span>|<span data-ttu-id="63421-149">Número de usuários com falhas</span><span class="sxs-lookup"><span data-stu-id="63421-149">Number of failed Users</span></span>|
|<span data-ttu-id="63421-150">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="63421-150">lastUpdateDateTime</span></span>|<span data-ttu-id="63421-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="63421-151">DateTimeOffset</span></span>|<span data-ttu-id="63421-152">Hora da última atualização</span><span class="sxs-lookup"><span data-stu-id="63421-152">Last update time</span></span>|
|<span data-ttu-id="63421-153">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="63421-153">configurationVersion</span></span>|<span data-ttu-id="63421-154">Int32</span><span class="sxs-lookup"><span data-stu-id="63421-154">Int32</span></span>|<span data-ttu-id="63421-155">Versão da política para essa visão geral</span><span class="sxs-lookup"><span data-stu-id="63421-155">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="63421-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="63421-156">Response</span></span>
<span data-ttu-id="63421-157">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="63421-157">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63421-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="63421-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="63421-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="63421-159">Request</span></span>
<span data-ttu-id="63421-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="63421-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="63421-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="63421-161">Response</span></span>
<span data-ttu-id="63421-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="63421-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




