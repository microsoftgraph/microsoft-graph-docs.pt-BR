---
title: Criar managedDeviceMobileAppConfigurationUserStatus
description: Criar um novo objeto managedDeviceMobileAppConfigurationUserStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: edeeb8966cef97cc0d581f0d0d356f79dbe71096
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754207"
---
# <a name="create-manageddevicemobileappconfigurationuserstatus"></a><span data-ttu-id="017a3-103">Criar managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="017a3-103">Create managedDeviceMobileAppConfigurationUserStatus</span></span>

<span data-ttu-id="017a3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="017a3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="017a3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="017a3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="017a3-106">Criar um novo objeto [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="017a3-106">Create a new [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="017a3-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="017a3-107">Prerequisites</span></span>
<span data-ttu-id="017a3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="017a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="017a3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="017a3-110">Permission type</span></span>|<span data-ttu-id="017a3-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="017a3-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="017a3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="017a3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="017a3-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="017a3-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="017a3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="017a3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="017a3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="017a3-115">Not supported.</span></span>|
|<span data-ttu-id="017a3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="017a3-116">Application</span></span>|<span data-ttu-id="017a3-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="017a3-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="017a3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="017a3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="017a3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="017a3-119">Request headers</span></span>
|<span data-ttu-id="017a3-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="017a3-120">Header</span></span>|<span data-ttu-id="017a3-121">Valor</span><span class="sxs-lookup"><span data-stu-id="017a3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="017a3-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="017a3-122">Authorization</span></span>|<span data-ttu-id="017a3-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="017a3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="017a3-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="017a3-124">Accept</span></span>|<span data-ttu-id="017a3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="017a3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="017a3-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="017a3-126">Request body</span></span>
<span data-ttu-id="017a3-127">No corpo da solicitação, forneça uma representação JSON do objeto managedDeviceMobileAppConfigurationUserStatus.</span><span class="sxs-lookup"><span data-stu-id="017a3-127">In the request body, supply a JSON representation for the managedDeviceMobileAppConfigurationUserStatus object.</span></span>

<span data-ttu-id="017a3-128">A tabela a seguir mostra as propriedades que são necessárias ao criar managedDeviceMobileAppConfigurationUserStatus.</span><span class="sxs-lookup"><span data-stu-id="017a3-128">The following table shows the properties that are required when you create the managedDeviceMobileAppConfigurationUserStatus.</span></span>

|<span data-ttu-id="017a3-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="017a3-129">Property</span></span>|<span data-ttu-id="017a3-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="017a3-130">Type</span></span>|<span data-ttu-id="017a3-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="017a3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="017a3-132">id</span><span class="sxs-lookup"><span data-stu-id="017a3-132">id</span></span>|<span data-ttu-id="017a3-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="017a3-133">String</span></span>|<span data-ttu-id="017a3-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="017a3-134">Key of the entity.</span></span>|
|<span data-ttu-id="017a3-135">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="017a3-135">userDisplayName</span></span>|<span data-ttu-id="017a3-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="017a3-136">String</span></span>|<span data-ttu-id="017a3-137">Nome de usuário de DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="017a3-137">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="017a3-138">devicesCount</span><span class="sxs-lookup"><span data-stu-id="017a3-138">devicesCount</span></span>|<span data-ttu-id="017a3-139">Int32</span><span class="sxs-lookup"><span data-stu-id="017a3-139">Int32</span></span>|<span data-ttu-id="017a3-140">Contagem de dispositivos para esse usuário.</span><span class="sxs-lookup"><span data-stu-id="017a3-140">Devices count for that user.</span></span>|
|<span data-ttu-id="017a3-141">status</span><span class="sxs-lookup"><span data-stu-id="017a3-141">status</span></span>|[<span data-ttu-id="017a3-142">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="017a3-142">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="017a3-143">Status de conformidade do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="017a3-143">Compliance status of the policy report.</span></span> <span data-ttu-id="017a3-144">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="017a3-144">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="017a3-145">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="017a3-145">lastReportedDateTime</span></span>|<span data-ttu-id="017a3-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="017a3-146">DateTimeOffset</span></span>|<span data-ttu-id="017a3-147">Data e hora da última modificação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="017a3-147">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="017a3-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="017a3-148">userPrincipalName</span></span>|<span data-ttu-id="017a3-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="017a3-149">String</span></span>|<span data-ttu-id="017a3-150">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="017a3-150">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="017a3-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="017a3-151">Response</span></span>
<span data-ttu-id="017a3-152">Se tiver êxito, este método retornará um código de resposta `201 Created` e o objeto [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="017a3-152">If successful, this method returns a `201 Created` response code and a [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="017a3-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="017a3-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="017a3-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="017a3-154">Request</span></span>
<span data-ttu-id="017a3-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="017a3-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="017a3-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="017a3-156">Response</span></span>
<span data-ttu-id="017a3-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="017a3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




