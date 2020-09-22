---
title: Criar deviceConfigurationUserStatus
description: Criar um novo objeto deviceConfigurationUserStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 747cfce57540c4c19c2774f57fc907e7dbcded12
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48066856"
---
# <a name="create-deviceconfigurationuserstatus"></a><span data-ttu-id="a2790-103">Criar deviceConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="a2790-103">Create deviceConfigurationUserStatus</span></span>

<span data-ttu-id="a2790-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2790-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a2790-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a2790-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2790-106">Criar um novo objeto [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="a2790-106">Create a new [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a2790-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a2790-107">Prerequisites</span></span>
<span data-ttu-id="a2790-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2790-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2790-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a2790-110">Permission type</span></span>|<span data-ttu-id="a2790-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a2790-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2790-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a2790-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a2790-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2790-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a2790-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a2790-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2790-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a2790-115">Not supported.</span></span>|
|<span data-ttu-id="a2790-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a2790-116">Application</span></span>|<span data-ttu-id="a2790-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a2790-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2790-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a2790-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="a2790-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a2790-119">Request headers</span></span>
|<span data-ttu-id="a2790-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a2790-120">Header</span></span>|<span data-ttu-id="a2790-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a2790-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a2790-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a2790-122">Authorization</span></span>|<span data-ttu-id="a2790-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a2790-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a2790-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a2790-124">Accept</span></span>|<span data-ttu-id="a2790-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a2790-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2790-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a2790-126">Request body</span></span>
<span data-ttu-id="a2790-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceConfigurationUserStatus.</span><span class="sxs-lookup"><span data-stu-id="a2790-127">In the request body, supply a JSON representation for the deviceConfigurationUserStatus object.</span></span>

<span data-ttu-id="a2790-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceConfigurationUserStatus.</span><span class="sxs-lookup"><span data-stu-id="a2790-128">The following table shows the properties that are required when you create the deviceConfigurationUserStatus.</span></span>

|<span data-ttu-id="a2790-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a2790-129">Property</span></span>|<span data-ttu-id="a2790-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a2790-130">Type</span></span>|<span data-ttu-id="a2790-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2790-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2790-132">id</span><span class="sxs-lookup"><span data-stu-id="a2790-132">id</span></span>|<span data-ttu-id="a2790-133">String</span><span class="sxs-lookup"><span data-stu-id="a2790-133">String</span></span>|<span data-ttu-id="a2790-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a2790-134">Key of the entity.</span></span>|
|<span data-ttu-id="a2790-135">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="a2790-135">userDisplayName</span></span>|<span data-ttu-id="a2790-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a2790-136">String</span></span>|<span data-ttu-id="a2790-137">Nome de usuário de DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="a2790-137">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="a2790-138">devicesCount</span><span class="sxs-lookup"><span data-stu-id="a2790-138">devicesCount</span></span>|<span data-ttu-id="a2790-139">Int32</span><span class="sxs-lookup"><span data-stu-id="a2790-139">Int32</span></span>|<span data-ttu-id="a2790-140">Contagem de dispositivos para esse usuário.</span><span class="sxs-lookup"><span data-stu-id="a2790-140">Devices count for that user.</span></span>|
|<span data-ttu-id="a2790-141">status</span><span class="sxs-lookup"><span data-stu-id="a2790-141">status</span></span>|[<span data-ttu-id="a2790-142">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="a2790-142">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="a2790-143">Status de conformidade do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="a2790-143">Compliance status of the policy report.</span></span> <span data-ttu-id="a2790-144">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="a2790-144">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="a2790-145">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="a2790-145">lastReportedDateTime</span></span>|<span data-ttu-id="a2790-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2790-146">DateTimeOffset</span></span>|<span data-ttu-id="a2790-147">Data e hora da última modificação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="a2790-147">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="a2790-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a2790-148">userPrincipalName</span></span>|<span data-ttu-id="a2790-149">String</span><span class="sxs-lookup"><span data-stu-id="a2790-149">String</span></span>|<span data-ttu-id="a2790-150">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="a2790-150">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="a2790-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2790-151">Response</span></span>
<span data-ttu-id="a2790-152">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a2790-152">If successful, this method returns a `201 Created` response code and a [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2790-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a2790-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="a2790-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a2790-154">Request</span></span>
<span data-ttu-id="a2790-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a2790-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses
Content-type: application/json
Content-length: 290

{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserStatus",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="a2790-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2790-156">Response</span></span>
<span data-ttu-id="a2790-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a2790-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 339

{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserStatus",
  "id": "7e323db2-3db2-7e32-b23d-327eb23d327e",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```









