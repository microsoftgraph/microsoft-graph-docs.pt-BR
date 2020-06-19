---
title: Atualizar deviceConfigurationUserStatus
description: Atualizar as propriedades de um objeto deviceConfigurationUserStatus.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 01399d41441569fd4b7fd4eba16ee2da4e9ef011
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792839"
---
# <a name="update-deviceconfigurationuserstatus"></a><span data-ttu-id="aaf76-103">Atualizar deviceConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="aaf76-103">Update deviceConfigurationUserStatus</span></span>

<span data-ttu-id="aaf76-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aaf76-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aaf76-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="aaf76-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aaf76-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="aaf76-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aaf76-107">Atualizar as propriedades de um objeto [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="aaf76-107">Update the properties of a [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aaf76-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="aaf76-108">Prerequisites</span></span>
<span data-ttu-id="aaf76-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="aaf76-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="aaf76-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aaf76-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aaf76-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aaf76-111">Permission type</span></span>|<span data-ttu-id="aaf76-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="aaf76-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aaf76-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aaf76-113">Delegated (work or school account)</span></span>|<span data-ttu-id="aaf76-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aaf76-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="aaf76-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aaf76-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aaf76-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aaf76-116">Not supported.</span></span>|
|<span data-ttu-id="aaf76-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aaf76-117">Application</span></span>|<span data-ttu-id="aaf76-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aaf76-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="aaf76-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aaf76-119">HTTP Request</span></span>
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
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/userStatuses/{deviceConfigurationUserStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/userStatuses/{deviceConfigurationUserStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/userStatuses/{deviceConfigurationUserStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/userStatuses/{deviceConfigurationUserStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerEnterpriseWiFiConfiguration/identityCertificateForClientAuthentication/userStatuses/{deviceConfigurationUserStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/userStatuses/{deviceConfigurationUserStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="aaf76-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aaf76-120">Request headers</span></span>
|<span data-ttu-id="aaf76-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="aaf76-121">Header</span></span>|<span data-ttu-id="aaf76-122">Valor</span><span class="sxs-lookup"><span data-stu-id="aaf76-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aaf76-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="aaf76-123">Authorization</span></span>|<span data-ttu-id="aaf76-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aaf76-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aaf76-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="aaf76-125">Accept</span></span>|<span data-ttu-id="aaf76-126">application/json</span><span class="sxs-lookup"><span data-stu-id="aaf76-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aaf76-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aaf76-127">Request body</span></span>
<span data-ttu-id="aaf76-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="aaf76-128">In the request body, supply a JSON representation for the [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object.</span></span>

<span data-ttu-id="aaf76-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="aaf76-129">The following table shows the properties that are required when you create the [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span></span>

|<span data-ttu-id="aaf76-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="aaf76-130">Property</span></span>|<span data-ttu-id="aaf76-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="aaf76-131">Type</span></span>|<span data-ttu-id="aaf76-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="aaf76-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aaf76-133">id</span><span class="sxs-lookup"><span data-stu-id="aaf76-133">id</span></span>|<span data-ttu-id="aaf76-134">String</span><span class="sxs-lookup"><span data-stu-id="aaf76-134">String</span></span>|<span data-ttu-id="aaf76-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="aaf76-135">Key of the entity.</span></span>|
|<span data-ttu-id="aaf76-136">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="aaf76-136">userDisplayName</span></span>|<span data-ttu-id="aaf76-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aaf76-137">String</span></span>|<span data-ttu-id="aaf76-138">Nome de usuário de DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="aaf76-138">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="aaf76-139">devicesCount</span><span class="sxs-lookup"><span data-stu-id="aaf76-139">devicesCount</span></span>|<span data-ttu-id="aaf76-140">Int32</span><span class="sxs-lookup"><span data-stu-id="aaf76-140">Int32</span></span>|<span data-ttu-id="aaf76-141">Contagem de dispositivos para esse usuário.</span><span class="sxs-lookup"><span data-stu-id="aaf76-141">Devices count for that user.</span></span>|
|<span data-ttu-id="aaf76-142">status</span><span class="sxs-lookup"><span data-stu-id="aaf76-142">status</span></span>|[<span data-ttu-id="aaf76-143">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="aaf76-143">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="aaf76-144">Status de conformidade do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="aaf76-144">Compliance status of the policy report.</span></span> <span data-ttu-id="aaf76-145">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="aaf76-145">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="aaf76-146">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="aaf76-146">lastReportedDateTime</span></span>|<span data-ttu-id="aaf76-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aaf76-147">DateTimeOffset</span></span>|<span data-ttu-id="aaf76-148">Data e hora da última modificação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="aaf76-148">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="aaf76-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="aaf76-149">userPrincipalName</span></span>|<span data-ttu-id="aaf76-150">String</span><span class="sxs-lookup"><span data-stu-id="aaf76-150">String</span></span>|<span data-ttu-id="aaf76-151">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="aaf76-151">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="aaf76-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="aaf76-152">Response</span></span>
<span data-ttu-id="aaf76-153">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aaf76-153">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aaf76-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aaf76-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="aaf76-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aaf76-155">Request</span></span>
<span data-ttu-id="aaf76-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="aaf76-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="aaf76-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="aaf76-157">Response</span></span>
<span data-ttu-id="aaf76-158">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="aaf76-158">Here is an example of the response.</span></span> <span data-ttu-id="aaf76-159">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="aaf76-159">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="aaf76-160">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="aaf76-160">All of the properties will be returned from an actual call.</span></span>
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



