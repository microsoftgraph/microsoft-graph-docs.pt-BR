---
title: Atualizar deviceConfigurationUserOverview
description: Atualizar as propriedades de um objeto deviceConfigurationUserOverview.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b91c8ff52a39c6810a833042f7ed5d6e78a910d6
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760619"
---
# <a name="update-deviceconfigurationuseroverview"></a><span data-ttu-id="7c429-103">Atualizar deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="7c429-103">Update deviceConfigurationUserOverview</span></span>

<span data-ttu-id="7c429-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c429-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7c429-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7c429-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c429-106">Atualizar as propriedades de um objeto [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="7c429-106">Update the properties of a [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7c429-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7c429-107">Prerequisites</span></span>
<span data-ttu-id="7c429-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c429-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c429-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7c429-110">Permission type</span></span>|<span data-ttu-id="7c429-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7c429-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c429-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7c429-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7c429-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c429-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7c429-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7c429-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c429-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7c429-115">Not supported.</span></span>|
|<span data-ttu-id="7c429-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7c429-116">Application</span></span>|<span data-ttu-id="7c429-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c429-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c429-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7c429-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="7c429-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7c429-119">Request headers</span></span>
|<span data-ttu-id="7c429-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7c429-120">Header</span></span>|<span data-ttu-id="7c429-121">Valor</span><span class="sxs-lookup"><span data-stu-id="7c429-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7c429-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7c429-122">Authorization</span></span>|<span data-ttu-id="7c429-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7c429-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7c429-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7c429-124">Accept</span></span>|<span data-ttu-id="7c429-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7c429-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c429-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7c429-126">Request body</span></span>
<span data-ttu-id="7c429-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="7c429-127">In the request body, supply a JSON representation for the [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>

<span data-ttu-id="7c429-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="7c429-128">The following table shows the properties that are required when you create the [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md).</span></span>

|<span data-ttu-id="7c429-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7c429-129">Property</span></span>|<span data-ttu-id="7c429-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="7c429-130">Type</span></span>|<span data-ttu-id="7c429-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="7c429-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c429-132">id</span><span class="sxs-lookup"><span data-stu-id="7c429-132">id</span></span>|<span data-ttu-id="7c429-133">String</span><span class="sxs-lookup"><span data-stu-id="7c429-133">String</span></span>|<span data-ttu-id="7c429-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="7c429-134">Key of the entity.</span></span>|
|<span data-ttu-id="7c429-135">pendingCount</span><span class="sxs-lookup"><span data-stu-id="7c429-135">pendingCount</span></span>|<span data-ttu-id="7c429-136">Int32</span><span class="sxs-lookup"><span data-stu-id="7c429-136">Int32</span></span>|<span data-ttu-id="7c429-137">Número de usuários pendentes</span><span class="sxs-lookup"><span data-stu-id="7c429-137">Number of pending Users</span></span>|
|<span data-ttu-id="7c429-138">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="7c429-138">notApplicableCount</span></span>|<span data-ttu-id="7c429-139">Int32</span><span class="sxs-lookup"><span data-stu-id="7c429-139">Int32</span></span>|<span data-ttu-id="7c429-140">Número de usuários não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="7c429-140">Number of not applicable users</span></span>|
|<span data-ttu-id="7c429-141">successCount</span><span class="sxs-lookup"><span data-stu-id="7c429-141">successCount</span></span>|<span data-ttu-id="7c429-142">Int32</span><span class="sxs-lookup"><span data-stu-id="7c429-142">Int32</span></span>|<span data-ttu-id="7c429-143">Número de usuários bem-sucedidos</span><span class="sxs-lookup"><span data-stu-id="7c429-143">Number of succeeded Users</span></span>|
|<span data-ttu-id="7c429-144">errorCount</span><span class="sxs-lookup"><span data-stu-id="7c429-144">errorCount</span></span>|<span data-ttu-id="7c429-145">Int32</span><span class="sxs-lookup"><span data-stu-id="7c429-145">Int32</span></span>|<span data-ttu-id="7c429-146">Número de usuários com erro</span><span class="sxs-lookup"><span data-stu-id="7c429-146">Number of error Users</span></span>|
|<span data-ttu-id="7c429-147">failedCount</span><span class="sxs-lookup"><span data-stu-id="7c429-147">failedCount</span></span>|<span data-ttu-id="7c429-148">Int32</span><span class="sxs-lookup"><span data-stu-id="7c429-148">Int32</span></span>|<span data-ttu-id="7c429-149">Número de usuários com falhas</span><span class="sxs-lookup"><span data-stu-id="7c429-149">Number of failed Users</span></span>|
|<span data-ttu-id="7c429-150">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="7c429-150">lastUpdateDateTime</span></span>|<span data-ttu-id="7c429-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c429-151">DateTimeOffset</span></span>|<span data-ttu-id="7c429-152">Hora da última atualização</span><span class="sxs-lookup"><span data-stu-id="7c429-152">Last update time</span></span>|
|<span data-ttu-id="7c429-153">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="7c429-153">configurationVersion</span></span>|<span data-ttu-id="7c429-154">Int32</span><span class="sxs-lookup"><span data-stu-id="7c429-154">Int32</span></span>|<span data-ttu-id="7c429-155">Versão da política para essa visão geral</span><span class="sxs-lookup"><span data-stu-id="7c429-155">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="7c429-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c429-156">Response</span></span>
<span data-ttu-id="7c429-157">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7c429-157">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c429-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7c429-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="7c429-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7c429-159">Request</span></span>
<span data-ttu-id="7c429-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7c429-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatusOverview
Content-type: application/json
Content-length: 282

{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserOverview",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="7c429-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c429-161">Response</span></span>
<span data-ttu-id="7c429-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7c429-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 331

{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserOverview",
  "id": "000e52d7-52d7-000e-d752-0e00d7520e00",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```




