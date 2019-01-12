---
title: Criar managedDeviceMobileAppConfigurationUserStatus
description: Criar um novo objeto managedDeviceMobileAppConfigurationUserStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3a02e43ac9758ae888b97a1ec3154e95edffe740
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926957"
---
# <a name="create-manageddevicemobileappconfigurationuserstatus"></a><span data-ttu-id="deebc-103">Criar managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="deebc-103">Create managedDeviceMobileAppConfigurationUserStatus</span></span>

> <span data-ttu-id="deebc-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="deebc-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="deebc-105">Criar um novo objeto [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="deebc-105">Create a new [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="deebc-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="deebc-106">Prerequisites</span></span>
<span data-ttu-id="deebc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="deebc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="deebc-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="deebc-109">Permission type</span></span>|<span data-ttu-id="deebc-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="deebc-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="deebc-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="deebc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="deebc-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="deebc-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="deebc-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="deebc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="deebc-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="deebc-114">Not supported.</span></span>|
|<span data-ttu-id="deebc-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="deebc-115">Application</span></span>|<span data-ttu-id="deebc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="deebc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="deebc-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="deebc-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="deebc-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="deebc-118">Request headers</span></span>
|<span data-ttu-id="deebc-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="deebc-119">Header</span></span>|<span data-ttu-id="deebc-120">Valor</span><span class="sxs-lookup"><span data-stu-id="deebc-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="deebc-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="deebc-121">Authorization</span></span>|<span data-ttu-id="deebc-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="deebc-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="deebc-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="deebc-123">Accept</span></span>|<span data-ttu-id="deebc-124">application/json</span><span class="sxs-lookup"><span data-stu-id="deebc-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="deebc-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="deebc-125">Request body</span></span>
<span data-ttu-id="deebc-126">No corpo da solicitação, forneça uma representação JSON do objeto managedDeviceMobileAppConfigurationUserStatus.</span><span class="sxs-lookup"><span data-stu-id="deebc-126">In the request body, supply a JSON representation for the managedDeviceMobileAppConfigurationUserStatus object.</span></span>

<span data-ttu-id="deebc-127">A tabela a seguir mostra as propriedades que são necessárias ao criar managedDeviceMobileAppConfigurationUserStatus.</span><span class="sxs-lookup"><span data-stu-id="deebc-127">The following table shows the properties that are required when you create the managedDeviceMobileAppConfigurationUserStatus.</span></span>

|<span data-ttu-id="deebc-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="deebc-128">Property</span></span>|<span data-ttu-id="deebc-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="deebc-129">Type</span></span>|<span data-ttu-id="deebc-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="deebc-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="deebc-131">id</span><span class="sxs-lookup"><span data-stu-id="deebc-131">id</span></span>|<span data-ttu-id="deebc-132">String</span><span class="sxs-lookup"><span data-stu-id="deebc-132">String</span></span>|<span data-ttu-id="deebc-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="deebc-133">Key of the entity.</span></span>|
|<span data-ttu-id="deebc-134">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="deebc-134">userDisplayName</span></span>|<span data-ttu-id="deebc-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="deebc-135">String</span></span>|<span data-ttu-id="deebc-136">Nome de usuário de DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="deebc-136">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="deebc-137">devicesCount</span><span class="sxs-lookup"><span data-stu-id="deebc-137">devicesCount</span></span>|<span data-ttu-id="deebc-138">Int32</span><span class="sxs-lookup"><span data-stu-id="deebc-138">Int32</span></span>|<span data-ttu-id="deebc-139">Contagem de dispositivos para esse usuário.</span><span class="sxs-lookup"><span data-stu-id="deebc-139">Devices count for that user.</span></span>|
|<span data-ttu-id="deebc-140">status</span><span class="sxs-lookup"><span data-stu-id="deebc-140">status</span></span>|[<span data-ttu-id="deebc-141">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="deebc-141">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="deebc-142">Status de conformidade do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="deebc-142">Compliance status of the policy report.</span></span> <span data-ttu-id="deebc-143">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="deebc-143">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="deebc-144">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="deebc-144">lastReportedDateTime</span></span>|<span data-ttu-id="deebc-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="deebc-145">DateTimeOffset</span></span>|<span data-ttu-id="deebc-146">Data e hora da última modificação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="deebc-146">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="deebc-147">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="deebc-147">userPrincipalName</span></span>|<span data-ttu-id="deebc-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="deebc-148">String</span></span>|<span data-ttu-id="deebc-149">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="deebc-149">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="deebc-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="deebc-150">Response</span></span>
<span data-ttu-id="deebc-151">Se tiver êxito, este método retornará um código de resposta `201 Created` e o objeto [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="deebc-151">If successful, this method returns a `201 Created` response code and a [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="deebc-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="deebc-152">Example</span></span>
### <a name="request"></a><span data-ttu-id="deebc-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="deebc-153">Request</span></span>
<span data-ttu-id="deebc-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="deebc-154">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses
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

### <a name="response"></a><span data-ttu-id="deebc-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="deebc-155">Response</span></span>
<span data-ttu-id="deebc-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="deebc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



