---
title: Criar deviceConfigurationUserStatus
description: Criar um novo objeto deviceConfigurationUserStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 996e470c97ace1ba56f0a695ff22226e19628e62
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27948300"
---
# <a name="create-deviceconfigurationuserstatus"></a><span data-ttu-id="5ee8a-103">Criar deviceConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="5ee8a-103">Create deviceConfigurationUserStatus</span></span>

> <span data-ttu-id="5ee8a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5ee8a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5ee8a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5ee8a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5ee8a-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="5ee8a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5ee8a-107">Criar um novo objeto [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="5ee8a-107">Create a new [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5ee8a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5ee8a-108">Prerequisites</span></span>
<span data-ttu-id="5ee8a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ee8a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ee8a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5ee8a-111">Permission type</span></span>|<span data-ttu-id="5ee8a-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5ee8a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5ee8a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5ee8a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5ee8a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ee8a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5ee8a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5ee8a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5ee8a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ee8a-116">Not supported.</span></span>|
|<span data-ttu-id="5ee8a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5ee8a-117">Application</span></span>|<span data-ttu-id="5ee8a-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ee8a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5ee8a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5ee8a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/userStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/userStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/userStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/userStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/userStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/userStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/userStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="5ee8a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5ee8a-120">Request headers</span></span>
|<span data-ttu-id="5ee8a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5ee8a-121">Header</span></span>|<span data-ttu-id="5ee8a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5ee8a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5ee8a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5ee8a-123">Authorization</span></span>|<span data-ttu-id="5ee8a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5ee8a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5ee8a-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5ee8a-125">Accept</span></span>|<span data-ttu-id="5ee8a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5ee8a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ee8a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5ee8a-127">Request body</span></span>
<span data-ttu-id="5ee8a-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceConfigurationUserStatus.</span><span class="sxs-lookup"><span data-stu-id="5ee8a-128">In the request body, supply a JSON representation for the deviceConfigurationUserStatus object.</span></span>

<span data-ttu-id="5ee8a-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceConfigurationUserStatus.</span><span class="sxs-lookup"><span data-stu-id="5ee8a-129">The following table shows the properties that are required when you create the deviceConfigurationUserStatus.</span></span>

|<span data-ttu-id="5ee8a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5ee8a-130">Property</span></span>|<span data-ttu-id="5ee8a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="5ee8a-131">Type</span></span>|<span data-ttu-id="5ee8a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ee8a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ee8a-133">id</span><span class="sxs-lookup"><span data-stu-id="5ee8a-133">id</span></span>|<span data-ttu-id="5ee8a-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5ee8a-134">String</span></span>|<span data-ttu-id="5ee8a-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="5ee8a-135">Key of the entity.</span></span>|
|<span data-ttu-id="5ee8a-136">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="5ee8a-136">userDisplayName</span></span>|<span data-ttu-id="5ee8a-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5ee8a-137">String</span></span>|<span data-ttu-id="5ee8a-138">Nome de usuário de DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="5ee8a-138">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="5ee8a-139">devicesCount</span><span class="sxs-lookup"><span data-stu-id="5ee8a-139">devicesCount</span></span>|<span data-ttu-id="5ee8a-140">Int32</span><span class="sxs-lookup"><span data-stu-id="5ee8a-140">Int32</span></span>|<span data-ttu-id="5ee8a-141">Contagem de dispositivos para esse usuário.</span><span class="sxs-lookup"><span data-stu-id="5ee8a-141">Devices count for that user.</span></span>|
|<span data-ttu-id="5ee8a-142">status</span><span class="sxs-lookup"><span data-stu-id="5ee8a-142">status</span></span>|[<span data-ttu-id="5ee8a-143">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="5ee8a-143">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="5ee8a-144">Status de conformidade do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="5ee8a-144">Compliance status of the policy report.</span></span> <span data-ttu-id="5ee8a-145">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="5ee8a-145">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="5ee8a-146">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="5ee8a-146">lastReportedDateTime</span></span>|<span data-ttu-id="5ee8a-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ee8a-147">DateTimeOffset</span></span>|<span data-ttu-id="5ee8a-148">Data e hora da última modificação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="5ee8a-148">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="5ee8a-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5ee8a-149">userPrincipalName</span></span>|<span data-ttu-id="5ee8a-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5ee8a-150">String</span></span>|<span data-ttu-id="5ee8a-151">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="5ee8a-151">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="5ee8a-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ee8a-152">Response</span></span>
<span data-ttu-id="5ee8a-153">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5ee8a-153">If successful, this method returns a `201 Created` response code and a [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ee8a-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5ee8a-154">Example</span></span>
### <a name="request"></a><span data-ttu-id="5ee8a-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ee8a-155">Request</span></span>
<span data-ttu-id="5ee8a-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5ee8a-156">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses
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

### <a name="response"></a><span data-ttu-id="5ee8a-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ee8a-157">Response</span></span>
<span data-ttu-id="5ee8a-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5ee8a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





