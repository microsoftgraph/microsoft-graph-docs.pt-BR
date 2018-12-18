---
title: Criar managedDeviceCertificateState
description: Crie um novo objeto de managedDeviceCertificateState.
author: tfitzmac
ms.openlocfilehash: 22b8a0db82e86b9136ee997a821223afe608b51a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27305954"
---
# <a name="create-manageddevicecertificatestate"></a><span data-ttu-id="e0e18-103">Criar managedDeviceCertificateState</span><span class="sxs-lookup"><span data-stu-id="e0e18-103">Create managedDeviceCertificateState</span></span>

> <span data-ttu-id="e0e18-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e0e18-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e0e18-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e0e18-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e0e18-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e0e18-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e0e18-107">Crie um novo objeto de [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="e0e18-107">Create a new [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e0e18-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e0e18-108">Prerequisites</span></span>
<span data-ttu-id="e0e18-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0e18-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0e18-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e0e18-111">Permission type</span></span>|<span data-ttu-id="e0e18-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e0e18-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e0e18-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e0e18-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e0e18-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0e18-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e0e18-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e0e18-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e0e18-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e0e18-116">Not supported.</span></span>|
|<span data-ttu-id="e0e18-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e0e18-117">Application</span></span>|<span data-ttu-id="e0e18-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e0e18-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e0e18-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e0e18-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="e0e18-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e0e18-120">Request headers</span></span>
|<span data-ttu-id="e0e18-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e0e18-121">Header</span></span>|<span data-ttu-id="e0e18-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e0e18-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e0e18-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e0e18-123">Authorization</span></span>|<span data-ttu-id="e0e18-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e0e18-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e0e18-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e0e18-125">Accept</span></span>|<span data-ttu-id="e0e18-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e0e18-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0e18-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e0e18-127">Request body</span></span>
<span data-ttu-id="e0e18-128">No corpo da solicitação, fornece uma representação JSON para o objeto managedDeviceCertificateState.</span><span class="sxs-lookup"><span data-stu-id="e0e18-128">In the request body, supply a JSON representation for the managedDeviceCertificateState object.</span></span>

<span data-ttu-id="e0e18-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o managedDeviceCertificateState.</span><span class="sxs-lookup"><span data-stu-id="e0e18-129">The following table shows the properties that are required when you create the managedDeviceCertificateState.</span></span>

|<span data-ttu-id="e0e18-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e0e18-130">Property</span></span>|<span data-ttu-id="e0e18-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e0e18-131">Type</span></span>|<span data-ttu-id="e0e18-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0e18-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0e18-133">id</span><span class="sxs-lookup"><span data-stu-id="e0e18-133">id</span></span>|<span data-ttu-id="e0e18-134">String</span><span class="sxs-lookup"><span data-stu-id="e0e18-134">String</span></span>|<span data-ttu-id="e0e18-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e0e18-135">Key of the entity.</span></span>|
|<span data-ttu-id="e0e18-136">devicePlatform</span><span class="sxs-lookup"><span data-stu-id="e0e18-136">devicePlatform</span></span>|[<span data-ttu-id="e0e18-137">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="e0e18-137">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="e0e18-138">Plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e0e18-138">Device platform.</span></span> <span data-ttu-id="e0e18-139">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span><span class="sxs-lookup"><span data-stu-id="e0e18-139">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|
|<span data-ttu-id="e0e18-140">certificateKeyUsage</span><span class="sxs-lookup"><span data-stu-id="e0e18-140">certificateKeyUsage</span></span>|[<span data-ttu-id="e0e18-141">keyUsages</span><span class="sxs-lookup"><span data-stu-id="e0e18-141">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="e0e18-142">Uso da chave.</span><span class="sxs-lookup"><span data-stu-id="e0e18-142">Key usage.</span></span> <span data-ttu-id="e0e18-143">Os valores possíveis são: `keyEncipherment` e `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="e0e18-143">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="e0e18-144">certificateValidityPeriodUnits</span><span class="sxs-lookup"><span data-stu-id="e0e18-144">certificateValidityPeriodUnits</span></span>|[<span data-ttu-id="e0e18-145">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="e0e18-145">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="e0e18-146">Unidades do período de validade.</span><span class="sxs-lookup"><span data-stu-id="e0e18-146">Validity period units.</span></span> <span data-ttu-id="e0e18-147">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="e0e18-147">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="e0e18-148">certificateIssuanceState</span><span class="sxs-lookup"><span data-stu-id="e0e18-148">certificateIssuanceState</span></span>|[<span data-ttu-id="e0e18-149">certificateIssuanceStates</span><span class="sxs-lookup"><span data-stu-id="e0e18-149">certificateIssuanceStates</span></span>](../resources/intune-deviceconfig-certificateissuancestates.md)|<span data-ttu-id="e0e18-150">Estado de emissão.</span><span class="sxs-lookup"><span data-stu-id="e0e18-150">Issuance State.</span></span> <span data-ttu-id="e0e18-151">Os valores possíveis são: `unknown`, `challengeIssued`, `challengeIssueFailed`, `requestCreationFailed`, `requestSubmitFailed`, `challengeValidationSucceeded`, `challengeValidationFailed`, `issueFailed`, `issuePending`, `issued`, `responseProcessingFailed`, `responsePending`, `enrollmentSucceeded`, `enrollmentNotNeeded`, `revoked`, `removedFromCollection`, `renewVerified`, `installFailed`, `installed` , `deleteFailed`, `deleted`, `renewalRequested`, `requested`.</span><span class="sxs-lookup"><span data-stu-id="e0e18-151">Possible values are: `unknown`, `challengeIssued`, `challengeIssueFailed`, `requestCreationFailed`, `requestSubmitFailed`, `challengeValidationSucceeded`, `challengeValidationFailed`, `issueFailed`, `issuePending`, `issued`, `responseProcessingFailed`, `responsePending`, `enrollmentSucceeded`, `enrollmentNotNeeded`, `revoked`, `removedFromCollection`, `renewVerified`, `installFailed`, `installed`, `deleteFailed`, `deleted`, `renewalRequested`, `requested`.</span></span>|
|<span data-ttu-id="e0e18-152">certificateKeyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="e0e18-152">certificateKeyStorageProvider</span></span>|[<span data-ttu-id="e0e18-153">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="e0e18-153">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="e0e18-154">Provedor de armazenamento de chave.</span><span class="sxs-lookup"><span data-stu-id="e0e18-154">Key Storage Provider.</span></span> <span data-ttu-id="e0e18-155">Os valores possíveis são: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="e0e18-155">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="e0e18-156">certificateSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="e0e18-156">certificateSubjectNameFormat</span></span>|[<span data-ttu-id="e0e18-157">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="e0e18-157">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="e0e18-158">Formato de nome de entidade.</span><span class="sxs-lookup"><span data-stu-id="e0e18-158">Subject name format.</span></span> <span data-ttu-id="e0e18-159">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="e0e18-159">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="e0e18-160">certificateSubjectAlternativeNameFormat</span><span class="sxs-lookup"><span data-stu-id="e0e18-160">certificateSubjectAlternativeNameFormat</span></span>|[<span data-ttu-id="e0e18-161">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="e0e18-161">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="e0e18-162">Formato de nome alternativo da entidade.</span><span class="sxs-lookup"><span data-stu-id="e0e18-162">Subject alternative name format.</span></span> <span data-ttu-id="e0e18-163">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="e0e18-163">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="e0e18-164">certificateRevokeStatus</span><span class="sxs-lookup"><span data-stu-id="e0e18-164">certificateRevokeStatus</span></span>|[<span data-ttu-id="e0e18-165">certificateRevocationStatus</span><span class="sxs-lookup"><span data-stu-id="e0e18-165">certificateRevocationStatus</span></span>](../resources/intune-deviceconfig-certificaterevocationstatus.md)|<span data-ttu-id="e0e18-166">Revogar o status.</span><span class="sxs-lookup"><span data-stu-id="e0e18-166">Revoke status.</span></span> <span data-ttu-id="e0e18-167">Os valores possíveis são: `none`, `pending`, `issued`, `failed`, `revoked`.</span><span class="sxs-lookup"><span data-stu-id="e0e18-167">Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.</span></span>|
|<span data-ttu-id="e0e18-168">certificateProfileDisplayName</span><span class="sxs-lookup"><span data-stu-id="e0e18-168">certificateProfileDisplayName</span></span>|<span data-ttu-id="e0e18-169">String</span><span class="sxs-lookup"><span data-stu-id="e0e18-169">String</span></span>|<span data-ttu-id="e0e18-170">Nome de exibição de perfil de certificado</span><span class="sxs-lookup"><span data-stu-id="e0e18-170">Certificate profile display name</span></span>|
|<span data-ttu-id="e0e18-171">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="e0e18-171">deviceDisplayName</span></span>|<span data-ttu-id="e0e18-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e0e18-172">String</span></span>|<span data-ttu-id="e0e18-173">Nome de exibição do dispositivo</span><span class="sxs-lookup"><span data-stu-id="e0e18-173">Device display name</span></span>|
|<span data-ttu-id="e0e18-174">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="e0e18-174">userDisplayName</span></span>|<span data-ttu-id="e0e18-175">String</span><span class="sxs-lookup"><span data-stu-id="e0e18-175">String</span></span>|<span data-ttu-id="e0e18-176">Nome de exibição do usuário</span><span class="sxs-lookup"><span data-stu-id="e0e18-176">User display name</span></span>|
|<span data-ttu-id="e0e18-177">certificateExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="e0e18-177">certificateExpirationDateTime</span></span>|<span data-ttu-id="e0e18-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0e18-178">DateTimeOffset</span></span>|<span data-ttu-id="e0e18-179">Data de expiração de certificado</span><span class="sxs-lookup"><span data-stu-id="e0e18-179">Certificate expiry date</span></span>|
|<span data-ttu-id="e0e18-180">certificateLastIssuanceStateChangedDateTime</span><span class="sxs-lookup"><span data-stu-id="e0e18-180">certificateLastIssuanceStateChangedDateTime</span></span>|<span data-ttu-id="e0e18-181">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0e18-181">DateTimeOffset</span></span>|<span data-ttu-id="e0e18-182">Última alteração de estado de emissão de certificado</span><span class="sxs-lookup"><span data-stu-id="e0e18-182">Last certificate issuance state change</span></span>|
|<span data-ttu-id="e0e18-183">lastCertificateStateChangeDateTime</span><span class="sxs-lookup"><span data-stu-id="e0e18-183">lastCertificateStateChangeDateTime</span></span>|<span data-ttu-id="e0e18-184">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0e18-184">DateTimeOffset</span></span>|<span data-ttu-id="e0e18-185">Última alteração de estado de emissão de certificado</span><span class="sxs-lookup"><span data-stu-id="e0e18-185">Last certificate issuance state change</span></span>|
|<span data-ttu-id="e0e18-186">certificateIssuer</span><span class="sxs-lookup"><span data-stu-id="e0e18-186">certificateIssuer</span></span>|<span data-ttu-id="e0e18-187">String</span><span class="sxs-lookup"><span data-stu-id="e0e18-187">String</span></span>|<span data-ttu-id="e0e18-188">Emissor</span><span class="sxs-lookup"><span data-stu-id="e0e18-188">Issuer</span></span>|
|<span data-ttu-id="e0e18-189">certificateThumbprint</span><span class="sxs-lookup"><span data-stu-id="e0e18-189">certificateThumbprint</span></span>|<span data-ttu-id="e0e18-190">String</span><span class="sxs-lookup"><span data-stu-id="e0e18-190">String</span></span>|<span data-ttu-id="e0e18-191">Impressão digital</span><span class="sxs-lookup"><span data-stu-id="e0e18-191">Thumbprint</span></span>|
|<span data-ttu-id="e0e18-192">Número_serial_do_certificado</span><span class="sxs-lookup"><span data-stu-id="e0e18-192">certificateSerialNumber</span></span>|<span data-ttu-id="e0e18-193">String</span><span class="sxs-lookup"><span data-stu-id="e0e18-193">String</span></span>|<span data-ttu-id="e0e18-194">Número de série</span><span class="sxs-lookup"><span data-stu-id="e0e18-194">Serial number</span></span>|
|<span data-ttu-id="e0e18-195">certificateKeyLength</span><span class="sxs-lookup"><span data-stu-id="e0e18-195">certificateKeyLength</span></span>|<span data-ttu-id="e0e18-196">Int32</span><span class="sxs-lookup"><span data-stu-id="e0e18-196">Int32</span></span>|<span data-ttu-id="e0e18-197">Comprimento da chave</span><span class="sxs-lookup"><span data-stu-id="e0e18-197">Key length</span></span>|
|<span data-ttu-id="e0e18-198">certificateEnhancedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="e0e18-198">certificateEnhancedKeyUsage</span></span>|<span data-ttu-id="e0e18-199">String</span><span class="sxs-lookup"><span data-stu-id="e0e18-199">String</span></span>|<span data-ttu-id="e0e18-200">Uso estendido de chave</span><span class="sxs-lookup"><span data-stu-id="e0e18-200">Extended key usage</span></span>|
|<span data-ttu-id="e0e18-201">certificateValidityPeriod</span><span class="sxs-lookup"><span data-stu-id="e0e18-201">certificateValidityPeriod</span></span>|<span data-ttu-id="e0e18-202">Int32</span><span class="sxs-lookup"><span data-stu-id="e0e18-202">Int32</span></span>|<span data-ttu-id="e0e18-203">Período de validade</span><span class="sxs-lookup"><span data-stu-id="e0e18-203">Validity period</span></span>|
|<span data-ttu-id="e0e18-204">certificateSubjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="e0e18-204">certificateSubjectNameFormatString</span></span>|<span data-ttu-id="e0e18-205">String</span><span class="sxs-lookup"><span data-stu-id="e0e18-205">String</span></span>|<span data-ttu-id="e0e18-206">Sequência de formato de nome de entidade para formatos de nome de entidade personalizada</span><span class="sxs-lookup"><span data-stu-id="e0e18-206">Subject name format string for custom subject name formats</span></span>|
|<span data-ttu-id="e0e18-207">certificateSubjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="e0e18-207">certificateSubjectAlternativeNameFormatString</span></span>|<span data-ttu-id="e0e18-208">String</span><span class="sxs-lookup"><span data-stu-id="e0e18-208">String</span></span>|<span data-ttu-id="e0e18-209">Sequência de formato de nome alternativo de entidade para formatos personalizados</span><span class="sxs-lookup"><span data-stu-id="e0e18-209">Subject alternative name format string for custom formats</span></span>|
|<span data-ttu-id="e0e18-210">certificateIssuanceDateTime</span><span class="sxs-lookup"><span data-stu-id="e0e18-210">certificateIssuanceDateTime</span></span>|<span data-ttu-id="e0e18-211">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0e18-211">DateTimeOffset</span></span>|<span data-ttu-id="e0e18-212">Data de emissão</span><span class="sxs-lookup"><span data-stu-id="e0e18-212">Issuance date</span></span>|
|<span data-ttu-id="e0e18-213">certificateErrorCode</span><span class="sxs-lookup"><span data-stu-id="e0e18-213">certificateErrorCode</span></span>|<span data-ttu-id="e0e18-214">Int32</span><span class="sxs-lookup"><span data-stu-id="e0e18-214">Int32</span></span>|<span data-ttu-id="e0e18-215">Código de erro</span><span class="sxs-lookup"><span data-stu-id="e0e18-215">Error code</span></span>|



## <a name="response"></a><span data-ttu-id="e0e18-216">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0e18-216">Response</span></span>
<span data-ttu-id="e0e18-217">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e0e18-217">If successful, this method returns a `201 Created` response code and a [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0e18-218">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e0e18-218">Example</span></span>
### <a name="request"></a><span data-ttu-id="e0e18-219">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e0e18-219">Request</span></span>
<span data-ttu-id="e0e18-220">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e0e18-220">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e0e18-221">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0e18-221">Response</span></span>
<span data-ttu-id="e0e18-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e0e18-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





