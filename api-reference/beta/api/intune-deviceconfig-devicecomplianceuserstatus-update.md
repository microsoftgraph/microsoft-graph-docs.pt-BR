---
title: Atualizar deviceComplianceUserStatus
description: Atualizar as propriedades de um objeto deviceComplianceUserStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2da0402d0869c50ba419f8c87568be0943d047f9
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166126"
---
# <a name="update-devicecomplianceuserstatus"></a><span data-ttu-id="166ae-103">Atualizar deviceComplianceUserStatus</span><span class="sxs-lookup"><span data-stu-id="166ae-103">Update deviceComplianceUserStatus</span></span>

> <span data-ttu-id="166ae-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="166ae-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="166ae-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="166ae-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="166ae-106">Atualizar as propriedades de um objeto [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="166ae-106">Update the properties of a [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="166ae-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="166ae-107">Prerequisites</span></span>
<span data-ttu-id="166ae-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="166ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="166ae-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="166ae-110">Permission type</span></span>|<span data-ttu-id="166ae-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="166ae-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="166ae-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="166ae-112">Delegated (work or school account)</span></span>|<span data-ttu-id="166ae-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="166ae-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="166ae-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="166ae-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="166ae-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="166ae-115">Not supported.</span></span>|
|<span data-ttu-id="166ae-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="166ae-116">Application</span></span>|<span data-ttu-id="166ae-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="166ae-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="166ae-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="166ae-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses/{deviceComplianceUserStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="166ae-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="166ae-119">Request headers</span></span>
|<span data-ttu-id="166ae-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="166ae-120">Header</span></span>|<span data-ttu-id="166ae-121">Valor</span><span class="sxs-lookup"><span data-stu-id="166ae-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="166ae-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="166ae-122">Authorization</span></span>|<span data-ttu-id="166ae-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="166ae-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="166ae-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="166ae-124">Accept</span></span>|<span data-ttu-id="166ae-125">application/json</span><span class="sxs-lookup"><span data-stu-id="166ae-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="166ae-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="166ae-126">Request body</span></span>
<span data-ttu-id="166ae-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="166ae-127">In the request body, supply a JSON representation for the [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object.</span></span>

<span data-ttu-id="166ae-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="166ae-128">The following table shows the properties that are required when you create the [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md).</span></span>

|<span data-ttu-id="166ae-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="166ae-129">Property</span></span>|<span data-ttu-id="166ae-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="166ae-130">Type</span></span>|<span data-ttu-id="166ae-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="166ae-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="166ae-132">id</span><span class="sxs-lookup"><span data-stu-id="166ae-132">id</span></span>|<span data-ttu-id="166ae-133">String</span><span class="sxs-lookup"><span data-stu-id="166ae-133">String</span></span>|<span data-ttu-id="166ae-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="166ae-134">Key of the entity.</span></span>|
|<span data-ttu-id="166ae-135">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="166ae-135">userDisplayName</span></span>|<span data-ttu-id="166ae-136">String</span><span class="sxs-lookup"><span data-stu-id="166ae-136">String</span></span>|<span data-ttu-id="166ae-137">Nome de usuário de DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="166ae-137">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="166ae-138">devicesCount</span><span class="sxs-lookup"><span data-stu-id="166ae-138">devicesCount</span></span>|<span data-ttu-id="166ae-139">Int32</span><span class="sxs-lookup"><span data-stu-id="166ae-139">Int32</span></span>|<span data-ttu-id="166ae-140">Contagem de dispositivos para esse usuário.</span><span class="sxs-lookup"><span data-stu-id="166ae-140">Devices count for that user.</span></span>|
|<span data-ttu-id="166ae-141">status</span><span class="sxs-lookup"><span data-stu-id="166ae-141">status</span></span>|[<span data-ttu-id="166ae-142">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="166ae-142">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="166ae-143">Status de conformidade do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="166ae-143">Compliance status of the policy report.</span></span> <span data-ttu-id="166ae-144">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="166ae-144">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="166ae-145">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="166ae-145">lastReportedDateTime</span></span>|<span data-ttu-id="166ae-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="166ae-146">DateTimeOffset</span></span>|<span data-ttu-id="166ae-147">Data e hora da última modificação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="166ae-147">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="166ae-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="166ae-148">userPrincipalName</span></span>|<span data-ttu-id="166ae-149">String</span><span class="sxs-lookup"><span data-stu-id="166ae-149">String</span></span>|<span data-ttu-id="166ae-150">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="166ae-150">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="166ae-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="166ae-151">Response</span></span>
<span data-ttu-id="166ae-152">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="166ae-152">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="166ae-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="166ae-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="166ae-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="166ae-154">Request</span></span>
<span data-ttu-id="166ae-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="166ae-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses/{deviceComplianceUserStatusId}
Content-type: application/json
Content-length: 287

{
  "@odata.type": "#microsoft.graph.deviceComplianceUserStatus",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="166ae-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="166ae-156">Response</span></span>
<span data-ttu-id="166ae-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="166ae-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 336

{
  "@odata.type": "#microsoft.graph.deviceComplianceUserStatus",
  "id": "a0b566cd-66cd-a0b5-cd66-b5a0cd66b5a0",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```




