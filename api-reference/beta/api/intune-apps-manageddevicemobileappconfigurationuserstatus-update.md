---
title: Atualizar managedDeviceMobileAppConfigurationUserStatus
description: Atualizar as propriedades de um objeto managedDeviceMobileAppConfigurationUserStatus.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 165d5a30718403a4b9afa3cc5f94511362c1e98a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36329702"
---
# <a name="update-manageddevicemobileappconfigurationuserstatus"></a><span data-ttu-id="1621a-103">Atualizar managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="1621a-103">Update managedDeviceMobileAppConfigurationUserStatus</span></span>

> <span data-ttu-id="1621a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1621a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1621a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1621a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1621a-106">Atualizar as propriedades de um objeto [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="1621a-106">Update the properties of a [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1621a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1621a-107">Prerequisites</span></span>
<span data-ttu-id="1621a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1621a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1621a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1621a-110">Permission type</span></span>|<span data-ttu-id="1621a-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1621a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1621a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1621a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1621a-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1621a-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1621a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1621a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1621a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1621a-115">Not supported.</span></span>|
|<span data-ttu-id="1621a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1621a-116">Application</span></span>|<span data-ttu-id="1621a-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1621a-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1621a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1621a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses/{managedDeviceMobileAppConfigurationUserStatusId}
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/userStatuses/{managedDeviceMobileAppConfigurationUserStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="1621a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1621a-119">Request headers</span></span>
|<span data-ttu-id="1621a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1621a-120">Header</span></span>|<span data-ttu-id="1621a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="1621a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1621a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1621a-122">Authorization</span></span>|<span data-ttu-id="1621a-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1621a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1621a-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1621a-124">Accept</span></span>|<span data-ttu-id="1621a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1621a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1621a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1621a-126">Request body</span></span>
<span data-ttu-id="1621a-127">No corpo da solicitação, forneça uma representação JSON do objeto [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="1621a-127">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>

<span data-ttu-id="1621a-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="1621a-128">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span></span>

|<span data-ttu-id="1621a-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1621a-129">Property</span></span>|<span data-ttu-id="1621a-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="1621a-130">Type</span></span>|<span data-ttu-id="1621a-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="1621a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1621a-132">id</span><span class="sxs-lookup"><span data-stu-id="1621a-132">id</span></span>|<span data-ttu-id="1621a-133">String</span><span class="sxs-lookup"><span data-stu-id="1621a-133">String</span></span>|<span data-ttu-id="1621a-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="1621a-134">Key of the entity.</span></span>|
|<span data-ttu-id="1621a-135">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="1621a-135">userDisplayName</span></span>|<span data-ttu-id="1621a-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1621a-136">String</span></span>|<span data-ttu-id="1621a-137">Nome de usuário de DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="1621a-137">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="1621a-138">devicesCount</span><span class="sxs-lookup"><span data-stu-id="1621a-138">devicesCount</span></span>|<span data-ttu-id="1621a-139">Int32</span><span class="sxs-lookup"><span data-stu-id="1621a-139">Int32</span></span>|<span data-ttu-id="1621a-140">Contagem de dispositivos para esse usuário.</span><span class="sxs-lookup"><span data-stu-id="1621a-140">Devices count for that user.</span></span>|
|<span data-ttu-id="1621a-141">status</span><span class="sxs-lookup"><span data-stu-id="1621a-141">status</span></span>|[<span data-ttu-id="1621a-142">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="1621a-142">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="1621a-143">Status de conformidade do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="1621a-143">Compliance status of the policy report.</span></span> <span data-ttu-id="1621a-144">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="1621a-144">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="1621a-145">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="1621a-145">lastReportedDateTime</span></span>|<span data-ttu-id="1621a-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1621a-146">DateTimeOffset</span></span>|<span data-ttu-id="1621a-147">Data e hora da última modificação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="1621a-147">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="1621a-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1621a-148">userPrincipalName</span></span>|<span data-ttu-id="1621a-149">String</span><span class="sxs-lookup"><span data-stu-id="1621a-149">String</span></span>|<span data-ttu-id="1621a-150">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="1621a-150">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="1621a-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="1621a-151">Response</span></span>
<span data-ttu-id="1621a-152">Se tiver êxito, este método retornará um código de resposta `200 OK` e o objeto [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1621a-152">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1621a-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1621a-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="1621a-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1621a-154">Request</span></span>
<span data-ttu-id="1621a-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1621a-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses/{managedDeviceMobileAppConfigurationUserStatusId}
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

### <a name="response"></a><span data-ttu-id="1621a-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="1621a-156">Response</span></span>
<span data-ttu-id="1621a-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1621a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






