---
title: Atualizar deviceConfigurationDeviceStatus
description: Atualizar as propriedades de um objeto deviceConfigurationDeviceStatus.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: aed2083cf5eb422067295c87ae28b2048816f76c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42514743"
---
# <a name="update-deviceconfigurationdevicestatus"></a><span data-ttu-id="11b16-103">Atualizar deviceConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="11b16-103">Update deviceConfigurationDeviceStatus</span></span>

<span data-ttu-id="11b16-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11b16-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="11b16-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="11b16-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11b16-106">Atualizar as propriedades de um objeto [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="11b16-106">Update the properties of a [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="11b16-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="11b16-107">Prerequisites</span></span>
<span data-ttu-id="11b16-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11b16-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11b16-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="11b16-110">Permission type</span></span>|<span data-ttu-id="11b16-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="11b16-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="11b16-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="11b16-112">Delegated (work or school account)</span></span>|<span data-ttu-id="11b16-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11b16-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="11b16-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="11b16-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="11b16-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="11b16-115">Not supported.</span></span>|
|<span data-ttu-id="11b16-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="11b16-116">Application</span></span>|<span data-ttu-id="11b16-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="11b16-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="11b16-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="11b16-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="11b16-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="11b16-119">Request headers</span></span>
|<span data-ttu-id="11b16-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="11b16-120">Header</span></span>|<span data-ttu-id="11b16-121">Valor</span><span class="sxs-lookup"><span data-stu-id="11b16-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="11b16-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="11b16-122">Authorization</span></span>|<span data-ttu-id="11b16-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="11b16-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="11b16-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="11b16-124">Accept</span></span>|<span data-ttu-id="11b16-125">application/json</span><span class="sxs-lookup"><span data-stu-id="11b16-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="11b16-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="11b16-126">Request body</span></span>
<span data-ttu-id="11b16-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="11b16-127">In the request body, supply a JSON representation for the [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object.</span></span>

<span data-ttu-id="11b16-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="11b16-128">The following table shows the properties that are required when you create the [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span></span>

|<span data-ttu-id="11b16-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="11b16-129">Property</span></span>|<span data-ttu-id="11b16-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="11b16-130">Type</span></span>|<span data-ttu-id="11b16-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="11b16-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11b16-132">id</span><span class="sxs-lookup"><span data-stu-id="11b16-132">id</span></span>|<span data-ttu-id="11b16-133">String</span><span class="sxs-lookup"><span data-stu-id="11b16-133">String</span></span>|<span data-ttu-id="11b16-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="11b16-134">Key of the entity.</span></span>|
|<span data-ttu-id="11b16-135">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="11b16-135">deviceDisplayName</span></span>|<span data-ttu-id="11b16-136">String</span><span class="sxs-lookup"><span data-stu-id="11b16-136">String</span></span>|<span data-ttu-id="11b16-137">Nome do dispositivo de DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="11b16-137">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="11b16-138">userName</span><span class="sxs-lookup"><span data-stu-id="11b16-138">userName</span></span>|<span data-ttu-id="11b16-139">String</span><span class="sxs-lookup"><span data-stu-id="11b16-139">String</span></span>|<span data-ttu-id="11b16-140">O nome de usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="11b16-140">The User Name that is being reported</span></span>|
|<span data-ttu-id="11b16-141">deviceModel</span><span class="sxs-lookup"><span data-stu-id="11b16-141">deviceModel</span></span>|<span data-ttu-id="11b16-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="11b16-142">String</span></span>|<span data-ttu-id="11b16-143">O modelo do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="11b16-143">The device model that is being reported</span></span>|
|<span data-ttu-id="11b16-144">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="11b16-144">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="11b16-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11b16-145">DateTimeOffset</span></span>|<span data-ttu-id="11b16-146">DateTime em que o período de cortesia de conformidade do dispositivo termina</span><span class="sxs-lookup"><span data-stu-id="11b16-146">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="11b16-147">status</span><span class="sxs-lookup"><span data-stu-id="11b16-147">status</span></span>|[<span data-ttu-id="11b16-148">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="11b16-148">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="11b16-149">Status de conformidade do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="11b16-149">Compliance status of the policy report.</span></span> <span data-ttu-id="11b16-150">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="11b16-150">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="11b16-151">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="11b16-151">lastReportedDateTime</span></span>|<span data-ttu-id="11b16-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11b16-152">DateTimeOffset</span></span>|<span data-ttu-id="11b16-153">Data e hora da última modificação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="11b16-153">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="11b16-154">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="11b16-154">userPrincipalName</span></span>|<span data-ttu-id="11b16-155">String</span><span class="sxs-lookup"><span data-stu-id="11b16-155">String</span></span>|<span data-ttu-id="11b16-156">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="11b16-156">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="11b16-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="11b16-157">Response</span></span>
<span data-ttu-id="11b16-158">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="11b16-158">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11b16-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="11b16-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="11b16-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="11b16-160">Request</span></span>
<span data-ttu-id="11b16-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="11b16-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
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

### <a name="response"></a><span data-ttu-id="11b16-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="11b16-162">Response</span></span>
<span data-ttu-id="11b16-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="11b16-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




