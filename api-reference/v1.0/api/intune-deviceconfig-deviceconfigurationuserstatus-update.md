---
title: Atualizar deviceConfigurationUserStatus
description: Atualizar as propriedades de um objeto deviceConfigurationUserStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e5b4282399bff649a5300f465996137686e7699a
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760598"
---
# <a name="update-deviceconfigurationuserstatus"></a><span data-ttu-id="c3982-103">Atualizar deviceConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="c3982-103">Update deviceConfigurationUserStatus</span></span>

<span data-ttu-id="c3982-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3982-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c3982-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c3982-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3982-106">Atualizar as propriedades de um objeto [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="c3982-106">Update the properties of a [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c3982-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c3982-107">Prerequisites</span></span>
<span data-ttu-id="c3982-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3982-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3982-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c3982-110">Permission type</span></span>|<span data-ttu-id="c3982-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c3982-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3982-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c3982-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c3982-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3982-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c3982-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c3982-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3982-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c3982-115">Not supported.</span></span>|
|<span data-ttu-id="c3982-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c3982-116">Application</span></span>|<span data-ttu-id="c3982-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3982-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3982-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c3982-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses/{deviceConfigurationUserStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="c3982-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c3982-119">Request headers</span></span>
|<span data-ttu-id="c3982-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c3982-120">Header</span></span>|<span data-ttu-id="c3982-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c3982-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c3982-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c3982-122">Authorization</span></span>|<span data-ttu-id="c3982-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c3982-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c3982-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c3982-124">Accept</span></span>|<span data-ttu-id="c3982-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c3982-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3982-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c3982-126">Request body</span></span>
<span data-ttu-id="c3982-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="c3982-127">In the request body, supply a JSON representation for the [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object.</span></span>

<span data-ttu-id="c3982-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="c3982-128">The following table shows the properties that are required when you create the [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span></span>

|<span data-ttu-id="c3982-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c3982-129">Property</span></span>|<span data-ttu-id="c3982-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="c3982-130">Type</span></span>|<span data-ttu-id="c3982-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3982-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3982-132">id</span><span class="sxs-lookup"><span data-stu-id="c3982-132">id</span></span>|<span data-ttu-id="c3982-133">String</span><span class="sxs-lookup"><span data-stu-id="c3982-133">String</span></span>|<span data-ttu-id="c3982-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c3982-134">Key of the entity.</span></span>|
|<span data-ttu-id="c3982-135">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="c3982-135">userDisplayName</span></span>|<span data-ttu-id="c3982-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c3982-136">String</span></span>|<span data-ttu-id="c3982-137">Nome de usuário de DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="c3982-137">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="c3982-138">devicesCount</span><span class="sxs-lookup"><span data-stu-id="c3982-138">devicesCount</span></span>|<span data-ttu-id="c3982-139">Int32</span><span class="sxs-lookup"><span data-stu-id="c3982-139">Int32</span></span>|<span data-ttu-id="c3982-140">Contagem de dispositivos para esse usuário.</span><span class="sxs-lookup"><span data-stu-id="c3982-140">Devices count for that user.</span></span>|
|<span data-ttu-id="c3982-141">status</span><span class="sxs-lookup"><span data-stu-id="c3982-141">status</span></span>|[<span data-ttu-id="c3982-142">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="c3982-142">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="c3982-143">Status de conformidade do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="c3982-143">Compliance status of the policy report.</span></span> <span data-ttu-id="c3982-144">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="c3982-144">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="c3982-145">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="c3982-145">lastReportedDateTime</span></span>|<span data-ttu-id="c3982-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3982-146">DateTimeOffset</span></span>|<span data-ttu-id="c3982-147">Data e hora da última modificação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="c3982-147">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="c3982-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c3982-148">userPrincipalName</span></span>|<span data-ttu-id="c3982-149">String</span><span class="sxs-lookup"><span data-stu-id="c3982-149">String</span></span>|<span data-ttu-id="c3982-150">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="c3982-150">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="c3982-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3982-151">Response</span></span>
<span data-ttu-id="c3982-152">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c3982-152">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3982-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c3982-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="c3982-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c3982-154">Request</span></span>
<span data-ttu-id="c3982-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c3982-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses/{deviceConfigurationUserStatusId}
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

### <a name="response"></a><span data-ttu-id="c3982-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3982-156">Response</span></span>
<span data-ttu-id="c3982-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c3982-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




