---
title: Atualizar deviceConfigurationUserOverview
description: Atualizar as propriedades de um objeto deviceConfigurationUserOverview.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ae2741d235fff832b9d25679739201c885f74e15
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977849"
---
# <a name="update-deviceconfigurationuseroverview"></a><span data-ttu-id="6ee74-103">Atualizar deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="6ee74-103">Update deviceConfigurationUserOverview</span></span>

> <span data-ttu-id="6ee74-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6ee74-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6ee74-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6ee74-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6ee74-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="6ee74-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6ee74-107">Atualizar as propriedades de um objeto [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="6ee74-107">Update the properties of a [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6ee74-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6ee74-108">Prerequisites</span></span>
<span data-ttu-id="6ee74-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ee74-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ee74-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6ee74-111">Permission type</span></span>|<span data-ttu-id="6ee74-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6ee74-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6ee74-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6ee74-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6ee74-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ee74-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6ee74-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6ee74-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6ee74-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6ee74-116">Not supported.</span></span>|
|<span data-ttu-id="6ee74-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6ee74-117">Application</span></span>|<span data-ttu-id="6ee74-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6ee74-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6ee74-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6ee74-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="6ee74-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6ee74-120">Request headers</span></span>
|<span data-ttu-id="6ee74-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6ee74-121">Header</span></span>|<span data-ttu-id="6ee74-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6ee74-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6ee74-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6ee74-123">Authorization</span></span>|<span data-ttu-id="6ee74-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6ee74-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6ee74-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6ee74-125">Accept</span></span>|<span data-ttu-id="6ee74-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6ee74-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ee74-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6ee74-127">Request body</span></span>
<span data-ttu-id="6ee74-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="6ee74-128">In the request body, supply a JSON representation for the [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>

<span data-ttu-id="6ee74-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="6ee74-129">The following table shows the properties that are required when you create the [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md).</span></span>

|<span data-ttu-id="6ee74-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6ee74-130">Property</span></span>|<span data-ttu-id="6ee74-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6ee74-131">Type</span></span>|<span data-ttu-id="6ee74-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6ee74-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ee74-133">id</span><span class="sxs-lookup"><span data-stu-id="6ee74-133">id</span></span>|<span data-ttu-id="6ee74-134">String</span><span class="sxs-lookup"><span data-stu-id="6ee74-134">String</span></span>|<span data-ttu-id="6ee74-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6ee74-135">Key of the entity.</span></span>|
|<span data-ttu-id="6ee74-136">pendingCount</span><span class="sxs-lookup"><span data-stu-id="6ee74-136">pendingCount</span></span>|<span data-ttu-id="6ee74-137">Int32</span><span class="sxs-lookup"><span data-stu-id="6ee74-137">Int32</span></span>|<span data-ttu-id="6ee74-138">Número de usuários pendentes</span><span class="sxs-lookup"><span data-stu-id="6ee74-138">Number of pending Users</span></span>|
|<span data-ttu-id="6ee74-139">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="6ee74-139">notApplicableCount</span></span>|<span data-ttu-id="6ee74-140">Int32</span><span class="sxs-lookup"><span data-stu-id="6ee74-140">Int32</span></span>|<span data-ttu-id="6ee74-141">Número de usuários não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="6ee74-141">Number of not applicable users</span></span>|
|<span data-ttu-id="6ee74-142">successCount</span><span class="sxs-lookup"><span data-stu-id="6ee74-142">successCount</span></span>|<span data-ttu-id="6ee74-143">Int32</span><span class="sxs-lookup"><span data-stu-id="6ee74-143">Int32</span></span>|<span data-ttu-id="6ee74-144">Número de usuários bem-sucedidos</span><span class="sxs-lookup"><span data-stu-id="6ee74-144">Number of succeeded Users</span></span>|
|<span data-ttu-id="6ee74-145">errorCount</span><span class="sxs-lookup"><span data-stu-id="6ee74-145">errorCount</span></span>|<span data-ttu-id="6ee74-146">Int32</span><span class="sxs-lookup"><span data-stu-id="6ee74-146">Int32</span></span>|<span data-ttu-id="6ee74-147">Número de usuários com erro</span><span class="sxs-lookup"><span data-stu-id="6ee74-147">Number of error Users</span></span>|
|<span data-ttu-id="6ee74-148">failedCount</span><span class="sxs-lookup"><span data-stu-id="6ee74-148">failedCount</span></span>|<span data-ttu-id="6ee74-149">Int32</span><span class="sxs-lookup"><span data-stu-id="6ee74-149">Int32</span></span>|<span data-ttu-id="6ee74-150">Número de usuários com falhas</span><span class="sxs-lookup"><span data-stu-id="6ee74-150">Number of failed Users</span></span>|
|<span data-ttu-id="6ee74-151">conflictCount</span><span class="sxs-lookup"><span data-stu-id="6ee74-151">conflictCount</span></span>|<span data-ttu-id="6ee74-152">Int32</span><span class="sxs-lookup"><span data-stu-id="6ee74-152">Int32</span></span>|<span data-ttu-id="6ee74-153">Número de usuários em conflito</span><span class="sxs-lookup"><span data-stu-id="6ee74-153">Number of users in conflict</span></span>|
|<span data-ttu-id="6ee74-154">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="6ee74-154">lastUpdateDateTime</span></span>|<span data-ttu-id="6ee74-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6ee74-155">DateTimeOffset</span></span>|<span data-ttu-id="6ee74-156">Hora da última atualização</span><span class="sxs-lookup"><span data-stu-id="6ee74-156">Last update time</span></span>|
|<span data-ttu-id="6ee74-157">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="6ee74-157">configurationVersion</span></span>|<span data-ttu-id="6ee74-158">Int32</span><span class="sxs-lookup"><span data-stu-id="6ee74-158">Int32</span></span>|<span data-ttu-id="6ee74-159">Versão da política para essa visão geral</span><span class="sxs-lookup"><span data-stu-id="6ee74-159">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="6ee74-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="6ee74-160">Response</span></span>
<span data-ttu-id="6ee74-161">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6ee74-161">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ee74-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6ee74-162">Example</span></span>
### <a name="request"></a><span data-ttu-id="6ee74-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6ee74-163">Request</span></span>
<span data-ttu-id="6ee74-164">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6ee74-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6ee74-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="6ee74-165">Response</span></span>
<span data-ttu-id="6ee74-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6ee74-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





