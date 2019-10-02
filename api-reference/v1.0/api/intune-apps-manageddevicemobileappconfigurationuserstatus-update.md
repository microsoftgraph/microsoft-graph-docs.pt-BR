---
title: Atualizar managedDeviceMobileAppConfigurationUserStatus
description: Atualizar as propriedades de um objeto managedDeviceMobileAppConfigurationUserStatus.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bcf0e67cf3570e6bcbed9315841a4a403ad2f503
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37358526"
---
# <a name="update-manageddevicemobileappconfigurationuserstatus"></a><span data-ttu-id="dbf25-103">Atualizar managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="dbf25-103">Update managedDeviceMobileAppConfigurationUserStatus</span></span>

> <span data-ttu-id="dbf25-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dbf25-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dbf25-105">Atualizar as propriedades de um objeto [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="dbf25-105">Update the properties of a [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dbf25-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dbf25-106">Prerequisites</span></span>
<span data-ttu-id="dbf25-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dbf25-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dbf25-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dbf25-109">Permission type</span></span>|<span data-ttu-id="dbf25-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="dbf25-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dbf25-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dbf25-111">Delegated (work or school account)</span></span>|<span data-ttu-id="dbf25-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dbf25-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="dbf25-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dbf25-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dbf25-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dbf25-114">Not supported.</span></span>|
|<span data-ttu-id="dbf25-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dbf25-115">Application</span></span>|<span data-ttu-id="dbf25-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dbf25-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dbf25-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dbf25-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses/{managedDeviceMobileAppConfigurationUserStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="dbf25-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dbf25-118">Request headers</span></span>
|<span data-ttu-id="dbf25-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dbf25-119">Header</span></span>|<span data-ttu-id="dbf25-120">Valor</span><span class="sxs-lookup"><span data-stu-id="dbf25-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dbf25-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="dbf25-121">Authorization</span></span>|<span data-ttu-id="dbf25-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dbf25-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dbf25-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dbf25-123">Accept</span></span>|<span data-ttu-id="dbf25-124">application/json</span><span class="sxs-lookup"><span data-stu-id="dbf25-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dbf25-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dbf25-125">Request body</span></span>
<span data-ttu-id="dbf25-126">No corpo da solicitação, forneça uma representação JSON do objeto [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="dbf25-126">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>

<span data-ttu-id="dbf25-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="dbf25-127">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span></span>

|<span data-ttu-id="dbf25-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dbf25-128">Property</span></span>|<span data-ttu-id="dbf25-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="dbf25-129">Type</span></span>|<span data-ttu-id="dbf25-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="dbf25-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dbf25-131">id</span><span class="sxs-lookup"><span data-stu-id="dbf25-131">id</span></span>|<span data-ttu-id="dbf25-132">String</span><span class="sxs-lookup"><span data-stu-id="dbf25-132">String</span></span>|<span data-ttu-id="dbf25-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="dbf25-133">Key of the entity.</span></span>|
|<span data-ttu-id="dbf25-134">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="dbf25-134">userDisplayName</span></span>|<span data-ttu-id="dbf25-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dbf25-135">String</span></span>|<span data-ttu-id="dbf25-136">Nome de usuário de DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="dbf25-136">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="dbf25-137">devicesCount</span><span class="sxs-lookup"><span data-stu-id="dbf25-137">devicesCount</span></span>|<span data-ttu-id="dbf25-138">Int32</span><span class="sxs-lookup"><span data-stu-id="dbf25-138">Int32</span></span>|<span data-ttu-id="dbf25-139">Contagem de dispositivos para esse usuário.</span><span class="sxs-lookup"><span data-stu-id="dbf25-139">Devices count for that user.</span></span>|
|<span data-ttu-id="dbf25-140">status</span><span class="sxs-lookup"><span data-stu-id="dbf25-140">status</span></span>|[<span data-ttu-id="dbf25-141">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="dbf25-141">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="dbf25-142">Status de conformidade do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="dbf25-142">Compliance status of the policy report.</span></span> <span data-ttu-id="dbf25-143">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="dbf25-143">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="dbf25-144">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="dbf25-144">lastReportedDateTime</span></span>|<span data-ttu-id="dbf25-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dbf25-145">DateTimeOffset</span></span>|<span data-ttu-id="dbf25-146">Data e hora da última modificação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="dbf25-146">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="dbf25-147">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="dbf25-147">userPrincipalName</span></span>|<span data-ttu-id="dbf25-148">String</span><span class="sxs-lookup"><span data-stu-id="dbf25-148">String</span></span>|<span data-ttu-id="dbf25-149">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="dbf25-149">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="dbf25-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="dbf25-150">Response</span></span>
<span data-ttu-id="dbf25-151">Se tiver êxito, este método retornará um código de resposta `200 OK` e o objeto [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dbf25-151">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dbf25-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dbf25-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="dbf25-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dbf25-153">Request</span></span>
<span data-ttu-id="dbf25-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dbf25-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="dbf25-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="dbf25-155">Response</span></span>
<span data-ttu-id="dbf25-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dbf25-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




