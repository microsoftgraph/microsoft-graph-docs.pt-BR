---
title: Criar deviceComplianceUserStatus
description: Criar um novo objeto deviceComplianceUserStatus.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 505884c137fca0249d3be444d09ad1a37039619c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36346090"
---
# <a name="create-devicecomplianceuserstatus"></a><span data-ttu-id="0df3c-103">Criar deviceComplianceUserStatus</span><span class="sxs-lookup"><span data-stu-id="0df3c-103">Create deviceComplianceUserStatus</span></span>

> <span data-ttu-id="0df3c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0df3c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0df3c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0df3c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0df3c-106">Criar um novo objeto [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="0df3c-106">Create a new [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0df3c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0df3c-107">Prerequisites</span></span>
<span data-ttu-id="0df3c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0df3c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0df3c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0df3c-110">Permission type</span></span>|<span data-ttu-id="0df3c-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0df3c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0df3c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0df3c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0df3c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0df3c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0df3c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0df3c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0df3c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0df3c-115">Not supported.</span></span>|
|<span data-ttu-id="0df3c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0df3c-116">Application</span></span>|<span data-ttu-id="0df3c-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0df3c-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0df3c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0df3c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="0df3c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0df3c-119">Request headers</span></span>
|<span data-ttu-id="0df3c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0df3c-120">Header</span></span>|<span data-ttu-id="0df3c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="0df3c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0df3c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0df3c-122">Authorization</span></span>|<span data-ttu-id="0df3c-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0df3c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0df3c-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0df3c-124">Accept</span></span>|<span data-ttu-id="0df3c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0df3c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0df3c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0df3c-126">Request body</span></span>
<span data-ttu-id="0df3c-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceComplianceUserStatus.</span><span class="sxs-lookup"><span data-stu-id="0df3c-127">In the request body, supply a JSON representation for the deviceComplianceUserStatus object.</span></span>

<span data-ttu-id="0df3c-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceComplianceUserStatus.</span><span class="sxs-lookup"><span data-stu-id="0df3c-128">The following table shows the properties that are required when you create the deviceComplianceUserStatus.</span></span>

|<span data-ttu-id="0df3c-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0df3c-129">Property</span></span>|<span data-ttu-id="0df3c-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="0df3c-130">Type</span></span>|<span data-ttu-id="0df3c-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="0df3c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0df3c-132">id</span><span class="sxs-lookup"><span data-stu-id="0df3c-132">id</span></span>|<span data-ttu-id="0df3c-133">String</span><span class="sxs-lookup"><span data-stu-id="0df3c-133">String</span></span>|<span data-ttu-id="0df3c-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0df3c-134">Key of the entity.</span></span>|
|<span data-ttu-id="0df3c-135">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="0df3c-135">userDisplayName</span></span>|<span data-ttu-id="0df3c-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0df3c-136">String</span></span>|<span data-ttu-id="0df3c-137">Nome de usuário de DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="0df3c-137">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="0df3c-138">devicesCount</span><span class="sxs-lookup"><span data-stu-id="0df3c-138">devicesCount</span></span>|<span data-ttu-id="0df3c-139">Int32</span><span class="sxs-lookup"><span data-stu-id="0df3c-139">Int32</span></span>|<span data-ttu-id="0df3c-140">Contagem de dispositivos para esse usuário.</span><span class="sxs-lookup"><span data-stu-id="0df3c-140">Devices count for that user.</span></span>|
|<span data-ttu-id="0df3c-141">status</span><span class="sxs-lookup"><span data-stu-id="0df3c-141">status</span></span>|[<span data-ttu-id="0df3c-142">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="0df3c-142">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="0df3c-143">Status de conformidade do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="0df3c-143">Compliance status of the policy report.</span></span> <span data-ttu-id="0df3c-144">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="0df3c-144">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="0df3c-145">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="0df3c-145">lastReportedDateTime</span></span>|<span data-ttu-id="0df3c-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0df3c-146">DateTimeOffset</span></span>|<span data-ttu-id="0df3c-147">Data e hora da última modificação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="0df3c-147">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="0df3c-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0df3c-148">userPrincipalName</span></span>|<span data-ttu-id="0df3c-149">String</span><span class="sxs-lookup"><span data-stu-id="0df3c-149">String</span></span>|<span data-ttu-id="0df3c-150">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="0df3c-150">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="0df3c-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="0df3c-151">Response</span></span>
<span data-ttu-id="0df3c-152">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0df3c-152">If successful, this method returns a `201 Created` response code and a [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0df3c-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0df3c-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="0df3c-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0df3c-154">Request</span></span>
<span data-ttu-id="0df3c-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0df3c-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses
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

### <a name="response"></a><span data-ttu-id="0df3c-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="0df3c-156">Response</span></span>
<span data-ttu-id="0df3c-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0df3c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






