---
title: Atualizar managedDeviceMobileAppConfigurationUserStatus
description: Atualizar as propriedades de um objeto managedDeviceMobileAppConfigurationUserStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cf319bfa8e0f1126d5f15b5c253962914b7bcb56
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30962852"
---
# <a name="update-manageddevicemobileappconfigurationuserstatus"></a><span data-ttu-id="207e1-103">Atualizar managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="207e1-103">Update managedDeviceMobileAppConfigurationUserStatus</span></span>

> <span data-ttu-id="207e1-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="207e1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="207e1-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="207e1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="207e1-106">Atualizar as propriedades de um objeto [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="207e1-106">Update the properties of a [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="207e1-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="207e1-107">Prerequisites</span></span>
<span data-ttu-id="207e1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="207e1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="207e1-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="207e1-110">Permission type</span></span>|<span data-ttu-id="207e1-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="207e1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="207e1-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="207e1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="207e1-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="207e1-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="207e1-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="207e1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="207e1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="207e1-115">Not supported.</span></span>|
|<span data-ttu-id="207e1-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="207e1-116">Application</span></span>|<span data-ttu-id="207e1-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="207e1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="207e1-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="207e1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses/{managedDeviceMobileAppConfigurationUserStatusId}
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/userStatuses/{managedDeviceMobileAppConfigurationUserStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="207e1-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="207e1-119">Request headers</span></span>
|<span data-ttu-id="207e1-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="207e1-120">Header</span></span>|<span data-ttu-id="207e1-121">Valor</span><span class="sxs-lookup"><span data-stu-id="207e1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="207e1-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="207e1-122">Authorization</span></span>|<span data-ttu-id="207e1-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="207e1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="207e1-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="207e1-124">Accept</span></span>|<span data-ttu-id="207e1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="207e1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="207e1-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="207e1-126">Request body</span></span>
<span data-ttu-id="207e1-127">No corpo da solicitação, forneça uma representação JSON do objeto [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="207e1-127">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>

<span data-ttu-id="207e1-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="207e1-128">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span></span>

|<span data-ttu-id="207e1-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="207e1-129">Property</span></span>|<span data-ttu-id="207e1-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="207e1-130">Type</span></span>|<span data-ttu-id="207e1-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="207e1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="207e1-132">id</span><span class="sxs-lookup"><span data-stu-id="207e1-132">id</span></span>|<span data-ttu-id="207e1-133">String</span><span class="sxs-lookup"><span data-stu-id="207e1-133">String</span></span>|<span data-ttu-id="207e1-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="207e1-134">Key of the entity.</span></span>|
|<span data-ttu-id="207e1-135">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="207e1-135">userDisplayName</span></span>|<span data-ttu-id="207e1-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="207e1-136">String</span></span>|<span data-ttu-id="207e1-137">Nome de usuário de DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="207e1-137">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="207e1-138">devicesCount</span><span class="sxs-lookup"><span data-stu-id="207e1-138">devicesCount</span></span>|<span data-ttu-id="207e1-139">Int32</span><span class="sxs-lookup"><span data-stu-id="207e1-139">Int32</span></span>|<span data-ttu-id="207e1-140">Contagem de dispositivos para esse usuário.</span><span class="sxs-lookup"><span data-stu-id="207e1-140">Devices count for that user.</span></span>|
|<span data-ttu-id="207e1-141">status</span><span class="sxs-lookup"><span data-stu-id="207e1-141">status</span></span>|[<span data-ttu-id="207e1-142">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="207e1-142">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="207e1-143">Status de conformidade do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="207e1-143">Compliance status of the policy report.</span></span> <span data-ttu-id="207e1-144">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="207e1-144">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="207e1-145">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="207e1-145">lastReportedDateTime</span></span>|<span data-ttu-id="207e1-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="207e1-146">DateTimeOffset</span></span>|<span data-ttu-id="207e1-147">Data e hora da última modificação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="207e1-147">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="207e1-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="207e1-148">userPrincipalName</span></span>|<span data-ttu-id="207e1-149">String</span><span class="sxs-lookup"><span data-stu-id="207e1-149">String</span></span>|<span data-ttu-id="207e1-150">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="207e1-150">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="207e1-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="207e1-151">Response</span></span>
<span data-ttu-id="207e1-152">Se tiver êxito, este método retornará um código de resposta `200 OK` e o objeto [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="207e1-152">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="207e1-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="207e1-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="207e1-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="207e1-154">Request</span></span>
<span data-ttu-id="207e1-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="207e1-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="207e1-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="207e1-156">Response</span></span>
<span data-ttu-id="207e1-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="207e1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




