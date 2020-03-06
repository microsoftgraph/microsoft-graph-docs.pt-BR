---
title: Criar deviceComplianceUserStatus
description: Criar um novo objeto deviceComplianceUserStatus.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 594e40f277bfcbdcb89edcab2a1a11a58d505f4e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42514891"
---
# <a name="create-devicecomplianceuserstatus"></a><span data-ttu-id="46161-103">Criar deviceComplianceUserStatus</span><span class="sxs-lookup"><span data-stu-id="46161-103">Create deviceComplianceUserStatus</span></span>

<span data-ttu-id="46161-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="46161-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="46161-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="46161-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46161-106">Criar um novo objeto [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="46161-106">Create a new [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="46161-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="46161-107">Prerequisites</span></span>
<span data-ttu-id="46161-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46161-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46161-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="46161-110">Permission type</span></span>|<span data-ttu-id="46161-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="46161-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46161-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="46161-112">Delegated (work or school account)</span></span>|<span data-ttu-id="46161-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46161-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="46161-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="46161-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46161-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="46161-115">Not supported.</span></span>|
|<span data-ttu-id="46161-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="46161-116">Application</span></span>|<span data-ttu-id="46161-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="46161-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="46161-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="46161-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="46161-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="46161-119">Request headers</span></span>
|<span data-ttu-id="46161-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="46161-120">Header</span></span>|<span data-ttu-id="46161-121">Valor</span><span class="sxs-lookup"><span data-stu-id="46161-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="46161-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="46161-122">Authorization</span></span>|<span data-ttu-id="46161-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="46161-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="46161-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="46161-124">Accept</span></span>|<span data-ttu-id="46161-125">application/json</span><span class="sxs-lookup"><span data-stu-id="46161-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="46161-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="46161-126">Request body</span></span>
<span data-ttu-id="46161-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceComplianceUserStatus.</span><span class="sxs-lookup"><span data-stu-id="46161-127">In the request body, supply a JSON representation for the deviceComplianceUserStatus object.</span></span>

<span data-ttu-id="46161-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceComplianceUserStatus.</span><span class="sxs-lookup"><span data-stu-id="46161-128">The following table shows the properties that are required when you create the deviceComplianceUserStatus.</span></span>

|<span data-ttu-id="46161-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="46161-129">Property</span></span>|<span data-ttu-id="46161-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="46161-130">Type</span></span>|<span data-ttu-id="46161-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="46161-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46161-132">id</span><span class="sxs-lookup"><span data-stu-id="46161-132">id</span></span>|<span data-ttu-id="46161-133">String</span><span class="sxs-lookup"><span data-stu-id="46161-133">String</span></span>|<span data-ttu-id="46161-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="46161-134">Key of the entity.</span></span>|
|<span data-ttu-id="46161-135">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="46161-135">userDisplayName</span></span>|<span data-ttu-id="46161-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="46161-136">String</span></span>|<span data-ttu-id="46161-137">Nome de usuário de DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="46161-137">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="46161-138">devicesCount</span><span class="sxs-lookup"><span data-stu-id="46161-138">devicesCount</span></span>|<span data-ttu-id="46161-139">Int32</span><span class="sxs-lookup"><span data-stu-id="46161-139">Int32</span></span>|<span data-ttu-id="46161-140">Contagem de dispositivos para esse usuário.</span><span class="sxs-lookup"><span data-stu-id="46161-140">Devices count for that user.</span></span>|
|<span data-ttu-id="46161-141">status</span><span class="sxs-lookup"><span data-stu-id="46161-141">status</span></span>|[<span data-ttu-id="46161-142">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="46161-142">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="46161-143">Status de conformidade do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="46161-143">Compliance status of the policy report.</span></span> <span data-ttu-id="46161-144">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="46161-144">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="46161-145">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="46161-145">lastReportedDateTime</span></span>|<span data-ttu-id="46161-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="46161-146">DateTimeOffset</span></span>|<span data-ttu-id="46161-147">Data e hora da última modificação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="46161-147">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="46161-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="46161-148">userPrincipalName</span></span>|<span data-ttu-id="46161-149">String</span><span class="sxs-lookup"><span data-stu-id="46161-149">String</span></span>|<span data-ttu-id="46161-150">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="46161-150">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="46161-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="46161-151">Response</span></span>
<span data-ttu-id="46161-152">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="46161-152">If successful, this method returns a `201 Created` response code and a [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46161-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="46161-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="46161-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="46161-154">Request</span></span>
<span data-ttu-id="46161-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="46161-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses
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

### <a name="response"></a><span data-ttu-id="46161-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="46161-156">Response</span></span>
<span data-ttu-id="46161-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="46161-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




