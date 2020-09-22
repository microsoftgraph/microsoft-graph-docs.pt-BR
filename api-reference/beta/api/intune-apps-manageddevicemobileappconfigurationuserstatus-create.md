---
title: Criar managedDeviceMobileAppConfigurationUserStatus
description: Criar um novo objeto managedDeviceMobileAppConfigurationUserStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 60dd31d7376776ee1158b3877e9165052194fbe0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47977884"
---
# <a name="create-manageddevicemobileappconfigurationuserstatus"></a><span data-ttu-id="3bef8-103">Criar managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="3bef8-103">Create managedDeviceMobileAppConfigurationUserStatus</span></span>

<span data-ttu-id="3bef8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3bef8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3bef8-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3bef8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3bef8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3bef8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3bef8-107">Criar um novo objeto [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="3bef8-107">Create a new [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3bef8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3bef8-108">Prerequisites</span></span>
<span data-ttu-id="3bef8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3bef8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3bef8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3bef8-111">Permission type</span></span>|<span data-ttu-id="3bef8-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3bef8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3bef8-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3bef8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3bef8-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3bef8-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3bef8-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3bef8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3bef8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3bef8-116">Not supported.</span></span>|
|<span data-ttu-id="3bef8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3bef8-117">Application</span></span>|<span data-ttu-id="3bef8-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3bef8-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3bef8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3bef8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses
POST /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="3bef8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3bef8-120">Request headers</span></span>
|<span data-ttu-id="3bef8-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3bef8-121">Header</span></span>|<span data-ttu-id="3bef8-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3bef8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3bef8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3bef8-123">Authorization</span></span>|<span data-ttu-id="3bef8-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3bef8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3bef8-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3bef8-125">Accept</span></span>|<span data-ttu-id="3bef8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3bef8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3bef8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3bef8-127">Request body</span></span>
<span data-ttu-id="3bef8-128">No corpo da solicitação, forneça uma representação JSON do objeto managedDeviceMobileAppConfigurationUserStatus.</span><span class="sxs-lookup"><span data-stu-id="3bef8-128">In the request body, supply a JSON representation for the managedDeviceMobileAppConfigurationUserStatus object.</span></span>

<span data-ttu-id="3bef8-129">A tabela a seguir mostra as propriedades que são necessárias ao criar managedDeviceMobileAppConfigurationUserStatus.</span><span class="sxs-lookup"><span data-stu-id="3bef8-129">The following table shows the properties that are required when you create the managedDeviceMobileAppConfigurationUserStatus.</span></span>

|<span data-ttu-id="3bef8-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3bef8-130">Property</span></span>|<span data-ttu-id="3bef8-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="3bef8-131">Type</span></span>|<span data-ttu-id="3bef8-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3bef8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3bef8-133">id</span><span class="sxs-lookup"><span data-stu-id="3bef8-133">id</span></span>|<span data-ttu-id="3bef8-134">String</span><span class="sxs-lookup"><span data-stu-id="3bef8-134">String</span></span>|<span data-ttu-id="3bef8-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="3bef8-135">Key of the entity.</span></span>|
|<span data-ttu-id="3bef8-136">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="3bef8-136">userDisplayName</span></span>|<span data-ttu-id="3bef8-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3bef8-137">String</span></span>|<span data-ttu-id="3bef8-138">Nome de usuário de DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="3bef8-138">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="3bef8-139">devicesCount</span><span class="sxs-lookup"><span data-stu-id="3bef8-139">devicesCount</span></span>|<span data-ttu-id="3bef8-140">Int32</span><span class="sxs-lookup"><span data-stu-id="3bef8-140">Int32</span></span>|<span data-ttu-id="3bef8-141">Contagem de dispositivos para esse usuário.</span><span class="sxs-lookup"><span data-stu-id="3bef8-141">Devices count for that user.</span></span>|
|<span data-ttu-id="3bef8-142">status</span><span class="sxs-lookup"><span data-stu-id="3bef8-142">status</span></span>|[<span data-ttu-id="3bef8-143">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="3bef8-143">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="3bef8-144">Status de conformidade do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="3bef8-144">Compliance status of the policy report.</span></span> <span data-ttu-id="3bef8-145">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="3bef8-145">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="3bef8-146">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="3bef8-146">lastReportedDateTime</span></span>|<span data-ttu-id="3bef8-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3bef8-147">DateTimeOffset</span></span>|<span data-ttu-id="3bef8-148">Data e hora da última modificação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="3bef8-148">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="3bef8-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="3bef8-149">userPrincipalName</span></span>|<span data-ttu-id="3bef8-150">String</span><span class="sxs-lookup"><span data-stu-id="3bef8-150">String</span></span>|<span data-ttu-id="3bef8-151">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="3bef8-151">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="3bef8-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="3bef8-152">Response</span></span>
<span data-ttu-id="3bef8-153">Se tiver êxito, este método retornará um código de resposta `201 Created` e o objeto [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3bef8-153">If successful, this method returns a `201 Created` response code and a [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3bef8-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3bef8-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="3bef8-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3bef8-155">Request</span></span>
<span data-ttu-id="3bef8-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3bef8-156">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses
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

### <a name="response"></a><span data-ttu-id="3bef8-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="3bef8-157">Response</span></span>
<span data-ttu-id="3bef8-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3bef8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






