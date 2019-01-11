---
title: Atualizar managedDeviceMobileAppConfigurationUserStatus
description: Atualizar as propriedades de um objeto managedDeviceMobileAppConfigurationUserStatus.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 23e44eeb6773c24e8959a399231fa5fa4aca5ab0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838385"
---
# <a name="update-manageddevicemobileappconfigurationuserstatus"></a><span data-ttu-id="53cdd-103">Atualizar managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="53cdd-103">Update managedDeviceMobileAppConfigurationUserStatus</span></span>

> <span data-ttu-id="53cdd-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="53cdd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="53cdd-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="53cdd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="53cdd-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="53cdd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="53cdd-107">Atualizar as propriedades de um objeto [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="53cdd-107">Update the properties of a [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="53cdd-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="53cdd-108">Prerequisites</span></span>
<span data-ttu-id="53cdd-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53cdd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53cdd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="53cdd-111">Permission type</span></span>|<span data-ttu-id="53cdd-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="53cdd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53cdd-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="53cdd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="53cdd-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53cdd-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="53cdd-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="53cdd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53cdd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="53cdd-116">Not supported.</span></span>|
|<span data-ttu-id="53cdd-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="53cdd-117">Application</span></span>|<span data-ttu-id="53cdd-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="53cdd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="53cdd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="53cdd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses/{managedDeviceMobileAppConfigurationUserStatusId}
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/userStatuses/{managedDeviceMobileAppConfigurationUserStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="53cdd-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="53cdd-120">Request headers</span></span>
|<span data-ttu-id="53cdd-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="53cdd-121">Header</span></span>|<span data-ttu-id="53cdd-122">Valor</span><span class="sxs-lookup"><span data-stu-id="53cdd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="53cdd-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="53cdd-123">Authorization</span></span>|<span data-ttu-id="53cdd-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="53cdd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="53cdd-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="53cdd-125">Accept</span></span>|<span data-ttu-id="53cdd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="53cdd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="53cdd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="53cdd-127">Request body</span></span>
<span data-ttu-id="53cdd-128">No corpo da solicitação, forneça uma representação JSON do objeto [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="53cdd-128">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>

<span data-ttu-id="53cdd-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="53cdd-129">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span></span>

|<span data-ttu-id="53cdd-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="53cdd-130">Property</span></span>|<span data-ttu-id="53cdd-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="53cdd-131">Type</span></span>|<span data-ttu-id="53cdd-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="53cdd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53cdd-133">id</span><span class="sxs-lookup"><span data-stu-id="53cdd-133">id</span></span>|<span data-ttu-id="53cdd-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="53cdd-134">String</span></span>|<span data-ttu-id="53cdd-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="53cdd-135">Key of the entity.</span></span>|
|<span data-ttu-id="53cdd-136">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="53cdd-136">userDisplayName</span></span>|<span data-ttu-id="53cdd-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="53cdd-137">String</span></span>|<span data-ttu-id="53cdd-138">Nome de usuário de DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="53cdd-138">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="53cdd-139">devicesCount</span><span class="sxs-lookup"><span data-stu-id="53cdd-139">devicesCount</span></span>|<span data-ttu-id="53cdd-140">Int32</span><span class="sxs-lookup"><span data-stu-id="53cdd-140">Int32</span></span>|<span data-ttu-id="53cdd-141">Contagem de dispositivos para esse usuário.</span><span class="sxs-lookup"><span data-stu-id="53cdd-141">Devices count for that user.</span></span>|
|<span data-ttu-id="53cdd-142">status</span><span class="sxs-lookup"><span data-stu-id="53cdd-142">status</span></span>|[<span data-ttu-id="53cdd-143">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="53cdd-143">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="53cdd-144">Status de conformidade do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="53cdd-144">Compliance status of the policy report.</span></span> <span data-ttu-id="53cdd-145">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="53cdd-145">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="53cdd-146">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="53cdd-146">lastReportedDateTime</span></span>|<span data-ttu-id="53cdd-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53cdd-147">DateTimeOffset</span></span>|<span data-ttu-id="53cdd-148">Data e hora da última modificação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="53cdd-148">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="53cdd-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="53cdd-149">userPrincipalName</span></span>|<span data-ttu-id="53cdd-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="53cdd-150">String</span></span>|<span data-ttu-id="53cdd-151">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="53cdd-151">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="53cdd-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="53cdd-152">Response</span></span>
<span data-ttu-id="53cdd-153">Se tiver êxito, este método retornará um código de resposta `200 OK` e o objeto [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="53cdd-153">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53cdd-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="53cdd-154">Example</span></span>
### <a name="request"></a><span data-ttu-id="53cdd-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="53cdd-155">Request</span></span>
<span data-ttu-id="53cdd-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="53cdd-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses/{managedDeviceMobileAppConfigurationUserStatusId}
Content-type: application/json
Content-length: 222

{
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="53cdd-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="53cdd-157">Response</span></span>
<span data-ttu-id="53cdd-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="53cdd-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





