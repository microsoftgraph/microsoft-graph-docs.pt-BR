---
title: Atualizar deviceComplianceDeviceStatus
description: Atualizar as propriedades de um objeto deviceComplianceDeviceStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 28643c5e308f026f6aca0b0c600387a35acf4f4f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27968992"
---
# <a name="update-devicecompliancedevicestatus"></a><span data-ttu-id="72782-103">Atualizar deviceComplianceDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="72782-103">Update deviceComplianceDeviceStatus</span></span>

> <span data-ttu-id="72782-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="72782-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="72782-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="72782-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="72782-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="72782-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="72782-107">Atualizar as propriedades de um objeto [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="72782-107">Update the properties of a [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="72782-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="72782-108">Prerequisites</span></span>
<span data-ttu-id="72782-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72782-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72782-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="72782-111">Permission type</span></span>|<span data-ttu-id="72782-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="72782-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="72782-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="72782-113">Delegated (work or school account)</span></span>|<span data-ttu-id="72782-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72782-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="72782-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="72782-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="72782-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="72782-116">Not supported.</span></span>|
|<span data-ttu-id="72782-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="72782-117">Application</span></span>|<span data-ttu-id="72782-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="72782-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="72782-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="72782-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="72782-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="72782-120">Request headers</span></span>
|<span data-ttu-id="72782-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="72782-121">Header</span></span>|<span data-ttu-id="72782-122">Valor</span><span class="sxs-lookup"><span data-stu-id="72782-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="72782-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="72782-123">Authorization</span></span>|<span data-ttu-id="72782-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="72782-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="72782-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="72782-125">Accept</span></span>|<span data-ttu-id="72782-126">application/json</span><span class="sxs-lookup"><span data-stu-id="72782-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="72782-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="72782-127">Request body</span></span>
<span data-ttu-id="72782-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="72782-128">In the request body, supply a JSON representation for the [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>

<span data-ttu-id="72782-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="72782-129">The following table shows the properties that are required when you create the [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span></span>

|<span data-ttu-id="72782-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="72782-130">Property</span></span>|<span data-ttu-id="72782-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="72782-131">Type</span></span>|<span data-ttu-id="72782-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="72782-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72782-133">id</span><span class="sxs-lookup"><span data-stu-id="72782-133">id</span></span>|<span data-ttu-id="72782-134">String</span><span class="sxs-lookup"><span data-stu-id="72782-134">String</span></span>|<span data-ttu-id="72782-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="72782-135">Key of the entity.</span></span>|
|<span data-ttu-id="72782-136">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="72782-136">deviceDisplayName</span></span>|<span data-ttu-id="72782-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="72782-137">String</span></span>|<span data-ttu-id="72782-138">Nome do dispositivo de DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="72782-138">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="72782-139">userName</span><span class="sxs-lookup"><span data-stu-id="72782-139">userName</span></span>|<span data-ttu-id="72782-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="72782-140">String</span></span>|<span data-ttu-id="72782-141">O nome de usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="72782-141">The User Name that is being reported</span></span>|
|<span data-ttu-id="72782-142">deviceModel</span><span class="sxs-lookup"><span data-stu-id="72782-142">deviceModel</span></span>|<span data-ttu-id="72782-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="72782-143">String</span></span>|<span data-ttu-id="72782-144">O modelo do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="72782-144">The device model that is being reported</span></span>|
|<span data-ttu-id="72782-145">platform</span><span class="sxs-lookup"><span data-stu-id="72782-145">platform</span></span>|<span data-ttu-id="72782-146">Int32</span><span class="sxs-lookup"><span data-stu-id="72782-146">Int32</span></span>|<span data-ttu-id="72782-147">Plataforma do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="72782-147">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="72782-148">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="72782-148">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="72782-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="72782-149">DateTimeOffset</span></span>|<span data-ttu-id="72782-150">DateTime em que o período de cortesia de conformidade do dispositivo termina</span><span class="sxs-lookup"><span data-stu-id="72782-150">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="72782-151">status</span><span class="sxs-lookup"><span data-stu-id="72782-151">status</span></span>|[<span data-ttu-id="72782-152">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="72782-152">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="72782-153">Status de conformidade do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="72782-153">Compliance status of the policy report.</span></span> <span data-ttu-id="72782-154">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="72782-154">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="72782-155">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="72782-155">lastReportedDateTime</span></span>|<span data-ttu-id="72782-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="72782-156">DateTimeOffset</span></span>|<span data-ttu-id="72782-157">Data e hora da última modificação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="72782-157">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="72782-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="72782-158">userPrincipalName</span></span>|<span data-ttu-id="72782-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="72782-159">String</span></span>|<span data-ttu-id="72782-160">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="72782-160">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="72782-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="72782-161">Response</span></span>
<span data-ttu-id="72782-162">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="72782-162">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72782-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="72782-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="72782-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="72782-164">Request</span></span>
<span data-ttu-id="72782-165">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="72782-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
Content-type: application/json
Content-length: 377

{
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

### <a name="response"></a><span data-ttu-id="72782-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="72782-166">Response</span></span>
<span data-ttu-id="72782-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="72782-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





