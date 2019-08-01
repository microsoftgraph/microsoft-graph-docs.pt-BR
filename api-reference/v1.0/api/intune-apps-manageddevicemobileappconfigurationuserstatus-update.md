---
title: Atualizar managedDeviceMobileAppConfigurationUserStatus
description: Atualizar as propriedades de um objeto managedDeviceMobileAppConfigurationUserStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b5f9202c0a01a912eb2aa329e11f3d7efd613ce6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013924"
---
# <a name="update-manageddevicemobileappconfigurationuserstatus"></a><span data-ttu-id="4f2da-103">Atualizar managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="4f2da-103">Update managedDeviceMobileAppConfigurationUserStatus</span></span>

> <span data-ttu-id="4f2da-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4f2da-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f2da-105">Atualizar as propriedades de um objeto [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="4f2da-105">Update the properties of a [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4f2da-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4f2da-106">Prerequisites</span></span>
<span data-ttu-id="4f2da-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f2da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f2da-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4f2da-109">Permission type</span></span>|<span data-ttu-id="4f2da-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4f2da-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4f2da-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4f2da-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4f2da-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f2da-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4f2da-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4f2da-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4f2da-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4f2da-114">Not supported.</span></span>|
|<span data-ttu-id="4f2da-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4f2da-115">Application</span></span>|<span data-ttu-id="4f2da-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4f2da-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4f2da-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4f2da-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses/{managedDeviceMobileAppConfigurationUserStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="4f2da-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4f2da-118">Request headers</span></span>
|<span data-ttu-id="4f2da-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4f2da-119">Header</span></span>|<span data-ttu-id="4f2da-120">Valor</span><span class="sxs-lookup"><span data-stu-id="4f2da-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4f2da-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="4f2da-121">Authorization</span></span>|<span data-ttu-id="4f2da-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4f2da-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4f2da-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4f2da-123">Accept</span></span>|<span data-ttu-id="4f2da-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4f2da-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f2da-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4f2da-125">Request body</span></span>
<span data-ttu-id="4f2da-126">No corpo da solicitação, forneça uma representação JSON do objeto [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="4f2da-126">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>

<span data-ttu-id="4f2da-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="4f2da-127">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span></span>

|<span data-ttu-id="4f2da-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4f2da-128">Property</span></span>|<span data-ttu-id="4f2da-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="4f2da-129">Type</span></span>|<span data-ttu-id="4f2da-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="4f2da-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f2da-131">id</span><span class="sxs-lookup"><span data-stu-id="4f2da-131">id</span></span>|<span data-ttu-id="4f2da-132">String</span><span class="sxs-lookup"><span data-stu-id="4f2da-132">String</span></span>|<span data-ttu-id="4f2da-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4f2da-133">Key of the entity.</span></span>|
|<span data-ttu-id="4f2da-134">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="4f2da-134">userDisplayName</span></span>|<span data-ttu-id="4f2da-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4f2da-135">String</span></span>|<span data-ttu-id="4f2da-136">Nome de usuário de DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="4f2da-136">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="4f2da-137">devicesCount</span><span class="sxs-lookup"><span data-stu-id="4f2da-137">devicesCount</span></span>|<span data-ttu-id="4f2da-138">Int32</span><span class="sxs-lookup"><span data-stu-id="4f2da-138">Int32</span></span>|<span data-ttu-id="4f2da-139">Contagem de dispositivos para esse usuário.</span><span class="sxs-lookup"><span data-stu-id="4f2da-139">Devices count for that user.</span></span>|
|<span data-ttu-id="4f2da-140">status</span><span class="sxs-lookup"><span data-stu-id="4f2da-140">status</span></span>|[<span data-ttu-id="4f2da-141">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="4f2da-141">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="4f2da-142">Status de conformidade do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="4f2da-142">Compliance status of the policy report.</span></span> <span data-ttu-id="4f2da-143">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="4f2da-143">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="4f2da-144">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="4f2da-144">lastReportedDateTime</span></span>|<span data-ttu-id="4f2da-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4f2da-145">DateTimeOffset</span></span>|<span data-ttu-id="4f2da-146">Data e hora da última modificação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="4f2da-146">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="4f2da-147">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4f2da-147">userPrincipalName</span></span>|<span data-ttu-id="4f2da-148">String</span><span class="sxs-lookup"><span data-stu-id="4f2da-148">String</span></span>|<span data-ttu-id="4f2da-149">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="4f2da-149">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="4f2da-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f2da-150">Response</span></span>
<span data-ttu-id="4f2da-151">Se tiver êxito, este método retornará um código de resposta `200 OK` e o objeto [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4f2da-151">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f2da-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4f2da-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="4f2da-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4f2da-153">Request</span></span>
<span data-ttu-id="4f2da-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4f2da-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4f2da-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f2da-155">Response</span></span>
<span data-ttu-id="4f2da-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4f2da-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



