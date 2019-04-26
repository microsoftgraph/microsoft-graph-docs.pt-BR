---
title: Criar deviceConfigurationUserStatus
description: Criar um novo objeto deviceConfigurationUserStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 280e961cc25aa4eba2a739544055975013b88c51
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32565846"
---
# <a name="create-deviceconfigurationuserstatus"></a><span data-ttu-id="dbec9-103">Criar deviceConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="dbec9-103">Create deviceConfigurationUserStatus</span></span>

> <span data-ttu-id="dbec9-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dbec9-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dbec9-105">Criar um novo objeto [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="dbec9-105">Create a new [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dbec9-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dbec9-106">Prerequisites</span></span>
<span data-ttu-id="dbec9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dbec9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dbec9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dbec9-109">Permission type</span></span>|<span data-ttu-id="dbec9-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="dbec9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dbec9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dbec9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="dbec9-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dbec9-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dbec9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dbec9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dbec9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dbec9-114">Not supported.</span></span>|
|<span data-ttu-id="dbec9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dbec9-115">Application</span></span>|<span data-ttu-id="dbec9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dbec9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dbec9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dbec9-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="dbec9-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dbec9-118">Request headers</span></span>
|<span data-ttu-id="dbec9-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dbec9-119">Header</span></span>|<span data-ttu-id="dbec9-120">Valor</span><span class="sxs-lookup"><span data-stu-id="dbec9-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dbec9-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="dbec9-121">Authorization</span></span>|<span data-ttu-id="dbec9-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dbec9-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dbec9-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dbec9-123">Accept</span></span>|<span data-ttu-id="dbec9-124">application/json</span><span class="sxs-lookup"><span data-stu-id="dbec9-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dbec9-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dbec9-125">Request body</span></span>
<span data-ttu-id="dbec9-126">No corpo da solicitação, forneça uma representação JSON do objeto deviceConfigurationUserStatus.</span><span class="sxs-lookup"><span data-stu-id="dbec9-126">In the request body, supply a JSON representation for the deviceConfigurationUserStatus object.</span></span>

<span data-ttu-id="dbec9-127">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceConfigurationUserStatus.</span><span class="sxs-lookup"><span data-stu-id="dbec9-127">The following table shows the properties that are required when you create the deviceConfigurationUserStatus.</span></span>

|<span data-ttu-id="dbec9-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dbec9-128">Property</span></span>|<span data-ttu-id="dbec9-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="dbec9-129">Type</span></span>|<span data-ttu-id="dbec9-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="dbec9-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dbec9-131">id</span><span class="sxs-lookup"><span data-stu-id="dbec9-131">id</span></span>|<span data-ttu-id="dbec9-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dbec9-132">String</span></span>|<span data-ttu-id="dbec9-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="dbec9-133">Key of the entity.</span></span>|
|<span data-ttu-id="dbec9-134">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="dbec9-134">userDisplayName</span></span>|<span data-ttu-id="dbec9-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dbec9-135">String</span></span>|<span data-ttu-id="dbec9-136">Nome de usuário de DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="dbec9-136">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="dbec9-137">devicesCount</span><span class="sxs-lookup"><span data-stu-id="dbec9-137">devicesCount</span></span>|<span data-ttu-id="dbec9-138">Int32</span><span class="sxs-lookup"><span data-stu-id="dbec9-138">Int32</span></span>|<span data-ttu-id="dbec9-139">Contagem de dispositivos para esse usuário.</span><span class="sxs-lookup"><span data-stu-id="dbec9-139">Devices count for that user.</span></span>|
|<span data-ttu-id="dbec9-140">status</span><span class="sxs-lookup"><span data-stu-id="dbec9-140">status</span></span>|[<span data-ttu-id="dbec9-141">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="dbec9-141">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="dbec9-142">Status de conformidade do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="dbec9-142">Compliance status of the policy report.</span></span> <span data-ttu-id="dbec9-143">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="dbec9-143">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="dbec9-144">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="dbec9-144">lastReportedDateTime</span></span>|<span data-ttu-id="dbec9-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dbec9-145">DateTimeOffset</span></span>|<span data-ttu-id="dbec9-146">Data e hora da última modificação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="dbec9-146">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="dbec9-147">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="dbec9-147">userPrincipalName</span></span>|<span data-ttu-id="dbec9-148">String</span><span class="sxs-lookup"><span data-stu-id="dbec9-148">String</span></span>|<span data-ttu-id="dbec9-149">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="dbec9-149">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="dbec9-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="dbec9-150">Response</span></span>
<span data-ttu-id="dbec9-151">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dbec9-151">If successful, this method returns a `201 Created` response code and a [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dbec9-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dbec9-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="dbec9-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dbec9-153">Request</span></span>
<span data-ttu-id="dbec9-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dbec9-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="dbec9-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="dbec9-155">Response</span></span>
<span data-ttu-id="dbec9-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dbec9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



