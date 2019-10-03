---
title: Atualizar deviceComplianceUserStatus
description: Atualizar as propriedades de um objeto deviceComplianceUserStatus.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2c6255c468240509716852d7084d4f6e74be7033
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37368844"
---
# <a name="update-devicecomplianceuserstatus"></a><span data-ttu-id="dd20f-103">Atualizar deviceComplianceUserStatus</span><span class="sxs-lookup"><span data-stu-id="dd20f-103">Update deviceComplianceUserStatus</span></span>

> <span data-ttu-id="dd20f-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dd20f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dd20f-105">Atualizar as propriedades de um objeto [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="dd20f-105">Update the properties of a [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dd20f-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dd20f-106">Prerequisites</span></span>
<span data-ttu-id="dd20f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd20f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd20f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dd20f-109">Permission type</span></span>|<span data-ttu-id="dd20f-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="dd20f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dd20f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dd20f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="dd20f-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd20f-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dd20f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dd20f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dd20f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dd20f-114">Not supported.</span></span>|
|<span data-ttu-id="dd20f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dd20f-115">Application</span></span>|<span data-ttu-id="dd20f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dd20f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dd20f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dd20f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses/{deviceComplianceUserStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="dd20f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dd20f-118">Request headers</span></span>
|<span data-ttu-id="dd20f-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dd20f-119">Header</span></span>|<span data-ttu-id="dd20f-120">Valor</span><span class="sxs-lookup"><span data-stu-id="dd20f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dd20f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="dd20f-121">Authorization</span></span>|<span data-ttu-id="dd20f-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dd20f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dd20f-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dd20f-123">Accept</span></span>|<span data-ttu-id="dd20f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="dd20f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd20f-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dd20f-125">Request body</span></span>
<span data-ttu-id="dd20f-126">No corpo da solicitação, forneça uma representação JSON do objeto [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="dd20f-126">In the request body, supply a JSON representation for the [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object.</span></span>

<span data-ttu-id="dd20f-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="dd20f-127">The following table shows the properties that are required when you create the [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md).</span></span>

|<span data-ttu-id="dd20f-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dd20f-128">Property</span></span>|<span data-ttu-id="dd20f-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="dd20f-129">Type</span></span>|<span data-ttu-id="dd20f-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd20f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd20f-131">id</span><span class="sxs-lookup"><span data-stu-id="dd20f-131">id</span></span>|<span data-ttu-id="dd20f-132">String</span><span class="sxs-lookup"><span data-stu-id="dd20f-132">String</span></span>|<span data-ttu-id="dd20f-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="dd20f-133">Key of the entity.</span></span>|
|<span data-ttu-id="dd20f-134">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="dd20f-134">userDisplayName</span></span>|<span data-ttu-id="dd20f-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dd20f-135">String</span></span>|<span data-ttu-id="dd20f-136">Nome de usuário de DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="dd20f-136">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="dd20f-137">devicesCount</span><span class="sxs-lookup"><span data-stu-id="dd20f-137">devicesCount</span></span>|<span data-ttu-id="dd20f-138">Int32</span><span class="sxs-lookup"><span data-stu-id="dd20f-138">Int32</span></span>|<span data-ttu-id="dd20f-139">Contagem de dispositivos para esse usuário.</span><span class="sxs-lookup"><span data-stu-id="dd20f-139">Devices count for that user.</span></span>|
|<span data-ttu-id="dd20f-140">status</span><span class="sxs-lookup"><span data-stu-id="dd20f-140">status</span></span>|[<span data-ttu-id="dd20f-141">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="dd20f-141">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="dd20f-142">Status de conformidade do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="dd20f-142">Compliance status of the policy report.</span></span> <span data-ttu-id="dd20f-143">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="dd20f-143">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="dd20f-144">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="dd20f-144">lastReportedDateTime</span></span>|<span data-ttu-id="dd20f-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dd20f-145">DateTimeOffset</span></span>|<span data-ttu-id="dd20f-146">Data e hora da última modificação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="dd20f-146">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="dd20f-147">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="dd20f-147">userPrincipalName</span></span>|<span data-ttu-id="dd20f-148">String</span><span class="sxs-lookup"><span data-stu-id="dd20f-148">String</span></span>|<span data-ttu-id="dd20f-149">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="dd20f-149">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="dd20f-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd20f-150">Response</span></span>
<span data-ttu-id="dd20f-151">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dd20f-151">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd20f-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dd20f-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="dd20f-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dd20f-153">Request</span></span>
<span data-ttu-id="dd20f-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dd20f-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses/{deviceComplianceUserStatusId}
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

### <a name="response"></a><span data-ttu-id="dd20f-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd20f-155">Response</span></span>
<span data-ttu-id="dd20f-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dd20f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




