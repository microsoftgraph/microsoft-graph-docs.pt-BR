---
title: Atualizar deviceConfigurationUserOverview
description: Atualizar as propriedades de um objeto deviceConfigurationUserOverview.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 03fc23138363f2c6840878acd59cb011b2129355
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42514729"
---
# <a name="update-deviceconfigurationuseroverview"></a><span data-ttu-id="f1553-103">Atualizar deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="f1553-103">Update deviceConfigurationUserOverview</span></span>

<span data-ttu-id="f1553-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1553-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f1553-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f1553-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1553-106">Atualizar as propriedades de um objeto [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="f1553-106">Update the properties of a [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f1553-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f1553-107">Prerequisites</span></span>
<span data-ttu-id="f1553-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1553-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1553-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f1553-110">Permission type</span></span>|<span data-ttu-id="f1553-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f1553-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1553-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f1553-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f1553-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1553-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f1553-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f1553-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1553-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1553-115">Not supported.</span></span>|
|<span data-ttu-id="f1553-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f1553-116">Application</span></span>|<span data-ttu-id="f1553-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1553-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1553-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f1553-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="f1553-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f1553-119">Request headers</span></span>
|<span data-ttu-id="f1553-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f1553-120">Header</span></span>|<span data-ttu-id="f1553-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f1553-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1553-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f1553-122">Authorization</span></span>|<span data-ttu-id="f1553-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f1553-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1553-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f1553-124">Accept</span></span>|<span data-ttu-id="f1553-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f1553-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1553-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f1553-126">Request body</span></span>
<span data-ttu-id="f1553-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="f1553-127">In the request body, supply a JSON representation for the [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>

<span data-ttu-id="f1553-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="f1553-128">The following table shows the properties that are required when you create the [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md).</span></span>

|<span data-ttu-id="f1553-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f1553-129">Property</span></span>|<span data-ttu-id="f1553-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f1553-130">Type</span></span>|<span data-ttu-id="f1553-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1553-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1553-132">id</span><span class="sxs-lookup"><span data-stu-id="f1553-132">id</span></span>|<span data-ttu-id="f1553-133">String</span><span class="sxs-lookup"><span data-stu-id="f1553-133">String</span></span>|<span data-ttu-id="f1553-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f1553-134">Key of the entity.</span></span>|
|<span data-ttu-id="f1553-135">pendingCount</span><span class="sxs-lookup"><span data-stu-id="f1553-135">pendingCount</span></span>|<span data-ttu-id="f1553-136">Int32</span><span class="sxs-lookup"><span data-stu-id="f1553-136">Int32</span></span>|<span data-ttu-id="f1553-137">Número de usuários pendentes</span><span class="sxs-lookup"><span data-stu-id="f1553-137">Number of pending Users</span></span>|
|<span data-ttu-id="f1553-138">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="f1553-138">notApplicableCount</span></span>|<span data-ttu-id="f1553-139">Int32</span><span class="sxs-lookup"><span data-stu-id="f1553-139">Int32</span></span>|<span data-ttu-id="f1553-140">Número de usuários não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="f1553-140">Number of not applicable users</span></span>|
|<span data-ttu-id="f1553-141">successCount</span><span class="sxs-lookup"><span data-stu-id="f1553-141">successCount</span></span>|<span data-ttu-id="f1553-142">Int32</span><span class="sxs-lookup"><span data-stu-id="f1553-142">Int32</span></span>|<span data-ttu-id="f1553-143">Número de usuários bem-sucedidos</span><span class="sxs-lookup"><span data-stu-id="f1553-143">Number of succeeded Users</span></span>|
|<span data-ttu-id="f1553-144">errorCount</span><span class="sxs-lookup"><span data-stu-id="f1553-144">errorCount</span></span>|<span data-ttu-id="f1553-145">Int32</span><span class="sxs-lookup"><span data-stu-id="f1553-145">Int32</span></span>|<span data-ttu-id="f1553-146">Número de usuários com erro</span><span class="sxs-lookup"><span data-stu-id="f1553-146">Number of error Users</span></span>|
|<span data-ttu-id="f1553-147">failedCount</span><span class="sxs-lookup"><span data-stu-id="f1553-147">failedCount</span></span>|<span data-ttu-id="f1553-148">Int32</span><span class="sxs-lookup"><span data-stu-id="f1553-148">Int32</span></span>|<span data-ttu-id="f1553-149">Número de usuários com falhas</span><span class="sxs-lookup"><span data-stu-id="f1553-149">Number of failed Users</span></span>|
|<span data-ttu-id="f1553-150">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="f1553-150">lastUpdateDateTime</span></span>|<span data-ttu-id="f1553-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1553-151">DateTimeOffset</span></span>|<span data-ttu-id="f1553-152">Hora da última atualização</span><span class="sxs-lookup"><span data-stu-id="f1553-152">Last update time</span></span>|
|<span data-ttu-id="f1553-153">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="f1553-153">configurationVersion</span></span>|<span data-ttu-id="f1553-154">Int32</span><span class="sxs-lookup"><span data-stu-id="f1553-154">Int32</span></span>|<span data-ttu-id="f1553-155">Versão da política para essa visão geral</span><span class="sxs-lookup"><span data-stu-id="f1553-155">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="f1553-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1553-156">Response</span></span>
<span data-ttu-id="f1553-157">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f1553-157">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1553-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f1553-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="f1553-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f1553-159">Request</span></span>
<span data-ttu-id="f1553-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f1553-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f1553-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1553-161">Response</span></span>
<span data-ttu-id="f1553-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f1553-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




