---
title: Atualizar deviceConfigurationUserOverview
description: Atualizar as propriedades de um objeto deviceConfigurationUserOverview.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5badee7a5a5257b06e30e9a943bd37eb7d9db107
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30958995"
---
# <a name="update-deviceconfigurationuseroverview"></a><span data-ttu-id="02dbb-103">Atualizar deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="02dbb-103">Update deviceConfigurationUserOverview</span></span>

> <span data-ttu-id="02dbb-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="02dbb-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02dbb-105">Atualizar as propriedades de um objeto [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="02dbb-105">Update the properties of a [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="02dbb-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="02dbb-106">Prerequisites</span></span>
<span data-ttu-id="02dbb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02dbb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02dbb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="02dbb-109">Permission type</span></span>|<span data-ttu-id="02dbb-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="02dbb-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="02dbb-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="02dbb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="02dbb-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02dbb-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="02dbb-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="02dbb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="02dbb-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02dbb-114">Not supported.</span></span>|
|<span data-ttu-id="02dbb-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="02dbb-115">Application</span></span>|<span data-ttu-id="02dbb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02dbb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="02dbb-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="02dbb-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="02dbb-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="02dbb-118">Request headers</span></span>
|<span data-ttu-id="02dbb-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="02dbb-119">Header</span></span>|<span data-ttu-id="02dbb-120">Valor</span><span class="sxs-lookup"><span data-stu-id="02dbb-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="02dbb-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="02dbb-121">Authorization</span></span>|<span data-ttu-id="02dbb-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="02dbb-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="02dbb-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="02dbb-123">Accept</span></span>|<span data-ttu-id="02dbb-124">application/json</span><span class="sxs-lookup"><span data-stu-id="02dbb-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="02dbb-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="02dbb-125">Request body</span></span>
<span data-ttu-id="02dbb-126">No corpo da solicitação, forneça uma representação JSON do objeto [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="02dbb-126">In the request body, supply a JSON representation for the [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>

<span data-ttu-id="02dbb-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="02dbb-127">The following table shows the properties that are required when you create the [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md).</span></span>

|<span data-ttu-id="02dbb-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="02dbb-128">Property</span></span>|<span data-ttu-id="02dbb-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="02dbb-129">Type</span></span>|<span data-ttu-id="02dbb-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="02dbb-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02dbb-131">id</span><span class="sxs-lookup"><span data-stu-id="02dbb-131">id</span></span>|<span data-ttu-id="02dbb-132">String</span><span class="sxs-lookup"><span data-stu-id="02dbb-132">String</span></span>|<span data-ttu-id="02dbb-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="02dbb-133">Key of the entity.</span></span>|
|<span data-ttu-id="02dbb-134">pendingCount</span><span class="sxs-lookup"><span data-stu-id="02dbb-134">pendingCount</span></span>|<span data-ttu-id="02dbb-135">Int32</span><span class="sxs-lookup"><span data-stu-id="02dbb-135">Int32</span></span>|<span data-ttu-id="02dbb-136">Número de usuários pendentes</span><span class="sxs-lookup"><span data-stu-id="02dbb-136">Number of pending Users</span></span>|
|<span data-ttu-id="02dbb-137">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="02dbb-137">notApplicableCount</span></span>|<span data-ttu-id="02dbb-138">Int32</span><span class="sxs-lookup"><span data-stu-id="02dbb-138">Int32</span></span>|<span data-ttu-id="02dbb-139">Número de usuários não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="02dbb-139">Number of not applicable users</span></span>|
|<span data-ttu-id="02dbb-140">successCount</span><span class="sxs-lookup"><span data-stu-id="02dbb-140">successCount</span></span>|<span data-ttu-id="02dbb-141">Int32</span><span class="sxs-lookup"><span data-stu-id="02dbb-141">Int32</span></span>|<span data-ttu-id="02dbb-142">Número de usuários bem-sucedidos</span><span class="sxs-lookup"><span data-stu-id="02dbb-142">Number of succeeded Users</span></span>|
|<span data-ttu-id="02dbb-143">errorCount</span><span class="sxs-lookup"><span data-stu-id="02dbb-143">errorCount</span></span>|<span data-ttu-id="02dbb-144">Int32</span><span class="sxs-lookup"><span data-stu-id="02dbb-144">Int32</span></span>|<span data-ttu-id="02dbb-145">Número de usuários com erro</span><span class="sxs-lookup"><span data-stu-id="02dbb-145">Number of error Users</span></span>|
|<span data-ttu-id="02dbb-146">failedCount</span><span class="sxs-lookup"><span data-stu-id="02dbb-146">failedCount</span></span>|<span data-ttu-id="02dbb-147">Int32</span><span class="sxs-lookup"><span data-stu-id="02dbb-147">Int32</span></span>|<span data-ttu-id="02dbb-148">Número de usuários com falhas</span><span class="sxs-lookup"><span data-stu-id="02dbb-148">Number of failed Users</span></span>|
|<span data-ttu-id="02dbb-149">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="02dbb-149">lastUpdateDateTime</span></span>|<span data-ttu-id="02dbb-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="02dbb-150">DateTimeOffset</span></span>|<span data-ttu-id="02dbb-151">Hora da última atualização</span><span class="sxs-lookup"><span data-stu-id="02dbb-151">Last update time</span></span>|
|<span data-ttu-id="02dbb-152">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="02dbb-152">configurationVersion</span></span>|<span data-ttu-id="02dbb-153">Int32</span><span class="sxs-lookup"><span data-stu-id="02dbb-153">Int32</span></span>|<span data-ttu-id="02dbb-154">Versão da política para essa visão geral</span><span class="sxs-lookup"><span data-stu-id="02dbb-154">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="02dbb-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="02dbb-155">Response</span></span>
<span data-ttu-id="02dbb-156">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="02dbb-156">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02dbb-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="02dbb-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="02dbb-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="02dbb-158">Request</span></span>
<span data-ttu-id="02dbb-159">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="02dbb-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="02dbb-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="02dbb-160">Response</span></span>
<span data-ttu-id="02dbb-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="02dbb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



