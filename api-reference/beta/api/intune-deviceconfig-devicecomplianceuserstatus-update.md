---
title: Atualizar deviceComplianceUserStatus
description: Atualizar as propriedades de um objeto deviceComplianceUserStatus.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fcc5a75465e3517cf462c853ee582bcd9d8a832c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42449205"
---
# <a name="update-devicecomplianceuserstatus"></a><span data-ttu-id="b7aa5-103">Atualizar deviceComplianceUserStatus</span><span class="sxs-lookup"><span data-stu-id="b7aa5-103">Update deviceComplianceUserStatus</span></span>

<span data-ttu-id="b7aa5-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b7aa5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b7aa5-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b7aa5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b7aa5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b7aa5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7aa5-107">Atualizar as propriedades de um objeto [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="b7aa5-107">Update the properties of a [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b7aa5-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b7aa5-108">Prerequisites</span></span>
<span data-ttu-id="b7aa5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7aa5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7aa5-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b7aa5-111">Permission type</span></span>|<span data-ttu-id="b7aa5-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b7aa5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b7aa5-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b7aa5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b7aa5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7aa5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b7aa5-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b7aa5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b7aa5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b7aa5-116">Not supported.</span></span>|
|<span data-ttu-id="b7aa5-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b7aa5-117">Application</span></span>|<span data-ttu-id="b7aa5-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7aa5-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b7aa5-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b7aa5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses/{deviceComplianceUserStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="b7aa5-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b7aa5-120">Request headers</span></span>
|<span data-ttu-id="b7aa5-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b7aa5-121">Header</span></span>|<span data-ttu-id="b7aa5-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b7aa5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b7aa5-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b7aa5-123">Authorization</span></span>|<span data-ttu-id="b7aa5-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b7aa5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b7aa5-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b7aa5-125">Accept</span></span>|<span data-ttu-id="b7aa5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b7aa5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7aa5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b7aa5-127">Request body</span></span>
<span data-ttu-id="b7aa5-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="b7aa5-128">In the request body, supply a JSON representation for the [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object.</span></span>

<span data-ttu-id="b7aa5-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="b7aa5-129">The following table shows the properties that are required when you create the [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md).</span></span>

|<span data-ttu-id="b7aa5-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b7aa5-130">Property</span></span>|<span data-ttu-id="b7aa5-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b7aa5-131">Type</span></span>|<span data-ttu-id="b7aa5-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b7aa5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7aa5-133">id</span><span class="sxs-lookup"><span data-stu-id="b7aa5-133">id</span></span>|<span data-ttu-id="b7aa5-134">String</span><span class="sxs-lookup"><span data-stu-id="b7aa5-134">String</span></span>|<span data-ttu-id="b7aa5-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b7aa5-135">Key of the entity.</span></span>|
|<span data-ttu-id="b7aa5-136">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="b7aa5-136">userDisplayName</span></span>|<span data-ttu-id="b7aa5-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b7aa5-137">String</span></span>|<span data-ttu-id="b7aa5-138">Nome de usuário de DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="b7aa5-138">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="b7aa5-139">devicesCount</span><span class="sxs-lookup"><span data-stu-id="b7aa5-139">devicesCount</span></span>|<span data-ttu-id="b7aa5-140">Int32</span><span class="sxs-lookup"><span data-stu-id="b7aa5-140">Int32</span></span>|<span data-ttu-id="b7aa5-141">Contagem de dispositivos para esse usuário.</span><span class="sxs-lookup"><span data-stu-id="b7aa5-141">Devices count for that user.</span></span>|
|<span data-ttu-id="b7aa5-142">status</span><span class="sxs-lookup"><span data-stu-id="b7aa5-142">status</span></span>|[<span data-ttu-id="b7aa5-143">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="b7aa5-143">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="b7aa5-144">Status de conformidade do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="b7aa5-144">Compliance status of the policy report.</span></span> <span data-ttu-id="b7aa5-145">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="b7aa5-145">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="b7aa5-146">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="b7aa5-146">lastReportedDateTime</span></span>|<span data-ttu-id="b7aa5-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b7aa5-147">DateTimeOffset</span></span>|<span data-ttu-id="b7aa5-148">Data e hora da última modificação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="b7aa5-148">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="b7aa5-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b7aa5-149">userPrincipalName</span></span>|<span data-ttu-id="b7aa5-150">String</span><span class="sxs-lookup"><span data-stu-id="b7aa5-150">String</span></span>|<span data-ttu-id="b7aa5-151">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="b7aa5-151">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="b7aa5-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7aa5-152">Response</span></span>
<span data-ttu-id="b7aa5-153">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b7aa5-153">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7aa5-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b7aa5-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="b7aa5-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b7aa5-155">Request</span></span>
<span data-ttu-id="b7aa5-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b7aa5-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b7aa5-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7aa5-157">Response</span></span>
<span data-ttu-id="b7aa5-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b7aa5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





