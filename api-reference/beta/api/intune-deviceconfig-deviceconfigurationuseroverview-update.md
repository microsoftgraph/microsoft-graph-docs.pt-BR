---
title: Atualizar deviceConfigurationUserOverview
description: Atualizar as propriedades de um objeto deviceConfigurationUserOverview.
ms.openlocfilehash: 44a175c11958746937fc1dd9b1b4e86940f708ce
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040400"
---
# <a name="update-deviceconfigurationuseroverview"></a><span data-ttu-id="efd81-103">Atualizar deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="efd81-103">Update deviceConfigurationUserOverview</span></span>

> <span data-ttu-id="efd81-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="efd81-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="efd81-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="efd81-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="efd81-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="efd81-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="efd81-107">Atualizar as propriedades de um objeto [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="efd81-107">Update the properties of a [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="efd81-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="efd81-108">Prerequisites</span></span>
<span data-ttu-id="efd81-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="efd81-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="efd81-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="efd81-111">Permission type</span></span>|<span data-ttu-id="efd81-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="efd81-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="efd81-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="efd81-113">Delegated (work or school account)</span></span>|<span data-ttu-id="efd81-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efd81-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="efd81-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="efd81-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="efd81-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="efd81-116">Not supported.</span></span>|
|<span data-ttu-id="efd81-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="efd81-117">Application</span></span>|<span data-ttu-id="efd81-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="efd81-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="efd81-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="efd81-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="efd81-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="efd81-120">Request headers</span></span>
|<span data-ttu-id="efd81-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="efd81-121">Header</span></span>|<span data-ttu-id="efd81-122">Valor</span><span class="sxs-lookup"><span data-stu-id="efd81-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="efd81-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="efd81-123">Authorization</span></span>|<span data-ttu-id="efd81-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="efd81-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="efd81-125">Accept</span><span class="sxs-lookup"><span data-stu-id="efd81-125">Accept</span></span>|<span data-ttu-id="efd81-126">application/json</span><span class="sxs-lookup"><span data-stu-id="efd81-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="efd81-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="efd81-127">Request body</span></span>
<span data-ttu-id="efd81-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="efd81-128">In the request body, supply a JSON representation for the [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>

<span data-ttu-id="efd81-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="efd81-129">The following table shows the properties that are required when you create the [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md).</span></span>

|<span data-ttu-id="efd81-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="efd81-130">Property</span></span>|<span data-ttu-id="efd81-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="efd81-131">Type</span></span>|<span data-ttu-id="efd81-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="efd81-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="efd81-133">id</span><span class="sxs-lookup"><span data-stu-id="efd81-133">id</span></span>|<span data-ttu-id="efd81-134">String</span><span class="sxs-lookup"><span data-stu-id="efd81-134">String</span></span>|<span data-ttu-id="efd81-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="efd81-135">Key of the entity.</span></span>|
|<span data-ttu-id="efd81-136">pendingCount</span><span class="sxs-lookup"><span data-stu-id="efd81-136">pendingCount</span></span>|<span data-ttu-id="efd81-137">Int32</span><span class="sxs-lookup"><span data-stu-id="efd81-137">Int32</span></span>|<span data-ttu-id="efd81-138">Número de usuários pendentes</span><span class="sxs-lookup"><span data-stu-id="efd81-138">Number of pending Users</span></span>|
|<span data-ttu-id="efd81-139">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="efd81-139">notApplicableCount</span></span>|<span data-ttu-id="efd81-140">Int32</span><span class="sxs-lookup"><span data-stu-id="efd81-140">Int32</span></span>|<span data-ttu-id="efd81-141">Número de usuários não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="efd81-141">Number of not applicable users</span></span>|
|<span data-ttu-id="efd81-142">successCount</span><span class="sxs-lookup"><span data-stu-id="efd81-142">successCount</span></span>|<span data-ttu-id="efd81-143">Int32</span><span class="sxs-lookup"><span data-stu-id="efd81-143">Int32</span></span>|<span data-ttu-id="efd81-144">Número de usuários bem-sucedidos</span><span class="sxs-lookup"><span data-stu-id="efd81-144">Number of succeeded Users</span></span>|
|<span data-ttu-id="efd81-145">errorCount</span><span class="sxs-lookup"><span data-stu-id="efd81-145">errorCount</span></span>|<span data-ttu-id="efd81-146">Int32</span><span class="sxs-lookup"><span data-stu-id="efd81-146">Int32</span></span>|<span data-ttu-id="efd81-147">Número de usuários com erro</span><span class="sxs-lookup"><span data-stu-id="efd81-147">Number of error Users</span></span>|
|<span data-ttu-id="efd81-148">failedCount</span><span class="sxs-lookup"><span data-stu-id="efd81-148">failedCount</span></span>|<span data-ttu-id="efd81-149">Int32</span><span class="sxs-lookup"><span data-stu-id="efd81-149">Int32</span></span>|<span data-ttu-id="efd81-150">Número de usuários com falhas</span><span class="sxs-lookup"><span data-stu-id="efd81-150">Number of failed Users</span></span>|
|<span data-ttu-id="efd81-151">conflictCount</span><span class="sxs-lookup"><span data-stu-id="efd81-151">conflictCount</span></span>|<span data-ttu-id="efd81-152">Int32</span><span class="sxs-lookup"><span data-stu-id="efd81-152">Int32</span></span>|<span data-ttu-id="efd81-153">Número de usuários em conflito</span><span class="sxs-lookup"><span data-stu-id="efd81-153">Number of users in conflict</span></span>|
|<span data-ttu-id="efd81-154">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="efd81-154">lastUpdateDateTime</span></span>|<span data-ttu-id="efd81-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="efd81-155">DateTimeOffset</span></span>|<span data-ttu-id="efd81-156">Hora da última atualização</span><span class="sxs-lookup"><span data-stu-id="efd81-156">Last update time</span></span>|
|<span data-ttu-id="efd81-157">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="efd81-157">configurationVersion</span></span>|<span data-ttu-id="efd81-158">Int32</span><span class="sxs-lookup"><span data-stu-id="efd81-158">Int32</span></span>|<span data-ttu-id="efd81-159">Versão da política para essa visão geral</span><span class="sxs-lookup"><span data-stu-id="efd81-159">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="efd81-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="efd81-160">Response</span></span>
<span data-ttu-id="efd81-161">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="efd81-161">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="efd81-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="efd81-162">Example</span></span>
### <a name="request"></a><span data-ttu-id="efd81-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="efd81-163">Request</span></span>
<span data-ttu-id="efd81-164">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="efd81-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatusOverview
Content-type: application/json
Content-length: 236

{
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

### <a name="response"></a><span data-ttu-id="efd81-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="efd81-165">Response</span></span>
<span data-ttu-id="efd81-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="efd81-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





