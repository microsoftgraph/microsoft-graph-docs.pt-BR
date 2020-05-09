---
title: Criar managedDeviceCertificateState
description: Criar um novo objeto managedDeviceCertificateState.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 914285da1e6934df509c43e53d5e99cb0acbd24d
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/09/2020
ms.locfileid: "44177839"
---
# <a name="create-manageddevicecertificatestate"></a><span data-ttu-id="abbee-103">Criar managedDeviceCertificateState</span><span class="sxs-lookup"><span data-stu-id="abbee-103">Create managedDeviceCertificateState</span></span>

<span data-ttu-id="abbee-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="abbee-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="abbee-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="abbee-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="abbee-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="abbee-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="abbee-107">Criar um novo objeto [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="abbee-107">Create a new [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="abbee-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="abbee-108">Prerequisites</span></span>
<span data-ttu-id="abbee-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="abbee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="abbee-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="abbee-111">Permission type</span></span>|<span data-ttu-id="abbee-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="abbee-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="abbee-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="abbee-113">Delegated (work or school account)</span></span>|<span data-ttu-id="abbee-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="abbee-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="abbee-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="abbee-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="abbee-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="abbee-116">Not supported.</span></span>|
|<span data-ttu-id="abbee-117">Application</span><span class="sxs-lookup"><span data-stu-id="abbee-117">Application</span></span>|<span data-ttu-id="abbee-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="abbee-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="abbee-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="abbee-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidPkcsCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidScepCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosImportedPFXCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidImportedPFXCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerScepCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidForWorkImportedPFXCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerImportedPFXCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkPkcsCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkScepCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidWorkProfilePkcsCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidWorkProfileScepCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/microsoft.graph.windowsPhone81SCEPCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/microsoft.graph.macOSPkcsCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/microsoft.graph.macOSScepCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/microsoft.graph.macOSImportedPFXCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10PkcsCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows81SCEPCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10ImportedPFXCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windowsPhone81ImportedPFXCertificateProfile/managedDeviceCertificateStates
```

## <a name="request-headers"></a><span data-ttu-id="abbee-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="abbee-120">Request headers</span></span>
|<span data-ttu-id="abbee-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="abbee-121">Header</span></span>|<span data-ttu-id="abbee-122">Valor</span><span class="sxs-lookup"><span data-stu-id="abbee-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="abbee-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="abbee-123">Authorization</span></span>|<span data-ttu-id="abbee-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="abbee-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="abbee-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="abbee-125">Accept</span></span>|<span data-ttu-id="abbee-126">application/json</span><span class="sxs-lookup"><span data-stu-id="abbee-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="abbee-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="abbee-127">Request body</span></span>
<span data-ttu-id="abbee-128">No corpo da solicitação, forneça uma representação JSON do objeto managedDeviceCertificateState.</span><span class="sxs-lookup"><span data-stu-id="abbee-128">In the request body, supply a JSON representation for the managedDeviceCertificateState object.</span></span>

<span data-ttu-id="abbee-129">A tabela a seguir mostra as propriedades que são necessárias ao criar managedDeviceCertificateState.</span><span class="sxs-lookup"><span data-stu-id="abbee-129">The following table shows the properties that are required when you create the managedDeviceCertificateState.</span></span>

|<span data-ttu-id="abbee-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="abbee-130">Property</span></span>|<span data-ttu-id="abbee-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="abbee-131">Type</span></span>|<span data-ttu-id="abbee-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="abbee-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="abbee-133">id</span><span class="sxs-lookup"><span data-stu-id="abbee-133">id</span></span>|<span data-ttu-id="abbee-134">String</span><span class="sxs-lookup"><span data-stu-id="abbee-134">String</span></span>|<span data-ttu-id="abbee-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="abbee-135">Key of the entity.</span></span>|
|<span data-ttu-id="abbee-136">devicePlatform</span><span class="sxs-lookup"><span data-stu-id="abbee-136">devicePlatform</span></span>|[<span data-ttu-id="abbee-137">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="abbee-137">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="abbee-138">Plataforma de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="abbee-138">Device platform.</span></span> <span data-ttu-id="abbee-139">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="abbee-139">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="abbee-140">certificateKeyUsage</span><span class="sxs-lookup"><span data-stu-id="abbee-140">certificateKeyUsage</span></span>|[<span data-ttu-id="abbee-141">usos de</span><span class="sxs-lookup"><span data-stu-id="abbee-141">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="abbee-142">Uso de chave.</span><span class="sxs-lookup"><span data-stu-id="abbee-142">Key usage.</span></span> <span data-ttu-id="abbee-143">Os valores possíveis são: `keyEncipherment` e `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="abbee-143">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="abbee-144">certificateValidityPeriodUnits</span><span class="sxs-lookup"><span data-stu-id="abbee-144">certificateValidityPeriodUnits</span></span>|[<span data-ttu-id="abbee-145">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="abbee-145">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="abbee-146">Unidades de período de validade.</span><span class="sxs-lookup"><span data-stu-id="abbee-146">Validity period units.</span></span> <span data-ttu-id="abbee-147">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="abbee-147">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="abbee-148">certificateIssuanceState</span><span class="sxs-lookup"><span data-stu-id="abbee-148">certificateIssuanceState</span></span>|[<span data-ttu-id="abbee-149">certificateIssuanceStates</span><span class="sxs-lookup"><span data-stu-id="abbee-149">certificateIssuanceStates</span></span>](../resources/intune-deviceconfig-certificateissuancestates.md)|<span data-ttu-id="abbee-150">Estado de emissão.</span><span class="sxs-lookup"><span data-stu-id="abbee-150">Issuance State.</span></span> <span data-ttu-id="abbee-151">Os valores possíveis são `unknown`: `challengeIssued`, `challengeIssueFailed`, `requestCreationFailed`, `requestSubmitFailed` `challengeValidationSucceeded` `challengeValidationFailed`,,, `issueFailed`, `issuePending`, `issued` `responseProcessingFailed` `responsePending`,,, `enrollmentSucceeded`, `enrollmentNotNeeded`, `revoked`, `removedFromCollection`, `renewVerified`, `installFailed`, `installed` `deleteFailed` `deleted` `renewalRequested`,,,, `requested`,,,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="abbee-151">Possible values are: `unknown`, `challengeIssued`, `challengeIssueFailed`, `requestCreationFailed`, `requestSubmitFailed`, `challengeValidationSucceeded`, `challengeValidationFailed`, `issueFailed`, `issuePending`, `issued`, `responseProcessingFailed`, `responsePending`, `enrollmentSucceeded`, `enrollmentNotNeeded`, `revoked`, `removedFromCollection`, `renewVerified`, `installFailed`, `installed`, `deleteFailed`, `deleted`, `renewalRequested`, `requested`.</span></span>|
|<span data-ttu-id="abbee-152">certificateKeyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="abbee-152">certificateKeyStorageProvider</span></span>|[<span data-ttu-id="abbee-153">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="abbee-153">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="abbee-154">Provedor de armazenamento de chave.</span><span class="sxs-lookup"><span data-stu-id="abbee-154">Key Storage Provider.</span></span> <span data-ttu-id="abbee-155">Os valores possíveis são: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="abbee-155">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="abbee-156">certificateSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="abbee-156">certificateSubjectNameFormat</span></span>|[<span data-ttu-id="abbee-157">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="abbee-157">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="abbee-158">Formato do nome da entidade.</span><span class="sxs-lookup"><span data-stu-id="abbee-158">Subject name format.</span></span> <span data-ttu-id="abbee-159">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="abbee-159">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="abbee-160">certificateSubjectAlternativeNameFormat</span><span class="sxs-lookup"><span data-stu-id="abbee-160">certificateSubjectAlternativeNameFormat</span></span>|[<span data-ttu-id="abbee-161">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="abbee-161">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="abbee-162">Formato de nome alternativo da entidade.</span><span class="sxs-lookup"><span data-stu-id="abbee-162">Subject alternative name format.</span></span> <span data-ttu-id="abbee-163">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="abbee-163">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="abbee-164">certificateRevokeStatus</span><span class="sxs-lookup"><span data-stu-id="abbee-164">certificateRevokeStatus</span></span>|[<span data-ttu-id="abbee-165">certificateRevocationStatus</span><span class="sxs-lookup"><span data-stu-id="abbee-165">certificateRevocationStatus</span></span>](../resources/intune-deviceconfig-certificaterevocationstatus.md)|<span data-ttu-id="abbee-166">Revogar status.</span><span class="sxs-lookup"><span data-stu-id="abbee-166">Revoke status.</span></span> <span data-ttu-id="abbee-167">Os valores possíveis são: `none`, `pending`, `issued`, `failed`, `revoked`.</span><span class="sxs-lookup"><span data-stu-id="abbee-167">Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.</span></span>|
|<span data-ttu-id="abbee-168">certificateProfileDisplayName</span><span class="sxs-lookup"><span data-stu-id="abbee-168">certificateProfileDisplayName</span></span>|<span data-ttu-id="abbee-169">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="abbee-169">String</span></span>|<span data-ttu-id="abbee-170">Nome de exibição do perfil do certificado</span><span class="sxs-lookup"><span data-stu-id="abbee-170">Certificate profile display name</span></span>|
|<span data-ttu-id="abbee-171">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="abbee-171">deviceDisplayName</span></span>|<span data-ttu-id="abbee-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="abbee-172">String</span></span>|<span data-ttu-id="abbee-173">Nome de exibição do dispositivo</span><span class="sxs-lookup"><span data-stu-id="abbee-173">Device display name</span></span>|
|<span data-ttu-id="abbee-174">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="abbee-174">userDisplayName</span></span>|<span data-ttu-id="abbee-175">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="abbee-175">String</span></span>|<span data-ttu-id="abbee-176">Nome de exibição do usuário</span><span class="sxs-lookup"><span data-stu-id="abbee-176">User display name</span></span>|
|<span data-ttu-id="abbee-177">certificateExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="abbee-177">certificateExpirationDateTime</span></span>|<span data-ttu-id="abbee-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="abbee-178">DateTimeOffset</span></span>|<span data-ttu-id="abbee-179">Data de vencimento do certificado</span><span class="sxs-lookup"><span data-stu-id="abbee-179">Certificate expiry date</span></span>|
|<span data-ttu-id="abbee-180">certificateLastIssuanceStateChangedDateTime</span><span class="sxs-lookup"><span data-stu-id="abbee-180">certificateLastIssuanceStateChangedDateTime</span></span>|<span data-ttu-id="abbee-181">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="abbee-181">DateTimeOffset</span></span>|<span data-ttu-id="abbee-182">Última alteração no estado de emissão de certificado</span><span class="sxs-lookup"><span data-stu-id="abbee-182">Last certificate issuance state change</span></span>|
|<span data-ttu-id="abbee-183">lastCertificateStateChangeDateTime</span><span class="sxs-lookup"><span data-stu-id="abbee-183">lastCertificateStateChangeDateTime</span></span>|<span data-ttu-id="abbee-184">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="abbee-184">DateTimeOffset</span></span>|<span data-ttu-id="abbee-185">Última alteração no estado de emissão de certificado</span><span class="sxs-lookup"><span data-stu-id="abbee-185">Last certificate issuance state change</span></span>|
|<span data-ttu-id="abbee-186">certificateIssuer</span><span class="sxs-lookup"><span data-stu-id="abbee-186">certificateIssuer</span></span>|<span data-ttu-id="abbee-187">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="abbee-187">String</span></span>|<span data-ttu-id="abbee-188">Emissor</span><span class="sxs-lookup"><span data-stu-id="abbee-188">Issuer</span></span>|
|<span data-ttu-id="abbee-189">certificateThumbprint</span><span class="sxs-lookup"><span data-stu-id="abbee-189">certificateThumbprint</span></span>|<span data-ttu-id="abbee-190">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="abbee-190">String</span></span>|<span data-ttu-id="abbee-191">Identificação</span><span class="sxs-lookup"><span data-stu-id="abbee-191">Thumbprint</span></span>|
|<span data-ttu-id="abbee-192">certificateSerialNumber</span><span class="sxs-lookup"><span data-stu-id="abbee-192">certificateSerialNumber</span></span>|<span data-ttu-id="abbee-193">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="abbee-193">String</span></span>|<span data-ttu-id="abbee-194">Número de série</span><span class="sxs-lookup"><span data-stu-id="abbee-194">Serial number</span></span>|
|<span data-ttu-id="abbee-195">certificateKeyLength</span><span class="sxs-lookup"><span data-stu-id="abbee-195">certificateKeyLength</span></span>|<span data-ttu-id="abbee-196">Int32</span><span class="sxs-lookup"><span data-stu-id="abbee-196">Int32</span></span>|<span data-ttu-id="abbee-197">Comprimento de chave</span><span class="sxs-lookup"><span data-stu-id="abbee-197">Key length</span></span>|
|<span data-ttu-id="abbee-198">certificateEnhancedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="abbee-198">certificateEnhancedKeyUsage</span></span>|<span data-ttu-id="abbee-199">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="abbee-199">String</span></span>|<span data-ttu-id="abbee-200">Uso estendido de chave</span><span class="sxs-lookup"><span data-stu-id="abbee-200">Extended key usage</span></span>|
|<span data-ttu-id="abbee-201">certificateValidityPeriod</span><span class="sxs-lookup"><span data-stu-id="abbee-201">certificateValidityPeriod</span></span>|<span data-ttu-id="abbee-202">Int32</span><span class="sxs-lookup"><span data-stu-id="abbee-202">Int32</span></span>|<span data-ttu-id="abbee-203">Período de validade</span><span class="sxs-lookup"><span data-stu-id="abbee-203">Validity period</span></span>|
|<span data-ttu-id="abbee-204">certificateSubjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="abbee-204">certificateSubjectNameFormatString</span></span>|<span data-ttu-id="abbee-205">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="abbee-205">String</span></span>|<span data-ttu-id="abbee-206">Cadeia de caracteres de formato de nome de entidade para formatos de nome de entidade personalizados</span><span class="sxs-lookup"><span data-stu-id="abbee-206">Subject name format string for custom subject name formats</span></span>|
|<span data-ttu-id="abbee-207">certificateSubjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="abbee-207">certificateSubjectAlternativeNameFormatString</span></span>|<span data-ttu-id="abbee-208">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="abbee-208">String</span></span>|<span data-ttu-id="abbee-209">Cadeia de caracteres de formato de nome alternativo da entidade para formatos personalizados</span><span class="sxs-lookup"><span data-stu-id="abbee-209">Subject alternative name format string for custom formats</span></span>|
|<span data-ttu-id="abbee-210">certificateIssuanceDateTime</span><span class="sxs-lookup"><span data-stu-id="abbee-210">certificateIssuanceDateTime</span></span>|<span data-ttu-id="abbee-211">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="abbee-211">DateTimeOffset</span></span>|<span data-ttu-id="abbee-212">Data de emissão</span><span class="sxs-lookup"><span data-stu-id="abbee-212">Issuance date</span></span>|
|<span data-ttu-id="abbee-213">certificateErrorCode</span><span class="sxs-lookup"><span data-stu-id="abbee-213">certificateErrorCode</span></span>|<span data-ttu-id="abbee-214">Int32</span><span class="sxs-lookup"><span data-stu-id="abbee-214">Int32</span></span>|<span data-ttu-id="abbee-215">Código de erro</span><span class="sxs-lookup"><span data-stu-id="abbee-215">Error code</span></span>|



## <a name="response"></a><span data-ttu-id="abbee-216">Resposta</span><span class="sxs-lookup"><span data-stu-id="abbee-216">Response</span></span>
<span data-ttu-id="abbee-217">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="abbee-217">If successful, this method returns a `201 Created` response code and a [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="abbee-218">Exemplo</span><span class="sxs-lookup"><span data-stu-id="abbee-218">Example</span></span>

### <a name="request"></a><span data-ttu-id="abbee-219">Solicitação</span><span class="sxs-lookup"><span data-stu-id="abbee-219">Request</span></span>
<span data-ttu-id="abbee-220">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="abbee-220">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates
Content-type: application/json
Content-length: 1517

{
  "@odata.type": "#microsoft.graph.managedDeviceCertificateState",
  "devicePlatform": "androidForWork",
  "certificateKeyUsage": "digitalSignature",
  "certificateValidityPeriodUnits": "months",
  "certificateIssuanceState": "challengeIssued",
  "certificateKeyStorageProvider": "useTpmKspOtherwiseFail",
  "certificateSubjectNameFormat": "commonNameIncludingEmail",
  "certificateSubjectAlternativeNameFormat": "emailAddress",
  "certificateRevokeStatus": "pending",
  "certificateProfileDisplayName": "Certificate Profile Display Name value",
  "deviceDisplayName": "Device Display Name value",
  "userDisplayName": "User Display Name value",
  "certificateExpirationDateTime": "2017-01-01T00:02:14.9489247-08:00",
  "certificateLastIssuanceStateChangedDateTime": "2017-01-01T00:00:27.7468732-08:00",
  "lastCertificateStateChangeDateTime": "2017-01-01T00:01:10.7144639-08:00",
  "certificateIssuer": "Certificate Issuer value",
  "certificateThumbprint": "Certificate Thumbprint value",
  "certificateSerialNumber": "Certificate Serial Number value",
  "certificateKeyLength": 4,
  "certificateEnhancedKeyUsage": "Certificate Enhanced Key Usage value",
  "certificateValidityPeriod": 9,
  "certificateSubjectNameFormatString": "Certificate Subject Name Format String value",
  "certificateSubjectAlternativeNameFormatString": "Certificate Subject Alternative Name Format String value",
  "certificateIssuanceDateTime": "2016-12-31T23:59:41.5044473-08:00",
  "certificateErrorCode": 4
}
```

### <a name="response"></a><span data-ttu-id="abbee-221">Resposta</span><span class="sxs-lookup"><span data-stu-id="abbee-221">Response</span></span>
<span data-ttu-id="abbee-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="abbee-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1566

{
  "@odata.type": "#microsoft.graph.managedDeviceCertificateState",
  "id": "d99bc884-c884-d99b-84c8-9bd984c89bd9",
  "devicePlatform": "androidForWork",
  "certificateKeyUsage": "digitalSignature",
  "certificateValidityPeriodUnits": "months",
  "certificateIssuanceState": "challengeIssued",
  "certificateKeyStorageProvider": "useTpmKspOtherwiseFail",
  "certificateSubjectNameFormat": "commonNameIncludingEmail",
  "certificateSubjectAlternativeNameFormat": "emailAddress",
  "certificateRevokeStatus": "pending",
  "certificateProfileDisplayName": "Certificate Profile Display Name value",
  "deviceDisplayName": "Device Display Name value",
  "userDisplayName": "User Display Name value",
  "certificateExpirationDateTime": "2017-01-01T00:02:14.9489247-08:00",
  "certificateLastIssuanceStateChangedDateTime": "2017-01-01T00:00:27.7468732-08:00",
  "lastCertificateStateChangeDateTime": "2017-01-01T00:01:10.7144639-08:00",
  "certificateIssuer": "Certificate Issuer value",
  "certificateThumbprint": "Certificate Thumbprint value",
  "certificateSerialNumber": "Certificate Serial Number value",
  "certificateKeyLength": 4,
  "certificateEnhancedKeyUsage": "Certificate Enhanced Key Usage value",
  "certificateValidityPeriod": 9,
  "certificateSubjectNameFormatString": "Certificate Subject Name Format String value",
  "certificateSubjectAlternativeNameFormatString": "Certificate Subject Alternative Name Format String value",
  "certificateIssuanceDateTime": "2016-12-31T23:59:41.5044473-08:00",
  "certificateErrorCode": 4
}
```



