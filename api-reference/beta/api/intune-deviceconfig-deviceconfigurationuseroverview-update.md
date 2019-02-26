---
title: Atualizar deviceConfigurationUserOverview
description: Atualizar as propriedades de um objeto deviceConfigurationUserOverview.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0837767a7855aec4fe60bf9c3d0adfed52b4b368
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156242"
---
# <a name="update-deviceconfigurationuseroverview"></a><span data-ttu-id="6aeb8-103">Atualizar deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="6aeb8-103">Update deviceConfigurationUserOverview</span></span>

> <span data-ttu-id="6aeb8-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6aeb8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6aeb8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6aeb8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6aeb8-106">Atualizar as propriedades de um objeto [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="6aeb8-106">Update the properties of a [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6aeb8-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6aeb8-107">Prerequisites</span></span>
<span data-ttu-id="6aeb8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="6aeb8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6aeb8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6aeb8-110">Permission type</span></span>|<span data-ttu-id="6aeb8-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6aeb8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6aeb8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6aeb8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6aeb8-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6aeb8-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6aeb8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6aeb8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6aeb8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6aeb8-115">Not supported.</span></span>|
|<span data-ttu-id="6aeb8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6aeb8-116">Application</span></span>|<span data-ttu-id="6aeb8-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6aeb8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6aeb8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6aeb8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/userStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/userStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/userStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/userStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/userStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/userStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/userStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/userStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="6aeb8-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6aeb8-119">Request headers</span></span>
|<span data-ttu-id="6aeb8-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6aeb8-120">Header</span></span>|<span data-ttu-id="6aeb8-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6aeb8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6aeb8-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6aeb8-122">Authorization</span></span>|<span data-ttu-id="6aeb8-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6aeb8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6aeb8-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6aeb8-124">Accept</span></span>|<span data-ttu-id="6aeb8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6aeb8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6aeb8-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6aeb8-126">Request body</span></span>
<span data-ttu-id="6aeb8-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="6aeb8-127">In the request body, supply a JSON representation for the [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>

<span data-ttu-id="6aeb8-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="6aeb8-128">The following table shows the properties that are required when you create the [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md).</span></span>

|<span data-ttu-id="6aeb8-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6aeb8-129">Property</span></span>|<span data-ttu-id="6aeb8-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="6aeb8-130">Type</span></span>|<span data-ttu-id="6aeb8-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="6aeb8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6aeb8-132">id</span><span class="sxs-lookup"><span data-stu-id="6aeb8-132">id</span></span>|<span data-ttu-id="6aeb8-133">String</span><span class="sxs-lookup"><span data-stu-id="6aeb8-133">String</span></span>|<span data-ttu-id="6aeb8-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6aeb8-134">Key of the entity.</span></span>|
|<span data-ttu-id="6aeb8-135">pendingCount</span><span class="sxs-lookup"><span data-stu-id="6aeb8-135">pendingCount</span></span>|<span data-ttu-id="6aeb8-136">Int32</span><span class="sxs-lookup"><span data-stu-id="6aeb8-136">Int32</span></span>|<span data-ttu-id="6aeb8-137">Número de usuários pendentes</span><span class="sxs-lookup"><span data-stu-id="6aeb8-137">Number of pending Users</span></span>|
|<span data-ttu-id="6aeb8-138">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="6aeb8-138">notApplicableCount</span></span>|<span data-ttu-id="6aeb8-139">Int32</span><span class="sxs-lookup"><span data-stu-id="6aeb8-139">Int32</span></span>|<span data-ttu-id="6aeb8-140">Número de usuários não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="6aeb8-140">Number of not applicable users</span></span>|
|<span data-ttu-id="6aeb8-141">successCount</span><span class="sxs-lookup"><span data-stu-id="6aeb8-141">successCount</span></span>|<span data-ttu-id="6aeb8-142">Int32</span><span class="sxs-lookup"><span data-stu-id="6aeb8-142">Int32</span></span>|<span data-ttu-id="6aeb8-143">Número de usuários bem-sucedidos</span><span class="sxs-lookup"><span data-stu-id="6aeb8-143">Number of succeeded Users</span></span>|
|<span data-ttu-id="6aeb8-144">errorCount</span><span class="sxs-lookup"><span data-stu-id="6aeb8-144">errorCount</span></span>|<span data-ttu-id="6aeb8-145">Int32</span><span class="sxs-lookup"><span data-stu-id="6aeb8-145">Int32</span></span>|<span data-ttu-id="6aeb8-146">Número de usuários com erro</span><span class="sxs-lookup"><span data-stu-id="6aeb8-146">Number of error Users</span></span>|
|<span data-ttu-id="6aeb8-147">failedCount</span><span class="sxs-lookup"><span data-stu-id="6aeb8-147">failedCount</span></span>|<span data-ttu-id="6aeb8-148">Int32</span><span class="sxs-lookup"><span data-stu-id="6aeb8-148">Int32</span></span>|<span data-ttu-id="6aeb8-149">Número de usuários com falhas</span><span class="sxs-lookup"><span data-stu-id="6aeb8-149">Number of failed Users</span></span>|
|<span data-ttu-id="6aeb8-150">conflictCount</span><span class="sxs-lookup"><span data-stu-id="6aeb8-150">conflictCount</span></span>|<span data-ttu-id="6aeb8-151">Int32</span><span class="sxs-lookup"><span data-stu-id="6aeb8-151">Int32</span></span>|<span data-ttu-id="6aeb8-152">Número de usuários em conflito</span><span class="sxs-lookup"><span data-stu-id="6aeb8-152">Number of users in conflict</span></span>|
|<span data-ttu-id="6aeb8-153">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="6aeb8-153">lastUpdateDateTime</span></span>|<span data-ttu-id="6aeb8-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6aeb8-154">DateTimeOffset</span></span>|<span data-ttu-id="6aeb8-155">Hora da última atualização</span><span class="sxs-lookup"><span data-stu-id="6aeb8-155">Last update time</span></span>|
|<span data-ttu-id="6aeb8-156">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="6aeb8-156">configurationVersion</span></span>|<span data-ttu-id="6aeb8-157">Int32</span><span class="sxs-lookup"><span data-stu-id="6aeb8-157">Int32</span></span>|<span data-ttu-id="6aeb8-158">Versão da política para essa visão geral</span><span class="sxs-lookup"><span data-stu-id="6aeb8-158">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="6aeb8-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="6aeb8-159">Response</span></span>
<span data-ttu-id="6aeb8-160">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6aeb8-160">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6aeb8-161">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6aeb8-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="6aeb8-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6aeb8-162">Request</span></span>
<span data-ttu-id="6aeb8-163">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6aeb8-163">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatusOverview
Content-type: application/json
Content-length: 306

{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserOverview",
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

### <a name="response"></a><span data-ttu-id="6aeb8-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="6aeb8-164">Response</span></span>
<span data-ttu-id="6aeb8-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6aeb8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 355

{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserOverview",
  "id": "000e52d7-52d7-000e-d752-0e00d7520e00",
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




