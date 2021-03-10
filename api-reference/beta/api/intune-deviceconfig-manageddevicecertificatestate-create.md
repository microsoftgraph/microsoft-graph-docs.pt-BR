---
title: Criar managedDeviceCertificateState
description: Crie um novo objeto managedDeviceCertificateState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 56afd70ac51fc4f32ac997bad8545f84315911e0
ms.sourcegitcommit: cde4a3386b08a67cb476df6d46b51885c643d94f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50626029"
---
# <a name="create-manageddevicecertificatestate"></a><span data-ttu-id="3c04a-103">Criar managedDeviceCertificateState</span><span class="sxs-lookup"><span data-stu-id="3c04a-103">Create managedDeviceCertificateState</span></span>

<span data-ttu-id="3c04a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c04a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3c04a-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3c04a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3c04a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3c04a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c04a-107">Crie um novo [objeto managedDeviceCertificateState.](../resources/intune-deviceconfig-manageddevicecertificatestate.md)</span><span class="sxs-lookup"><span data-stu-id="3c04a-107">Create a new [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3c04a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3c04a-108">Prerequisites</span></span>
<span data-ttu-id="3c04a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c04a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c04a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3c04a-111">Permission type</span></span>|<span data-ttu-id="3c04a-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3c04a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3c04a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3c04a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3c04a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c04a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3c04a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3c04a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c04a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3c04a-116">Not supported.</span></span>|
|<span data-ttu-id="3c04a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3c04a-117">Application</span></span>|<span data-ttu-id="3c04a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c04a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3c04a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3c04a-119">HTTP Request</span></span>
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
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerPkcsCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerScepCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfilePkcsCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfileScepCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidForWorkImportedPFXCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerImportedPFXCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidForWorkPkcsCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidForWorkScepCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/microsoft.graph.windowsPhone81SCEPCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/microsoft.graph.macOSPkcsCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/microsoft.graph.macOSScepCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/microsoft.graph.macOSImportedPFXCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10PkcsCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows81SCEPCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10ImportedPFXCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windowsPhone81ImportedPFXCertificateProfile/managedDeviceCertificateStates
```

## <a name="request-headers"></a><span data-ttu-id="3c04a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3c04a-120">Request headers</span></span>
|<span data-ttu-id="3c04a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3c04a-121">Header</span></span>|<span data-ttu-id="3c04a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3c04a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3c04a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3c04a-123">Authorization</span></span>|<span data-ttu-id="3c04a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3c04a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3c04a-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3c04a-125">Accept</span></span>|<span data-ttu-id="3c04a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3c04a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c04a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3c04a-127">Request body</span></span>
<span data-ttu-id="3c04a-128">No corpo da solicitação, fornece uma representação JSON para o objeto managedDeviceCertificateState.</span><span class="sxs-lookup"><span data-stu-id="3c04a-128">In the request body, supply a JSON representation for the managedDeviceCertificateState object.</span></span>

<span data-ttu-id="3c04a-129">A tabela a seguir mostra as propriedades que são necessárias ao criar managedDeviceCertificateState.</span><span class="sxs-lookup"><span data-stu-id="3c04a-129">The following table shows the properties that are required when you create the managedDeviceCertificateState.</span></span>

|<span data-ttu-id="3c04a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3c04a-130">Property</span></span>|<span data-ttu-id="3c04a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="3c04a-131">Type</span></span>|<span data-ttu-id="3c04a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c04a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c04a-133">id</span><span class="sxs-lookup"><span data-stu-id="3c04a-133">id</span></span>|<span data-ttu-id="3c04a-134">String</span><span class="sxs-lookup"><span data-stu-id="3c04a-134">String</span></span>|<span data-ttu-id="3c04a-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="3c04a-135">Key of the entity.</span></span>|
|<span data-ttu-id="3c04a-136">devicePlatform</span><span class="sxs-lookup"><span data-stu-id="3c04a-136">devicePlatform</span></span>|[<span data-ttu-id="3c04a-137">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="3c04a-137">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="3c04a-138">Plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3c04a-138">Device platform.</span></span> <span data-ttu-id="3c04a-139">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="3c04a-139">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="3c04a-140">certificateKeyUsage</span><span class="sxs-lookup"><span data-stu-id="3c04a-140">certificateKeyUsage</span></span>|[<span data-ttu-id="3c04a-141">keyUsages</span><span class="sxs-lookup"><span data-stu-id="3c04a-141">keyUsages</span></span>](../resources/intune-shared-keyusages.md)|<span data-ttu-id="3c04a-142">Uso de chave.</span><span class="sxs-lookup"><span data-stu-id="3c04a-142">Key usage.</span></span> <span data-ttu-id="3c04a-143">Os valores possíveis são: `keyEncipherment` e `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="3c04a-143">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="3c04a-144">certificateValidityPeriodUnits</span><span class="sxs-lookup"><span data-stu-id="3c04a-144">certificateValidityPeriodUnits</span></span>|[<span data-ttu-id="3c04a-145">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="3c04a-145">certificateValidityPeriodScale</span></span>](../resources/intune-shared-certificatevalidityperiodscale.md)|<span data-ttu-id="3c04a-146">Unidades de período de validade.</span><span class="sxs-lookup"><span data-stu-id="3c04a-146">Validity period units.</span></span> <span data-ttu-id="3c04a-147">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="3c04a-147">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="3c04a-148">certificateIssuanceState</span><span class="sxs-lookup"><span data-stu-id="3c04a-148">certificateIssuanceState</span></span>|[<span data-ttu-id="3c04a-149">certificateIssuanceStates</span><span class="sxs-lookup"><span data-stu-id="3c04a-149">certificateIssuanceStates</span></span>](../resources/intune-deviceconfig-certificateissuancestates.md)|<span data-ttu-id="3c04a-150">Estado de emissão.</span><span class="sxs-lookup"><span data-stu-id="3c04a-150">Issuance State.</span></span> <span data-ttu-id="3c04a-151">Os valores possíveis são: `unknown` , , , , , , , , `challengeIssued` `challengeIssueFailed` , `requestCreationFailed` `requestSubmitFailed` , `challengeValidationSucceeded` `challengeValidationFailed` `issueFailed` `issuePending` `issued` `responseProcessingFailed` `responsePending` `enrollmentSucceeded` `enrollmentNotNeeded` `revoked` , `removedFromCollection` `renewVerified` `installFailed` `installed` `deleteFailed` `deleted` `renewalRequested` `requested`</span><span class="sxs-lookup"><span data-stu-id="3c04a-151">Possible values are: `unknown`, `challengeIssued`, `challengeIssueFailed`, `requestCreationFailed`, `requestSubmitFailed`, `challengeValidationSucceeded`, `challengeValidationFailed`, `issueFailed`, `issuePending`, `issued`, `responseProcessingFailed`, `responsePending`, `enrollmentSucceeded`, `enrollmentNotNeeded`, `revoked`, `removedFromCollection`, `renewVerified`, `installFailed`, `installed`, `deleteFailed`, `deleted`, `renewalRequested`, `requested`.</span></span>|
|<span data-ttu-id="3c04a-152">certificateKeyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="3c04a-152">certificateKeyStorageProvider</span></span>|[<span data-ttu-id="3c04a-153">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="3c04a-153">keyStorageProviderOption</span></span>](../resources/intune-shared-keystorageprovideroption.md)|<span data-ttu-id="3c04a-154">Provedor de Armazenamento de Chaves.</span><span class="sxs-lookup"><span data-stu-id="3c04a-154">Key Storage Provider.</span></span> <span data-ttu-id="3c04a-155">Os valores possíveis são: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="3c04a-155">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="3c04a-156">certificateSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="3c04a-156">certificateSubjectNameFormat</span></span>|[<span data-ttu-id="3c04a-157">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="3c04a-157">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="3c04a-158">Formato de nome do assunto.</span><span class="sxs-lookup"><span data-stu-id="3c04a-158">Subject name format.</span></span> <span data-ttu-id="3c04a-159">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="3c04a-159">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="3c04a-160">certificateSubjectAlternativeNameFormat</span><span class="sxs-lookup"><span data-stu-id="3c04a-160">certificateSubjectAlternativeNameFormat</span></span>|[<span data-ttu-id="3c04a-161">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="3c04a-161">subjectAlternativeNameType</span></span>](../resources/intune-shared-subjectalternativenametype.md)|<span data-ttu-id="3c04a-162">Formato de nome alternativo do assunto.</span><span class="sxs-lookup"><span data-stu-id="3c04a-162">Subject alternative name format.</span></span> <span data-ttu-id="3c04a-163">Os possíveis valores são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span><span class="sxs-lookup"><span data-stu-id="3c04a-163">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span></span>|
|<span data-ttu-id="3c04a-164">certificateRevokeStatus</span><span class="sxs-lookup"><span data-stu-id="3c04a-164">certificateRevokeStatus</span></span>|[<span data-ttu-id="3c04a-165">certificateRevocationStatus</span><span class="sxs-lookup"><span data-stu-id="3c04a-165">certificateRevocationStatus</span></span>](../resources/intune-deviceconfig-certificaterevocationstatus.md)|<span data-ttu-id="3c04a-166">Revogar status.</span><span class="sxs-lookup"><span data-stu-id="3c04a-166">Revoke status.</span></span> <span data-ttu-id="3c04a-167">Os valores possíveis são: `none`, `pending`, `issued`, `failed`, `revoked`.</span><span class="sxs-lookup"><span data-stu-id="3c04a-167">Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.</span></span>|
|<span data-ttu-id="3c04a-168">certificateProfileDisplayName</span><span class="sxs-lookup"><span data-stu-id="3c04a-168">certificateProfileDisplayName</span></span>|<span data-ttu-id="3c04a-169">String</span><span class="sxs-lookup"><span data-stu-id="3c04a-169">String</span></span>|<span data-ttu-id="3c04a-170">Nome de exibição de perfil de certificado</span><span class="sxs-lookup"><span data-stu-id="3c04a-170">Certificate profile display name</span></span>|
|<span data-ttu-id="3c04a-171">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="3c04a-171">deviceDisplayName</span></span>|<span data-ttu-id="3c04a-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3c04a-172">String</span></span>|<span data-ttu-id="3c04a-173">Nome de exibição do dispositivo</span><span class="sxs-lookup"><span data-stu-id="3c04a-173">Device display name</span></span>|
|<span data-ttu-id="3c04a-174">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="3c04a-174">userDisplayName</span></span>|<span data-ttu-id="3c04a-175">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3c04a-175">String</span></span>|<span data-ttu-id="3c04a-176">Nome de exibição do usuário</span><span class="sxs-lookup"><span data-stu-id="3c04a-176">User display name</span></span>|
|<span data-ttu-id="3c04a-177">certificateExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="3c04a-177">certificateExpirationDateTime</span></span>|<span data-ttu-id="3c04a-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c04a-178">DateTimeOffset</span></span>|<span data-ttu-id="3c04a-179">Data de expiração do certificado</span><span class="sxs-lookup"><span data-stu-id="3c04a-179">Certificate expiry date</span></span>|
|<span data-ttu-id="3c04a-180">certificateLastIssuanceStateChangedDateTime</span><span class="sxs-lookup"><span data-stu-id="3c04a-180">certificateLastIssuanceStateChangedDateTime</span></span>|<span data-ttu-id="3c04a-181">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c04a-181">DateTimeOffset</span></span>|<span data-ttu-id="3c04a-182">Última alteração de estado de emissão de certificado</span><span class="sxs-lookup"><span data-stu-id="3c04a-182">Last certificate issuance state change</span></span>|
|<span data-ttu-id="3c04a-183">lastCertificateStateChangeDateTime</span><span class="sxs-lookup"><span data-stu-id="3c04a-183">lastCertificateStateChangeDateTime</span></span>|<span data-ttu-id="3c04a-184">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c04a-184">DateTimeOffset</span></span>|<span data-ttu-id="3c04a-185">Última alteração de estado de emissão de certificado</span><span class="sxs-lookup"><span data-stu-id="3c04a-185">Last certificate issuance state change</span></span>|
|<span data-ttu-id="3c04a-186">certificateIssuer</span><span class="sxs-lookup"><span data-stu-id="3c04a-186">certificateIssuer</span></span>|<span data-ttu-id="3c04a-187">String</span><span class="sxs-lookup"><span data-stu-id="3c04a-187">String</span></span>|<span data-ttu-id="3c04a-188">Emissor</span><span class="sxs-lookup"><span data-stu-id="3c04a-188">Issuer</span></span>|
|<span data-ttu-id="3c04a-189">certificateThumbprint</span><span class="sxs-lookup"><span data-stu-id="3c04a-189">certificateThumbprint</span></span>|<span data-ttu-id="3c04a-190">String</span><span class="sxs-lookup"><span data-stu-id="3c04a-190">String</span></span>|<span data-ttu-id="3c04a-191">Impressão Digital</span><span class="sxs-lookup"><span data-stu-id="3c04a-191">Thumbprint</span></span>|
|<span data-ttu-id="3c04a-192">certificateSerialNumber</span><span class="sxs-lookup"><span data-stu-id="3c04a-192">certificateSerialNumber</span></span>|<span data-ttu-id="3c04a-193">String</span><span class="sxs-lookup"><span data-stu-id="3c04a-193">String</span></span>|<span data-ttu-id="3c04a-194">Número de série</span><span class="sxs-lookup"><span data-stu-id="3c04a-194">Serial number</span></span>|
|<span data-ttu-id="3c04a-195">certificateKeyLength</span><span class="sxs-lookup"><span data-stu-id="3c04a-195">certificateKeyLength</span></span>|<span data-ttu-id="3c04a-196">Int32</span><span class="sxs-lookup"><span data-stu-id="3c04a-196">Int32</span></span>|<span data-ttu-id="3c04a-197">Comprimento de chave</span><span class="sxs-lookup"><span data-stu-id="3c04a-197">Key length</span></span>|
|<span data-ttu-id="3c04a-198">certificateEnhancedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="3c04a-198">certificateEnhancedKeyUsage</span></span>|<span data-ttu-id="3c04a-199">String</span><span class="sxs-lookup"><span data-stu-id="3c04a-199">String</span></span>|<span data-ttu-id="3c04a-200">Uso estendido de chave</span><span class="sxs-lookup"><span data-stu-id="3c04a-200">Extended key usage</span></span>|
|<span data-ttu-id="3c04a-201">certificateValidityPeriod</span><span class="sxs-lookup"><span data-stu-id="3c04a-201">certificateValidityPeriod</span></span>|<span data-ttu-id="3c04a-202">Int32</span><span class="sxs-lookup"><span data-stu-id="3c04a-202">Int32</span></span>|<span data-ttu-id="3c04a-203">Período de validade</span><span class="sxs-lookup"><span data-stu-id="3c04a-203">Validity period</span></span>|
|<span data-ttu-id="3c04a-204">certificateSubjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="3c04a-204">certificateSubjectNameFormatString</span></span>|<span data-ttu-id="3c04a-205">String</span><span class="sxs-lookup"><span data-stu-id="3c04a-205">String</span></span>|<span data-ttu-id="3c04a-206">Cadeia de caracteres de formato de nome de assunto para formatos de nome de assunto personalizados</span><span class="sxs-lookup"><span data-stu-id="3c04a-206">Subject name format string for custom subject name formats</span></span>|
|<span data-ttu-id="3c04a-207">certificateSubjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="3c04a-207">certificateSubjectAlternativeNameFormatString</span></span>|<span data-ttu-id="3c04a-208">String</span><span class="sxs-lookup"><span data-stu-id="3c04a-208">String</span></span>|<span data-ttu-id="3c04a-209">Cadeia de caracteres de formato de nome alternativo de assunto para formatos personalizados</span><span class="sxs-lookup"><span data-stu-id="3c04a-209">Subject alternative name format string for custom formats</span></span>|
|<span data-ttu-id="3c04a-210">certificateIssuanceDateTime</span><span class="sxs-lookup"><span data-stu-id="3c04a-210">certificateIssuanceDateTime</span></span>|<span data-ttu-id="3c04a-211">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c04a-211">DateTimeOffset</span></span>|<span data-ttu-id="3c04a-212">Data de emissão</span><span class="sxs-lookup"><span data-stu-id="3c04a-212">Issuance date</span></span>|
|<span data-ttu-id="3c04a-213">certificateErrorCode</span><span class="sxs-lookup"><span data-stu-id="3c04a-213">certificateErrorCode</span></span>|<span data-ttu-id="3c04a-214">Int32</span><span class="sxs-lookup"><span data-stu-id="3c04a-214">Int32</span></span>|<span data-ttu-id="3c04a-215">Código de erro</span><span class="sxs-lookup"><span data-stu-id="3c04a-215">Error code</span></span>|



## <a name="response"></a><span data-ttu-id="3c04a-216">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c04a-216">Response</span></span>
<span data-ttu-id="3c04a-217">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3c04a-217">If successful, this method returns a `201 Created` response code and a [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c04a-218">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3c04a-218">Example</span></span>

### <a name="request"></a><span data-ttu-id="3c04a-219">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3c04a-219">Request</span></span>
<span data-ttu-id="3c04a-220">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3c04a-220">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3c04a-221">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c04a-221">Response</span></span>
<span data-ttu-id="3c04a-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3c04a-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




