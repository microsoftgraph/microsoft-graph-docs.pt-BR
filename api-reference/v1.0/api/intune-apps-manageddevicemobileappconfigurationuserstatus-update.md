---
title: Atualizar managedDeviceMobileAppConfigurationUserStatus
description: Atualizar as propriedades de um objeto managedDeviceMobileAppConfigurationUserStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 66c862235eb5897639a5baf0598136343c28b3d4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48028928"
---
# <a name="update-manageddevicemobileappconfigurationuserstatus"></a><span data-ttu-id="fd2eb-103">Atualizar managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="fd2eb-103">Update managedDeviceMobileAppConfigurationUserStatus</span></span>

<span data-ttu-id="fd2eb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fd2eb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fd2eb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fd2eb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fd2eb-106">Atualizar as propriedades de um objeto [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="fd2eb-106">Update the properties of a [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fd2eb-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fd2eb-107">Prerequisites</span></span>
<span data-ttu-id="fd2eb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd2eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd2eb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fd2eb-110">Permission type</span></span>|<span data-ttu-id="fd2eb-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fd2eb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fd2eb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fd2eb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fd2eb-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd2eb-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fd2eb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fd2eb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fd2eb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fd2eb-115">Not supported.</span></span>|
|<span data-ttu-id="fd2eb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fd2eb-116">Application</span></span>|<span data-ttu-id="fd2eb-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fd2eb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fd2eb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fd2eb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses/{managedDeviceMobileAppConfigurationUserStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="fd2eb-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fd2eb-119">Request headers</span></span>
|<span data-ttu-id="fd2eb-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fd2eb-120">Header</span></span>|<span data-ttu-id="fd2eb-121">Valor</span><span class="sxs-lookup"><span data-stu-id="fd2eb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fd2eb-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="fd2eb-122">Authorization</span></span>|<span data-ttu-id="fd2eb-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fd2eb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fd2eb-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fd2eb-124">Accept</span></span>|<span data-ttu-id="fd2eb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fd2eb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd2eb-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fd2eb-126">Request body</span></span>
<span data-ttu-id="fd2eb-127">No corpo da solicitação, forneça uma representação JSON do objeto [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="fd2eb-127">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>

<span data-ttu-id="fd2eb-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="fd2eb-128">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span></span>

|<span data-ttu-id="fd2eb-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fd2eb-129">Property</span></span>|<span data-ttu-id="fd2eb-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="fd2eb-130">Type</span></span>|<span data-ttu-id="fd2eb-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="fd2eb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd2eb-132">id</span><span class="sxs-lookup"><span data-stu-id="fd2eb-132">id</span></span>|<span data-ttu-id="fd2eb-133">String</span><span class="sxs-lookup"><span data-stu-id="fd2eb-133">String</span></span>|<span data-ttu-id="fd2eb-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="fd2eb-134">Key of the entity.</span></span>|
|<span data-ttu-id="fd2eb-135">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="fd2eb-135">userDisplayName</span></span>|<span data-ttu-id="fd2eb-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd2eb-136">String</span></span>|<span data-ttu-id="fd2eb-137">Nome de usuário de DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="fd2eb-137">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="fd2eb-138">devicesCount</span><span class="sxs-lookup"><span data-stu-id="fd2eb-138">devicesCount</span></span>|<span data-ttu-id="fd2eb-139">Int32</span><span class="sxs-lookup"><span data-stu-id="fd2eb-139">Int32</span></span>|<span data-ttu-id="fd2eb-140">Contagem de dispositivos para esse usuário.</span><span class="sxs-lookup"><span data-stu-id="fd2eb-140">Devices count for that user.</span></span>|
|<span data-ttu-id="fd2eb-141">status</span><span class="sxs-lookup"><span data-stu-id="fd2eb-141">status</span></span>|[<span data-ttu-id="fd2eb-142">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="fd2eb-142">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="fd2eb-143">Status de conformidade do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="fd2eb-143">Compliance status of the policy report.</span></span> <span data-ttu-id="fd2eb-144">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="fd2eb-144">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="fd2eb-145">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="fd2eb-145">lastReportedDateTime</span></span>|<span data-ttu-id="fd2eb-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd2eb-146">DateTimeOffset</span></span>|<span data-ttu-id="fd2eb-147">Data e hora da última modificação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="fd2eb-147">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="fd2eb-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="fd2eb-148">userPrincipalName</span></span>|<span data-ttu-id="fd2eb-149">String</span><span class="sxs-lookup"><span data-stu-id="fd2eb-149">String</span></span>|<span data-ttu-id="fd2eb-150">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="fd2eb-150">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="fd2eb-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="fd2eb-151">Response</span></span>
<span data-ttu-id="fd2eb-152">Se tiver êxito, este método retornará um código de resposta `200 OK` e o objeto [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fd2eb-152">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd2eb-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fd2eb-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="fd2eb-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fd2eb-154">Request</span></span>
<span data-ttu-id="fd2eb-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fd2eb-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses/{managedDeviceMobileAppConfigurationUserStatusId}
Content-type: application/json
Content-length: 306

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserStatus",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="fd2eb-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="fd2eb-156">Response</span></span>
<span data-ttu-id="fd2eb-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fd2eb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 355

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserStatus",
  "id": "44960944-0944-4496-4409-964444099644",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```









