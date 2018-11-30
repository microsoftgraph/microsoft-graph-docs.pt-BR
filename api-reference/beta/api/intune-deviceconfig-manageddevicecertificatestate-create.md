---
title: Criar managedDeviceCertificateState
description: Crie um novo objeto de managedDeviceCertificateState.
ms.openlocfilehash: 7369b6d4eb8c5639fd928c5ff2be46b9db8dc10e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037958"
---
# <a name="create-manageddevicecertificatestate"></a><span data-ttu-id="685db-103">Criar managedDeviceCertificateState</span><span class="sxs-lookup"><span data-stu-id="685db-103">Create managedDeviceCertificateState</span></span>

> <span data-ttu-id="685db-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="685db-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="685db-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="685db-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="685db-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="685db-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="685db-107">Crie um novo objeto de [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="685db-107">Create a new [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="685db-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="685db-108">Prerequisites</span></span>
<span data-ttu-id="685db-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="685db-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="685db-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="685db-111">Permission type</span></span>|<span data-ttu-id="685db-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="685db-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="685db-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="685db-113">Delegated (work or school account)</span></span>|<span data-ttu-id="685db-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="685db-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="685db-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="685db-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="685db-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="685db-116">Not supported.</span></span>|
|<span data-ttu-id="685db-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="685db-117">Application</span></span>|<span data-ttu-id="685db-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="685db-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="685db-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="685db-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidPkcsCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidScepCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosImportedPFXCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSImportedPFXCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidImportedPFXCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfileScepCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidForWorkImportedPFXCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkPkcsCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkScepCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/microsoft.graph.windowsPhone81SCEPCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10PkcsCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows81SCEPCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10ImportedPFXCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windowsPhone81ImportedPFXCertificateProfile/managedDeviceCertificateStates
```

## <a name="request-headers"></a><span data-ttu-id="685db-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="685db-120">Request headers</span></span>
|<span data-ttu-id="685db-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="685db-121">Header</span></span>|<span data-ttu-id="685db-122">Valor</span><span class="sxs-lookup"><span data-stu-id="685db-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="685db-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="685db-123">Authorization</span></span>|<span data-ttu-id="685db-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="685db-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="685db-125">Accept</span><span class="sxs-lookup"><span data-stu-id="685db-125">Accept</span></span>|<span data-ttu-id="685db-126">application/json</span><span class="sxs-lookup"><span data-stu-id="685db-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="685db-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="685db-127">Request body</span></span>
<span data-ttu-id="685db-128">No corpo da solicitação, fornece uma representação JSON para o objeto managedDeviceCertificateState.</span><span class="sxs-lookup"><span data-stu-id="685db-128">In the request body, supply a JSON representation for the managedDeviceCertificateState object.</span></span>

<span data-ttu-id="685db-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o managedDeviceCertificateState.</span><span class="sxs-lookup"><span data-stu-id="685db-129">The following table shows the properties that are required when you create the managedDeviceCertificateState.</span></span>

|<span data-ttu-id="685db-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="685db-130">Property</span></span>|<span data-ttu-id="685db-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="685db-131">Type</span></span>|<span data-ttu-id="685db-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="685db-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="685db-133">id</span><span class="sxs-lookup"><span data-stu-id="685db-133">id</span></span>|<span data-ttu-id="685db-134">String</span><span class="sxs-lookup"><span data-stu-id="685db-134">String</span></span>|<span data-ttu-id="685db-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="685db-135">Key of the entity.</span></span>|
|<span data-ttu-id="685db-136">devicePlatform</span><span class="sxs-lookup"><span data-stu-id="685db-136">devicePlatform</span></span>|[<span data-ttu-id="685db-137">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="685db-137">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="685db-138">Plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="685db-138">Device platform.</span></span> <span data-ttu-id="685db-139">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span><span class="sxs-lookup"><span data-stu-id="685db-139">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|
|<span data-ttu-id="685db-140">certificateKeyUsage</span><span class="sxs-lookup"><span data-stu-id="685db-140">certificateKeyUsage</span></span>|[<span data-ttu-id="685db-141">keyUsages</span><span class="sxs-lookup"><span data-stu-id="685db-141">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="685db-142">Uso da chave.</span><span class="sxs-lookup"><span data-stu-id="685db-142">Key usage.</span></span> <span data-ttu-id="685db-143">Os valores possíveis são: `keyEncipherment` e `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="685db-143">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="685db-144">certificateValidityPeriodUnits</span><span class="sxs-lookup"><span data-stu-id="685db-144">certificateValidityPeriodUnits</span></span>|[<span data-ttu-id="685db-145">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="685db-145">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="685db-146">Unidades do período de validade.</span><span class="sxs-lookup"><span data-stu-id="685db-146">Validity period units.</span></span> <span data-ttu-id="685db-147">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="685db-147">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="685db-148">certificateIssuanceState</span><span class="sxs-lookup"><span data-stu-id="685db-148">certificateIssuanceState</span></span>|[<span data-ttu-id="685db-149">certificateIssuanceStates</span><span class="sxs-lookup"><span data-stu-id="685db-149">certificateIssuanceStates</span></span>](../resources/intune-deviceconfig-certificateissuancestates.md)|<span data-ttu-id="685db-150">Estado de emissão.</span><span class="sxs-lookup"><span data-stu-id="685db-150">Issuance State.</span></span> <span data-ttu-id="685db-151">Os valores possíveis são: `unknown`, `challengeIssued`, `challengeIssueFailed`, `requestCreationFailed`, `requestSubmitFailed`, `challengeValidationSucceeded`, `challengeValidationFailed`, `issueFailed`, `issuePending`, `issued`, `responseProcessingFailed`, `responsePending`, `enrollmentSucceeded`, `enrollmentNotNeeded`, `revoked`, `removedFromCollection`, `renewVerified`, `installFailed`, `installed` , `deleteFailed`, `deleted`, `renewalRequested`, `requested`.</span><span class="sxs-lookup"><span data-stu-id="685db-151">Possible values are: `unknown`, `challengeIssued`, `challengeIssueFailed`, `requestCreationFailed`, `requestSubmitFailed`, `challengeValidationSucceeded`, `challengeValidationFailed`, `issueFailed`, `issuePending`, `issued`, `responseProcessingFailed`, `responsePending`, `enrollmentSucceeded`, `enrollmentNotNeeded`, `revoked`, `removedFromCollection`, `renewVerified`, `installFailed`, `installed`, `deleteFailed`, `deleted`, `renewalRequested`, `requested`.</span></span>|
|<span data-ttu-id="685db-152">certificateKeyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="685db-152">certificateKeyStorageProvider</span></span>|[<span data-ttu-id="685db-153">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="685db-153">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="685db-154">Provedor de armazenamento de chave.</span><span class="sxs-lookup"><span data-stu-id="685db-154">Key Storage Provider.</span></span> <span data-ttu-id="685db-155">Os valores possíveis são: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="685db-155">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="685db-156">certificateSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="685db-156">certificateSubjectNameFormat</span></span>|[<span data-ttu-id="685db-157">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="685db-157">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="685db-158">Formato de nome de entidade.</span><span class="sxs-lookup"><span data-stu-id="685db-158">Subject name format.</span></span> <span data-ttu-id="685db-159">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="685db-159">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="685db-160">certificateSubjectAlternativeNameFormat</span><span class="sxs-lookup"><span data-stu-id="685db-160">certificateSubjectAlternativeNameFormat</span></span>|[<span data-ttu-id="685db-161">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="685db-161">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="685db-162">Formato de nome alternativo da entidade.</span><span class="sxs-lookup"><span data-stu-id="685db-162">Subject alternative name format.</span></span> <span data-ttu-id="685db-163">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="685db-163">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="685db-164">certificateRevokeStatus</span><span class="sxs-lookup"><span data-stu-id="685db-164">certificateRevokeStatus</span></span>|[<span data-ttu-id="685db-165">certificateRevocationStatus</span><span class="sxs-lookup"><span data-stu-id="685db-165">certificateRevocationStatus</span></span>](../resources/intune-deviceconfig-certificaterevocationstatus.md)|<span data-ttu-id="685db-166">Revogar o status.</span><span class="sxs-lookup"><span data-stu-id="685db-166">Revoke status.</span></span> <span data-ttu-id="685db-167">Os valores possíveis são: `none`, `pending`, `issued`, `failed`, `revoked`.</span><span class="sxs-lookup"><span data-stu-id="685db-167">Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.</span></span>|
|<span data-ttu-id="685db-168">certificateProfileDisplayName</span><span class="sxs-lookup"><span data-stu-id="685db-168">certificateProfileDisplayName</span></span>|<span data-ttu-id="685db-169">String</span><span class="sxs-lookup"><span data-stu-id="685db-169">String</span></span>|<span data-ttu-id="685db-170">Nome de exibição de perfil de certificado</span><span class="sxs-lookup"><span data-stu-id="685db-170">Certificate profile display name</span></span>|
|<span data-ttu-id="685db-171">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="685db-171">deviceDisplayName</span></span>|<span data-ttu-id="685db-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="685db-172">String</span></span>|<span data-ttu-id="685db-173">Nome de exibição do dispositivo</span><span class="sxs-lookup"><span data-stu-id="685db-173">Device display name</span></span>|
|<span data-ttu-id="685db-174">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="685db-174">userDisplayName</span></span>|<span data-ttu-id="685db-175">String</span><span class="sxs-lookup"><span data-stu-id="685db-175">String</span></span>|<span data-ttu-id="685db-176">Nome de exibição do usuário</span><span class="sxs-lookup"><span data-stu-id="685db-176">User display name</span></span>|
|<span data-ttu-id="685db-177">certificateExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="685db-177">certificateExpirationDateTime</span></span>|<span data-ttu-id="685db-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="685db-178">DateTimeOffset</span></span>|<span data-ttu-id="685db-179">Data de expiração de certificado</span><span class="sxs-lookup"><span data-stu-id="685db-179">Certificate expiry date</span></span>|
|<span data-ttu-id="685db-180">certificateLastIssuanceStateChangedDateTime</span><span class="sxs-lookup"><span data-stu-id="685db-180">certificateLastIssuanceStateChangedDateTime</span></span>|<span data-ttu-id="685db-181">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="685db-181">DateTimeOffset</span></span>|<span data-ttu-id="685db-182">Última alteração de estado de emissão de certificado</span><span class="sxs-lookup"><span data-stu-id="685db-182">Last certificate issuance state change</span></span>|
|<span data-ttu-id="685db-183">lastCertificateStateChangeDateTime</span><span class="sxs-lookup"><span data-stu-id="685db-183">lastCertificateStateChangeDateTime</span></span>|<span data-ttu-id="685db-184">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="685db-184">DateTimeOffset</span></span>|<span data-ttu-id="685db-185">Última alteração de estado de emissão de certificado</span><span class="sxs-lookup"><span data-stu-id="685db-185">Last certificate issuance state change</span></span>|
|<span data-ttu-id="685db-186">certificateIssuer</span><span class="sxs-lookup"><span data-stu-id="685db-186">certificateIssuer</span></span>|<span data-ttu-id="685db-187">String</span><span class="sxs-lookup"><span data-stu-id="685db-187">String</span></span>|<span data-ttu-id="685db-188">Emissor</span><span class="sxs-lookup"><span data-stu-id="685db-188">Issuer</span></span>|
|<span data-ttu-id="685db-189">certificateThumbprint</span><span class="sxs-lookup"><span data-stu-id="685db-189">certificateThumbprint</span></span>|<span data-ttu-id="685db-190">String</span><span class="sxs-lookup"><span data-stu-id="685db-190">String</span></span>|<span data-ttu-id="685db-191">Impressão digital</span><span class="sxs-lookup"><span data-stu-id="685db-191">Thumbprint</span></span>|
|<span data-ttu-id="685db-192">Número_serial_do_certificado</span><span class="sxs-lookup"><span data-stu-id="685db-192">certificateSerialNumber</span></span>|<span data-ttu-id="685db-193">String</span><span class="sxs-lookup"><span data-stu-id="685db-193">String</span></span>|<span data-ttu-id="685db-194">Número de série</span><span class="sxs-lookup"><span data-stu-id="685db-194">Serial number</span></span>|
|<span data-ttu-id="685db-195">certificateKeyLength</span><span class="sxs-lookup"><span data-stu-id="685db-195">certificateKeyLength</span></span>|<span data-ttu-id="685db-196">Int32</span><span class="sxs-lookup"><span data-stu-id="685db-196">Int32</span></span>|<span data-ttu-id="685db-197">Comprimento da chave</span><span class="sxs-lookup"><span data-stu-id="685db-197">Key length</span></span>|
|<span data-ttu-id="685db-198">certificateEnhancedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="685db-198">certificateEnhancedKeyUsage</span></span>|<span data-ttu-id="685db-199">String</span><span class="sxs-lookup"><span data-stu-id="685db-199">String</span></span>|<span data-ttu-id="685db-200">Uso estendido de chave</span><span class="sxs-lookup"><span data-stu-id="685db-200">Extended key usage</span></span>|
|<span data-ttu-id="685db-201">certificateValidityPeriod</span><span class="sxs-lookup"><span data-stu-id="685db-201">certificateValidityPeriod</span></span>|<span data-ttu-id="685db-202">Int32</span><span class="sxs-lookup"><span data-stu-id="685db-202">Int32</span></span>|<span data-ttu-id="685db-203">Período de validade</span><span class="sxs-lookup"><span data-stu-id="685db-203">Validity period</span></span>|
|<span data-ttu-id="685db-204">certificateSubjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="685db-204">certificateSubjectNameFormatString</span></span>|<span data-ttu-id="685db-205">String</span><span class="sxs-lookup"><span data-stu-id="685db-205">String</span></span>|<span data-ttu-id="685db-206">Sequência de formato de nome de entidade para formatos de nome de entidade personalizada</span><span class="sxs-lookup"><span data-stu-id="685db-206">Subject name format string for custom subject name formats</span></span>|
|<span data-ttu-id="685db-207">certificateSubjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="685db-207">certificateSubjectAlternativeNameFormatString</span></span>|<span data-ttu-id="685db-208">String</span><span class="sxs-lookup"><span data-stu-id="685db-208">String</span></span>|<span data-ttu-id="685db-209">Sequência de formato de nome alternativo de entidade para formatos personalizados</span><span class="sxs-lookup"><span data-stu-id="685db-209">Subject alternative name format string for custom formats</span></span>|
|<span data-ttu-id="685db-210">certificateIssuanceDateTime</span><span class="sxs-lookup"><span data-stu-id="685db-210">certificateIssuanceDateTime</span></span>|<span data-ttu-id="685db-211">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="685db-211">DateTimeOffset</span></span>|<span data-ttu-id="685db-212">Data de emissão</span><span class="sxs-lookup"><span data-stu-id="685db-212">Issuance date</span></span>|
|<span data-ttu-id="685db-213">certificateErrorCode</span><span class="sxs-lookup"><span data-stu-id="685db-213">certificateErrorCode</span></span>|<span data-ttu-id="685db-214">Int32</span><span class="sxs-lookup"><span data-stu-id="685db-214">Int32</span></span>|<span data-ttu-id="685db-215">Código de erro</span><span class="sxs-lookup"><span data-stu-id="685db-215">Error code</span></span>|



## <a name="response"></a><span data-ttu-id="685db-216">Resposta</span><span class="sxs-lookup"><span data-stu-id="685db-216">Response</span></span>
<span data-ttu-id="685db-217">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="685db-217">If successful, this method returns a `201 Created` response code and a [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="685db-218">Exemplo</span><span class="sxs-lookup"><span data-stu-id="685db-218">Example</span></span>
### <a name="request"></a><span data-ttu-id="685db-219">Solicitação</span><span class="sxs-lookup"><span data-stu-id="685db-219">Request</span></span>
<span data-ttu-id="685db-220">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="685db-220">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="685db-221">Resposta</span><span class="sxs-lookup"><span data-stu-id="685db-221">Response</span></span>
<span data-ttu-id="685db-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="685db-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





