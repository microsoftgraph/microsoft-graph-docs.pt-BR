---
title: Atualizar deviceConfigurationUserStatus
description: Atualizar as propriedades de um objeto deviceConfigurationUserStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ed3f4f62cfbc96fa69408e1f825e7ffba0fc648d
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48694708"
---
# <a name="update-deviceconfigurationuserstatus"></a><span data-ttu-id="f2f6f-103">Atualizar deviceConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="f2f6f-103">Update deviceConfigurationUserStatus</span></span>

<span data-ttu-id="f2f6f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2f6f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f2f6f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f2f6f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f2f6f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f2f6f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2f6f-107">Atualizar as propriedades de um objeto [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="f2f6f-107">Update the properties of a [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f2f6f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f2f6f-108">Prerequisites</span></span>
<span data-ttu-id="f2f6f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2f6f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2f6f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f2f6f-111">Permission type</span></span>|<span data-ttu-id="f2f6f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f2f6f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2f6f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f2f6f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f2f6f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2f6f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f2f6f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f2f6f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2f6f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f2f6f-116">Not supported.</span></span>|
|<span data-ttu-id="f2f6f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f2f6f-117">Application</span></span>|<span data-ttu-id="f2f6f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2f6f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2f6f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f2f6f-119">HTTP Request</span></span>
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
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/userStatuses/{deviceConfigurationUserStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="f2f6f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f2f6f-120">Request headers</span></span>
|<span data-ttu-id="f2f6f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f2f6f-121">Header</span></span>|<span data-ttu-id="f2f6f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f2f6f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f2f6f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f2f6f-123">Authorization</span></span>|<span data-ttu-id="f2f6f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f2f6f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f2f6f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f2f6f-125">Accept</span></span>|<span data-ttu-id="f2f6f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f2f6f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2f6f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f2f6f-127">Request body</span></span>
<span data-ttu-id="f2f6f-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="f2f6f-128">In the request body, supply a JSON representation for the [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object.</span></span>

<span data-ttu-id="f2f6f-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="f2f6f-129">The following table shows the properties that are required when you create the [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span></span>

|<span data-ttu-id="f2f6f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f2f6f-130">Property</span></span>|<span data-ttu-id="f2f6f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f2f6f-131">Type</span></span>|<span data-ttu-id="f2f6f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2f6f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2f6f-133">id</span><span class="sxs-lookup"><span data-stu-id="f2f6f-133">id</span></span>|<span data-ttu-id="f2f6f-134">String</span><span class="sxs-lookup"><span data-stu-id="f2f6f-134">String</span></span>|<span data-ttu-id="f2f6f-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f2f6f-135">Key of the entity.</span></span>|
|<span data-ttu-id="f2f6f-136">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="f2f6f-136">userDisplayName</span></span>|<span data-ttu-id="f2f6f-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2f6f-137">String</span></span>|<span data-ttu-id="f2f6f-138">Nome de usuário de DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="f2f6f-138">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="f2f6f-139">devicesCount</span><span class="sxs-lookup"><span data-stu-id="f2f6f-139">devicesCount</span></span>|<span data-ttu-id="f2f6f-140">Int32</span><span class="sxs-lookup"><span data-stu-id="f2f6f-140">Int32</span></span>|<span data-ttu-id="f2f6f-141">Contagem de dispositivos para esse usuário.</span><span class="sxs-lookup"><span data-stu-id="f2f6f-141">Devices count for that user.</span></span>|
|<span data-ttu-id="f2f6f-142">status</span><span class="sxs-lookup"><span data-stu-id="f2f6f-142">status</span></span>|[<span data-ttu-id="f2f6f-143">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="f2f6f-143">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="f2f6f-144">Status de conformidade do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="f2f6f-144">Compliance status of the policy report.</span></span> <span data-ttu-id="f2f6f-145">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="f2f6f-145">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="f2f6f-146">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="f2f6f-146">lastReportedDateTime</span></span>|<span data-ttu-id="f2f6f-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2f6f-147">DateTimeOffset</span></span>|<span data-ttu-id="f2f6f-148">Data e hora da última modificação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="f2f6f-148">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="f2f6f-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f2f6f-149">userPrincipalName</span></span>|<span data-ttu-id="f2f6f-150">String</span><span class="sxs-lookup"><span data-stu-id="f2f6f-150">String</span></span>|<span data-ttu-id="f2f6f-151">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="f2f6f-151">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="f2f6f-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2f6f-152">Response</span></span>
<span data-ttu-id="f2f6f-153">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f2f6f-153">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2f6f-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f2f6f-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="f2f6f-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f2f6f-155">Request</span></span>
<span data-ttu-id="f2f6f-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f2f6f-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f2f6f-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2f6f-157">Response</span></span>
<span data-ttu-id="f2f6f-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f2f6f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





