---
title: Atualizar deviceConfigurationUserStatus
description: Atualizar as propriedades de um objeto deviceConfigurationUserStatus.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b8c06f59c6359cf44fcd8cdc839000ed55ead15f
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33926793"
---
# <a name="update-deviceconfigurationuserstatus"></a><span data-ttu-id="1536e-103">Atualizar deviceConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="1536e-103">Update deviceConfigurationUserStatus</span></span>

> <span data-ttu-id="1536e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1536e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1536e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1536e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1536e-106">Atualizar as propriedades de um objeto [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="1536e-106">Update the properties of a [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1536e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1536e-107">Prerequisites</span></span>
<span data-ttu-id="1536e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1536e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1536e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1536e-110">Permission type</span></span>|<span data-ttu-id="1536e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1536e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1536e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1536e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1536e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1536e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1536e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1536e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1536e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1536e-115">Not supported.</span></span>|
|<span data-ttu-id="1536e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1536e-116">Application</span></span>|<span data-ttu-id="1536e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1536e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1536e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1536e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses/{deviceConfigurationUserStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/userStatuses/{deviceConfigurationUserStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/userStatuses/{deviceConfigurationUserStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/userStatuses/{deviceConfigurationUserStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/userStatuses/{deviceConfigurationUserStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/userStatuses/{deviceConfigurationUserStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/userStatuses/{deviceConfigurationUserStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/userStatuses/{deviceConfigurationUserStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/userStatuses/{deviceConfigurationUserStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="1536e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1536e-119">Request headers</span></span>
|<span data-ttu-id="1536e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1536e-120">Header</span></span>|<span data-ttu-id="1536e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="1536e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1536e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1536e-122">Authorization</span></span>|<span data-ttu-id="1536e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1536e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1536e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1536e-124">Accept</span></span>|<span data-ttu-id="1536e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1536e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1536e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1536e-126">Request body</span></span>
<span data-ttu-id="1536e-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="1536e-127">In the request body, supply a JSON representation for the [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object.</span></span>

<span data-ttu-id="1536e-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="1536e-128">The following table shows the properties that are required when you create the [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span></span>

|<span data-ttu-id="1536e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1536e-129">Property</span></span>|<span data-ttu-id="1536e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="1536e-130">Type</span></span>|<span data-ttu-id="1536e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="1536e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1536e-132">id</span><span class="sxs-lookup"><span data-stu-id="1536e-132">id</span></span>|<span data-ttu-id="1536e-133">String</span><span class="sxs-lookup"><span data-stu-id="1536e-133">String</span></span>|<span data-ttu-id="1536e-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="1536e-134">Key of the entity.</span></span>|
|<span data-ttu-id="1536e-135">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="1536e-135">userDisplayName</span></span>|<span data-ttu-id="1536e-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1536e-136">String</span></span>|<span data-ttu-id="1536e-137">Nome de usuário de DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="1536e-137">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="1536e-138">devicesCount</span><span class="sxs-lookup"><span data-stu-id="1536e-138">devicesCount</span></span>|<span data-ttu-id="1536e-139">Int32</span><span class="sxs-lookup"><span data-stu-id="1536e-139">Int32</span></span>|<span data-ttu-id="1536e-140">Contagem de dispositivos para esse usuário.</span><span class="sxs-lookup"><span data-stu-id="1536e-140">Devices count for that user.</span></span>|
|<span data-ttu-id="1536e-141">status</span><span class="sxs-lookup"><span data-stu-id="1536e-141">status</span></span>|[<span data-ttu-id="1536e-142">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="1536e-142">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="1536e-143">Status de conformidade do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="1536e-143">Compliance status of the policy report.</span></span> <span data-ttu-id="1536e-144">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="1536e-144">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="1536e-145">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="1536e-145">lastReportedDateTime</span></span>|<span data-ttu-id="1536e-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1536e-146">DateTimeOffset</span></span>|<span data-ttu-id="1536e-147">Data e hora da última modificação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="1536e-147">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="1536e-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1536e-148">userPrincipalName</span></span>|<span data-ttu-id="1536e-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1536e-149">String</span></span>|<span data-ttu-id="1536e-150">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="1536e-150">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="1536e-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="1536e-151">Response</span></span>
<span data-ttu-id="1536e-152">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1536e-152">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1536e-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1536e-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="1536e-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1536e-154">Request</span></span>
<span data-ttu-id="1536e-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1536e-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses/{deviceConfigurationUserStatusId}
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

### <a name="response"></a><span data-ttu-id="1536e-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="1536e-156">Response</span></span>
<span data-ttu-id="1536e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1536e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




