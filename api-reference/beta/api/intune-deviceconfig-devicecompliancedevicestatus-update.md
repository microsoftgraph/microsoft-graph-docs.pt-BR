---
title: Atualizar deviceComplianceDeviceStatus
description: Atualizar as propriedades de um objeto deviceComplianceDeviceStatus.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 35273f196231912f8343130e5a58ff62949579ac
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425488"
---
# <a name="update-devicecompliancedevicestatus"></a><span data-ttu-id="b086e-103">Atualizar deviceComplianceDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="b086e-103">Update deviceComplianceDeviceStatus</span></span>

> <span data-ttu-id="b086e-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="b086e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b086e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b086e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b086e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="b086e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b086e-107">Atualizar as propriedades de um objeto [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="b086e-107">Update the properties of a [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b086e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b086e-108">Prerequisites</span></span>
<span data-ttu-id="b086e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b086e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b086e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b086e-111">Permission type</span></span>|<span data-ttu-id="b086e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b086e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b086e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b086e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b086e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b086e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b086e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b086e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b086e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b086e-116">Not supported.</span></span>|
|<span data-ttu-id="b086e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b086e-117">Application</span></span>|<span data-ttu-id="b086e-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b086e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b086e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b086e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="b086e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b086e-120">Request headers</span></span>
|<span data-ttu-id="b086e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b086e-121">Header</span></span>|<span data-ttu-id="b086e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b086e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b086e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b086e-123">Authorization</span></span>|<span data-ttu-id="b086e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b086e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b086e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b086e-125">Accept</span></span>|<span data-ttu-id="b086e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b086e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b086e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b086e-127">Request body</span></span>
<span data-ttu-id="b086e-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="b086e-128">In the request body, supply a JSON representation for the [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>

<span data-ttu-id="b086e-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="b086e-129">The following table shows the properties that are required when you create the [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span></span>

|<span data-ttu-id="b086e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b086e-130">Property</span></span>|<span data-ttu-id="b086e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b086e-131">Type</span></span>|<span data-ttu-id="b086e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b086e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b086e-133">id</span><span class="sxs-lookup"><span data-stu-id="b086e-133">id</span></span>|<span data-ttu-id="b086e-134">String</span><span class="sxs-lookup"><span data-stu-id="b086e-134">String</span></span>|<span data-ttu-id="b086e-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b086e-135">Key of the entity.</span></span>|
|<span data-ttu-id="b086e-136">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="b086e-136">deviceDisplayName</span></span>|<span data-ttu-id="b086e-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b086e-137">String</span></span>|<span data-ttu-id="b086e-138">Nome do dispositivo de DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="b086e-138">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="b086e-139">userName</span><span class="sxs-lookup"><span data-stu-id="b086e-139">userName</span></span>|<span data-ttu-id="b086e-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b086e-140">String</span></span>|<span data-ttu-id="b086e-141">O nome de usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="b086e-141">The User Name that is being reported</span></span>|
|<span data-ttu-id="b086e-142">deviceModel</span><span class="sxs-lookup"><span data-stu-id="b086e-142">deviceModel</span></span>|<span data-ttu-id="b086e-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b086e-143">String</span></span>|<span data-ttu-id="b086e-144">O modelo do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="b086e-144">The device model that is being reported</span></span>|
|<span data-ttu-id="b086e-145">platform</span><span class="sxs-lookup"><span data-stu-id="b086e-145">platform</span></span>|<span data-ttu-id="b086e-146">Int32</span><span class="sxs-lookup"><span data-stu-id="b086e-146">Int32</span></span>|<span data-ttu-id="b086e-147">Plataforma do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="b086e-147">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="b086e-148">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="b086e-148">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="b086e-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b086e-149">DateTimeOffset</span></span>|<span data-ttu-id="b086e-150">DateTime em que o período de cortesia de conformidade do dispositivo termina</span><span class="sxs-lookup"><span data-stu-id="b086e-150">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="b086e-151">status</span><span class="sxs-lookup"><span data-stu-id="b086e-151">status</span></span>|[<span data-ttu-id="b086e-152">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="b086e-152">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="b086e-153">Status de conformidade do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="b086e-153">Compliance status of the policy report.</span></span> <span data-ttu-id="b086e-154">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="b086e-154">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="b086e-155">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="b086e-155">lastReportedDateTime</span></span>|<span data-ttu-id="b086e-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b086e-156">DateTimeOffset</span></span>|<span data-ttu-id="b086e-157">Data e hora da última modificação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="b086e-157">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="b086e-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b086e-158">userPrincipalName</span></span>|<span data-ttu-id="b086e-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b086e-159">String</span></span>|<span data-ttu-id="b086e-160">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="b086e-160">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="b086e-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="b086e-161">Response</span></span>
<span data-ttu-id="b086e-162">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b086e-162">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b086e-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b086e-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="b086e-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b086e-164">Request</span></span>
<span data-ttu-id="b086e-165">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b086e-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
Content-type: application/json
Content-length: 444

{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceStatus",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "platform": 8,
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="b086e-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="b086e-166">Response</span></span>
<span data-ttu-id="b086e-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b086e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 493

{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceStatus",
  "id": "c6c78124-8124-c6c7-2481-c7c62481c7c6",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "platform": 8,
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```




