---
title: Criar deviceConfigurationDeviceStatus
description: Criar um novo objeto deviceConfigurationDeviceStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3093d0b2aa3318fc408eb34d6fb80515c805bd1e
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752704"
---
# <a name="create-deviceconfigurationdevicestatus"></a><span data-ttu-id="ba670-103">Criar deviceConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="ba670-103">Create deviceConfigurationDeviceStatus</span></span>

<span data-ttu-id="ba670-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba670-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ba670-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ba670-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba670-106">Criar um novo objeto [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="ba670-106">Create a new [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ba670-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ba670-107">Prerequisites</span></span>
<span data-ttu-id="ba670-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba670-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba670-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ba670-110">Permission type</span></span>|<span data-ttu-id="ba670-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ba670-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ba670-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ba670-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ba670-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba670-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ba670-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ba670-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ba670-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ba670-115">Not supported.</span></span>|
|<span data-ttu-id="ba670-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ba670-116">Application</span></span>|<span data-ttu-id="ba670-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba670-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ba670-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ba670-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="ba670-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ba670-119">Request headers</span></span>
|<span data-ttu-id="ba670-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ba670-120">Header</span></span>|<span data-ttu-id="ba670-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ba670-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ba670-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ba670-122">Authorization</span></span>|<span data-ttu-id="ba670-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ba670-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ba670-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ba670-124">Accept</span></span>|<span data-ttu-id="ba670-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ba670-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ba670-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ba670-126">Request body</span></span>
<span data-ttu-id="ba670-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceConfigurationDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="ba670-127">In the request body, supply a JSON representation for the deviceConfigurationDeviceStatus object.</span></span>

<span data-ttu-id="ba670-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceConfigurationDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="ba670-128">The following table shows the properties that are required when you create the deviceConfigurationDeviceStatus.</span></span>

|<span data-ttu-id="ba670-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ba670-129">Property</span></span>|<span data-ttu-id="ba670-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="ba670-130">Type</span></span>|<span data-ttu-id="ba670-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba670-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba670-132">id</span><span class="sxs-lookup"><span data-stu-id="ba670-132">id</span></span>|<span data-ttu-id="ba670-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ba670-133">String</span></span>|<span data-ttu-id="ba670-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ba670-134">Key of the entity.</span></span>|
|<span data-ttu-id="ba670-135">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="ba670-135">deviceDisplayName</span></span>|<span data-ttu-id="ba670-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ba670-136">String</span></span>|<span data-ttu-id="ba670-137">Nome do dispositivo de DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="ba670-137">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="ba670-138">userName</span><span class="sxs-lookup"><span data-stu-id="ba670-138">userName</span></span>|<span data-ttu-id="ba670-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ba670-139">String</span></span>|<span data-ttu-id="ba670-140">O nome de usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="ba670-140">The User Name that is being reported</span></span>|
|<span data-ttu-id="ba670-141">deviceModel</span><span class="sxs-lookup"><span data-stu-id="ba670-141">deviceModel</span></span>|<span data-ttu-id="ba670-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ba670-142">String</span></span>|<span data-ttu-id="ba670-143">O modelo do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="ba670-143">The device model that is being reported</span></span>|
|<span data-ttu-id="ba670-144">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ba670-144">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="ba670-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba670-145">DateTimeOffset</span></span>|<span data-ttu-id="ba670-146">DateTime em que o período de cortesia de conformidade do dispositivo termina</span><span class="sxs-lookup"><span data-stu-id="ba670-146">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="ba670-147">status</span><span class="sxs-lookup"><span data-stu-id="ba670-147">status</span></span>|[<span data-ttu-id="ba670-148">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="ba670-148">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="ba670-149">Status de conformidade do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="ba670-149">Compliance status of the policy report.</span></span> <span data-ttu-id="ba670-150">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="ba670-150">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="ba670-151">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="ba670-151">lastReportedDateTime</span></span>|<span data-ttu-id="ba670-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba670-152">DateTimeOffset</span></span>|<span data-ttu-id="ba670-153">Data e hora da última modificação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="ba670-153">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="ba670-154">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ba670-154">userPrincipalName</span></span>|<span data-ttu-id="ba670-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ba670-155">String</span></span>|<span data-ttu-id="ba670-156">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="ba670-156">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="ba670-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba670-157">Response</span></span>
<span data-ttu-id="ba670-158">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ba670-158">If successful, this method returns a `201 Created` response code and a [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba670-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ba670-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="ba670-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ba670-160">Request</span></span>
<span data-ttu-id="ba670-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ba670-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
Content-type: application/json
Content-length: 429

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStatus",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="ba670-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba670-162">Response</span></span>
<span data-ttu-id="ba670-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ba670-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 478

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStatus",
  "id": "674e98e5-98e5-674e-e598-4e67e5984e67",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```




