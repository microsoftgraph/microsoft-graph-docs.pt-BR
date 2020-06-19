---
title: Atualizar deviceConfigurationUserOverview
description: Atualizar as propriedades de um objeto deviceConfigurationUserOverview.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a463559690d0255cd559ac7fd398b7e7406fcbaf
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792874"
---
# <a name="update-deviceconfigurationuseroverview"></a><span data-ttu-id="37e50-103">Atualizar deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="37e50-103">Update deviceConfigurationUserOverview</span></span>

<span data-ttu-id="37e50-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37e50-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="37e50-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="37e50-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="37e50-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="37e50-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37e50-107">Atualizar as propriedades de um objeto [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="37e50-107">Update the properties of a [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="37e50-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="37e50-108">Prerequisites</span></span>
<span data-ttu-id="37e50-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="37e50-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="37e50-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37e50-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37e50-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="37e50-111">Permission type</span></span>|<span data-ttu-id="37e50-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="37e50-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="37e50-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="37e50-113">Delegated (work or school account)</span></span>|<span data-ttu-id="37e50-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37e50-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="37e50-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="37e50-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="37e50-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="37e50-116">Not supported.</span></span>|
|<span data-ttu-id="37e50-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="37e50-117">Application</span></span>|<span data-ttu-id="37e50-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37e50-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="37e50-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="37e50-119">HTTP Request</span></span>
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
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/userStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/userStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/userStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/userStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerEnterpriseWiFiConfiguration/identityCertificateForClientAuthentication/userStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/userStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="37e50-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="37e50-120">Request headers</span></span>
|<span data-ttu-id="37e50-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="37e50-121">Header</span></span>|<span data-ttu-id="37e50-122">Valor</span><span class="sxs-lookup"><span data-stu-id="37e50-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="37e50-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="37e50-123">Authorization</span></span>|<span data-ttu-id="37e50-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="37e50-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="37e50-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="37e50-125">Accept</span></span>|<span data-ttu-id="37e50-126">application/json</span><span class="sxs-lookup"><span data-stu-id="37e50-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="37e50-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="37e50-127">Request body</span></span>
<span data-ttu-id="37e50-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="37e50-128">In the request body, supply a JSON representation for the [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>

<span data-ttu-id="37e50-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="37e50-129">The following table shows the properties that are required when you create the [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md).</span></span>

|<span data-ttu-id="37e50-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="37e50-130">Property</span></span>|<span data-ttu-id="37e50-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="37e50-131">Type</span></span>|<span data-ttu-id="37e50-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="37e50-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37e50-133">id</span><span class="sxs-lookup"><span data-stu-id="37e50-133">id</span></span>|<span data-ttu-id="37e50-134">String</span><span class="sxs-lookup"><span data-stu-id="37e50-134">String</span></span>|<span data-ttu-id="37e50-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="37e50-135">Key of the entity.</span></span>|
|<span data-ttu-id="37e50-136">pendingCount</span><span class="sxs-lookup"><span data-stu-id="37e50-136">pendingCount</span></span>|<span data-ttu-id="37e50-137">Int32</span><span class="sxs-lookup"><span data-stu-id="37e50-137">Int32</span></span>|<span data-ttu-id="37e50-138">Número de usuários pendentes</span><span class="sxs-lookup"><span data-stu-id="37e50-138">Number of pending Users</span></span>|
|<span data-ttu-id="37e50-139">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="37e50-139">notApplicableCount</span></span>|<span data-ttu-id="37e50-140">Int32</span><span class="sxs-lookup"><span data-stu-id="37e50-140">Int32</span></span>|<span data-ttu-id="37e50-141">Número de usuários não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="37e50-141">Number of not applicable users</span></span>|
|<span data-ttu-id="37e50-142">successCount</span><span class="sxs-lookup"><span data-stu-id="37e50-142">successCount</span></span>|<span data-ttu-id="37e50-143">Int32</span><span class="sxs-lookup"><span data-stu-id="37e50-143">Int32</span></span>|<span data-ttu-id="37e50-144">Número de usuários bem-sucedidos</span><span class="sxs-lookup"><span data-stu-id="37e50-144">Number of succeeded Users</span></span>|
|<span data-ttu-id="37e50-145">errorCount</span><span class="sxs-lookup"><span data-stu-id="37e50-145">errorCount</span></span>|<span data-ttu-id="37e50-146">Int32</span><span class="sxs-lookup"><span data-stu-id="37e50-146">Int32</span></span>|<span data-ttu-id="37e50-147">Número de usuários com erro</span><span class="sxs-lookup"><span data-stu-id="37e50-147">Number of error Users</span></span>|
|<span data-ttu-id="37e50-148">failedCount</span><span class="sxs-lookup"><span data-stu-id="37e50-148">failedCount</span></span>|<span data-ttu-id="37e50-149">Int32</span><span class="sxs-lookup"><span data-stu-id="37e50-149">Int32</span></span>|<span data-ttu-id="37e50-150">Número de usuários com falhas</span><span class="sxs-lookup"><span data-stu-id="37e50-150">Number of failed Users</span></span>|
|<span data-ttu-id="37e50-151">conflictCount</span><span class="sxs-lookup"><span data-stu-id="37e50-151">conflictCount</span></span>|<span data-ttu-id="37e50-152">Int32</span><span class="sxs-lookup"><span data-stu-id="37e50-152">Int32</span></span>|<span data-ttu-id="37e50-153">Número de usuários em conflito</span><span class="sxs-lookup"><span data-stu-id="37e50-153">Number of users in conflict</span></span>|
|<span data-ttu-id="37e50-154">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="37e50-154">lastUpdateDateTime</span></span>|<span data-ttu-id="37e50-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37e50-155">DateTimeOffset</span></span>|<span data-ttu-id="37e50-156">Hora da última atualização</span><span class="sxs-lookup"><span data-stu-id="37e50-156">Last update time</span></span>|
|<span data-ttu-id="37e50-157">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="37e50-157">configurationVersion</span></span>|<span data-ttu-id="37e50-158">Int32</span><span class="sxs-lookup"><span data-stu-id="37e50-158">Int32</span></span>|<span data-ttu-id="37e50-159">Versão da política para essa visão geral</span><span class="sxs-lookup"><span data-stu-id="37e50-159">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="37e50-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="37e50-160">Response</span></span>
<span data-ttu-id="37e50-161">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="37e50-161">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37e50-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="37e50-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="37e50-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="37e50-163">Request</span></span>
<span data-ttu-id="37e50-164">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="37e50-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="37e50-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="37e50-165">Response</span></span>
<span data-ttu-id="37e50-166">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="37e50-166">Here is an example of the response.</span></span> <span data-ttu-id="37e50-167">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="37e50-167">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="37e50-168">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="37e50-168">All of the properties will be returned from an actual call.</span></span>
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



