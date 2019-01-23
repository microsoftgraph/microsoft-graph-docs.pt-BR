---
title: Criar managedDeviceCertificateState
description: Crie um novo objeto de managedDeviceCertificateState.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f8efc74f2f8abad4b659f41ac53d270af5dab2a3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396312"
---
# <a name="create-manageddevicecertificatestate"></a><span data-ttu-id="f1d02-103">Criar managedDeviceCertificateState</span><span class="sxs-lookup"><span data-stu-id="f1d02-103">Create managedDeviceCertificateState</span></span>

> <span data-ttu-id="f1d02-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="f1d02-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f1d02-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f1d02-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f1d02-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="f1d02-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1d02-107">Crie um novo objeto de [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="f1d02-107">Create a new [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f1d02-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f1d02-108">Prerequisites</span></span>
<span data-ttu-id="f1d02-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f1d02-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f1d02-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f1d02-111">Permission type</span></span>|<span data-ttu-id="f1d02-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f1d02-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1d02-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f1d02-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f1d02-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1d02-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f1d02-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f1d02-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1d02-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1d02-116">Not supported.</span></span>|
|<span data-ttu-id="f1d02-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f1d02-117">Application</span></span>|<span data-ttu-id="f1d02-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1d02-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1d02-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f1d02-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="f1d02-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f1d02-120">Request headers</span></span>
|<span data-ttu-id="f1d02-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f1d02-121">Header</span></span>|<span data-ttu-id="f1d02-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f1d02-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1d02-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f1d02-123">Authorization</span></span>|<span data-ttu-id="f1d02-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f1d02-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1d02-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f1d02-125">Accept</span></span>|<span data-ttu-id="f1d02-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f1d02-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1d02-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f1d02-127">Request body</span></span>
<span data-ttu-id="f1d02-128">No corpo da solicitação, fornece uma representação JSON para o objeto managedDeviceCertificateState.</span><span class="sxs-lookup"><span data-stu-id="f1d02-128">In the request body, supply a JSON representation for the managedDeviceCertificateState object.</span></span>

<span data-ttu-id="f1d02-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o managedDeviceCertificateState.</span><span class="sxs-lookup"><span data-stu-id="f1d02-129">The following table shows the properties that are required when you create the managedDeviceCertificateState.</span></span>

|<span data-ttu-id="f1d02-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f1d02-130">Property</span></span>|<span data-ttu-id="f1d02-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f1d02-131">Type</span></span>|<span data-ttu-id="f1d02-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1d02-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1d02-133">id</span><span class="sxs-lookup"><span data-stu-id="f1d02-133">id</span></span>|<span data-ttu-id="f1d02-134">String</span><span class="sxs-lookup"><span data-stu-id="f1d02-134">String</span></span>|<span data-ttu-id="f1d02-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f1d02-135">Key of the entity.</span></span>|
|<span data-ttu-id="f1d02-136">devicePlatform</span><span class="sxs-lookup"><span data-stu-id="f1d02-136">devicePlatform</span></span>|[<span data-ttu-id="f1d02-137">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="f1d02-137">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="f1d02-138">Plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f1d02-138">Device platform.</span></span> <span data-ttu-id="f1d02-139">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span><span class="sxs-lookup"><span data-stu-id="f1d02-139">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|
|<span data-ttu-id="f1d02-140">certificateKeyUsage</span><span class="sxs-lookup"><span data-stu-id="f1d02-140">certificateKeyUsage</span></span>|[<span data-ttu-id="f1d02-141">keyUsages</span><span class="sxs-lookup"><span data-stu-id="f1d02-141">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="f1d02-142">Uso da chave.</span><span class="sxs-lookup"><span data-stu-id="f1d02-142">Key usage.</span></span> <span data-ttu-id="f1d02-143">Os valores possíveis são: `keyEncipherment` e `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="f1d02-143">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="f1d02-144">certificateValidityPeriodUnits</span><span class="sxs-lookup"><span data-stu-id="f1d02-144">certificateValidityPeriodUnits</span></span>|[<span data-ttu-id="f1d02-145">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="f1d02-145">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="f1d02-146">Unidades do período de validade.</span><span class="sxs-lookup"><span data-stu-id="f1d02-146">Validity period units.</span></span> <span data-ttu-id="f1d02-147">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="f1d02-147">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="f1d02-148">certificateIssuanceState</span><span class="sxs-lookup"><span data-stu-id="f1d02-148">certificateIssuanceState</span></span>|[<span data-ttu-id="f1d02-149">certificateIssuanceStates</span><span class="sxs-lookup"><span data-stu-id="f1d02-149">certificateIssuanceStates</span></span>](../resources/intune-deviceconfig-certificateissuancestates.md)|<span data-ttu-id="f1d02-150">Estado de emissão.</span><span class="sxs-lookup"><span data-stu-id="f1d02-150">Issuance State.</span></span> <span data-ttu-id="f1d02-151">Os valores possíveis são: `unknown`, `challengeIssued`, `challengeIssueFailed`, `requestCreationFailed`, `requestSubmitFailed`, `challengeValidationSucceeded`, `challengeValidationFailed`, `issueFailed`, `issuePending`, `issued`, `responseProcessingFailed`, `responsePending`, `enrollmentSucceeded`, `enrollmentNotNeeded`, `revoked`, `removedFromCollection`, `renewVerified`, `installFailed`, `installed` , `deleteFailed`, `deleted`, `renewalRequested`, `requested`.</span><span class="sxs-lookup"><span data-stu-id="f1d02-151">Possible values are: `unknown`, `challengeIssued`, `challengeIssueFailed`, `requestCreationFailed`, `requestSubmitFailed`, `challengeValidationSucceeded`, `challengeValidationFailed`, `issueFailed`, `issuePending`, `issued`, `responseProcessingFailed`, `responsePending`, `enrollmentSucceeded`, `enrollmentNotNeeded`, `revoked`, `removedFromCollection`, `renewVerified`, `installFailed`, `installed`, `deleteFailed`, `deleted`, `renewalRequested`, `requested`.</span></span>|
|<span data-ttu-id="f1d02-152">certificateKeyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="f1d02-152">certificateKeyStorageProvider</span></span>|[<span data-ttu-id="f1d02-153">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="f1d02-153">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="f1d02-154">Provedor de armazenamento de chave.</span><span class="sxs-lookup"><span data-stu-id="f1d02-154">Key Storage Provider.</span></span> <span data-ttu-id="f1d02-155">Os valores possíveis são: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="f1d02-155">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="f1d02-156">certificateSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="f1d02-156">certificateSubjectNameFormat</span></span>|[<span data-ttu-id="f1d02-157">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="f1d02-157">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="f1d02-158">Formato de nome de entidade.</span><span class="sxs-lookup"><span data-stu-id="f1d02-158">Subject name format.</span></span> <span data-ttu-id="f1d02-159">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="f1d02-159">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="f1d02-160">certificateSubjectAlternativeNameFormat</span><span class="sxs-lookup"><span data-stu-id="f1d02-160">certificateSubjectAlternativeNameFormat</span></span>|[<span data-ttu-id="f1d02-161">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="f1d02-161">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="f1d02-162">Formato de nome alternativo da entidade.</span><span class="sxs-lookup"><span data-stu-id="f1d02-162">Subject alternative name format.</span></span> <span data-ttu-id="f1d02-163">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="f1d02-163">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="f1d02-164">certificateRevokeStatus</span><span class="sxs-lookup"><span data-stu-id="f1d02-164">certificateRevokeStatus</span></span>|[<span data-ttu-id="f1d02-165">certificateRevocationStatus</span><span class="sxs-lookup"><span data-stu-id="f1d02-165">certificateRevocationStatus</span></span>](../resources/intune-deviceconfig-certificaterevocationstatus.md)|<span data-ttu-id="f1d02-166">Revogar o status.</span><span class="sxs-lookup"><span data-stu-id="f1d02-166">Revoke status.</span></span> <span data-ttu-id="f1d02-167">Os valores possíveis são: `none`, `pending`, `issued`, `failed`, `revoked`.</span><span class="sxs-lookup"><span data-stu-id="f1d02-167">Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.</span></span>|
|<span data-ttu-id="f1d02-168">certificateProfileDisplayName</span><span class="sxs-lookup"><span data-stu-id="f1d02-168">certificateProfileDisplayName</span></span>|<span data-ttu-id="f1d02-169">String</span><span class="sxs-lookup"><span data-stu-id="f1d02-169">String</span></span>|<span data-ttu-id="f1d02-170">Nome de exibição de perfil de certificado</span><span class="sxs-lookup"><span data-stu-id="f1d02-170">Certificate profile display name</span></span>|
|<span data-ttu-id="f1d02-171">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="f1d02-171">deviceDisplayName</span></span>|<span data-ttu-id="f1d02-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f1d02-172">String</span></span>|<span data-ttu-id="f1d02-173">Nome de exibição do dispositivo</span><span class="sxs-lookup"><span data-stu-id="f1d02-173">Device display name</span></span>|
|<span data-ttu-id="f1d02-174">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="f1d02-174">userDisplayName</span></span>|<span data-ttu-id="f1d02-175">String</span><span class="sxs-lookup"><span data-stu-id="f1d02-175">String</span></span>|<span data-ttu-id="f1d02-176">Nome de exibição do usuário</span><span class="sxs-lookup"><span data-stu-id="f1d02-176">User display name</span></span>|
|<span data-ttu-id="f1d02-177">certificateExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="f1d02-177">certificateExpirationDateTime</span></span>|<span data-ttu-id="f1d02-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1d02-178">DateTimeOffset</span></span>|<span data-ttu-id="f1d02-179">Data de expiração de certificado</span><span class="sxs-lookup"><span data-stu-id="f1d02-179">Certificate expiry date</span></span>|
|<span data-ttu-id="f1d02-180">certificateLastIssuanceStateChangedDateTime</span><span class="sxs-lookup"><span data-stu-id="f1d02-180">certificateLastIssuanceStateChangedDateTime</span></span>|<span data-ttu-id="f1d02-181">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1d02-181">DateTimeOffset</span></span>|<span data-ttu-id="f1d02-182">Última alteração de estado de emissão de certificado</span><span class="sxs-lookup"><span data-stu-id="f1d02-182">Last certificate issuance state change</span></span>|
|<span data-ttu-id="f1d02-183">lastCertificateStateChangeDateTime</span><span class="sxs-lookup"><span data-stu-id="f1d02-183">lastCertificateStateChangeDateTime</span></span>|<span data-ttu-id="f1d02-184">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1d02-184">DateTimeOffset</span></span>|<span data-ttu-id="f1d02-185">Última alteração de estado de emissão de certificado</span><span class="sxs-lookup"><span data-stu-id="f1d02-185">Last certificate issuance state change</span></span>|
|<span data-ttu-id="f1d02-186">certificateIssuer</span><span class="sxs-lookup"><span data-stu-id="f1d02-186">certificateIssuer</span></span>|<span data-ttu-id="f1d02-187">String</span><span class="sxs-lookup"><span data-stu-id="f1d02-187">String</span></span>|<span data-ttu-id="f1d02-188">Emissor</span><span class="sxs-lookup"><span data-stu-id="f1d02-188">Issuer</span></span>|
|<span data-ttu-id="f1d02-189">certificateThumbprint</span><span class="sxs-lookup"><span data-stu-id="f1d02-189">certificateThumbprint</span></span>|<span data-ttu-id="f1d02-190">String</span><span class="sxs-lookup"><span data-stu-id="f1d02-190">String</span></span>|<span data-ttu-id="f1d02-191">Impressão digital</span><span class="sxs-lookup"><span data-stu-id="f1d02-191">Thumbprint</span></span>|
|<span data-ttu-id="f1d02-192">Número_serial_do_certificado</span><span class="sxs-lookup"><span data-stu-id="f1d02-192">certificateSerialNumber</span></span>|<span data-ttu-id="f1d02-193">String</span><span class="sxs-lookup"><span data-stu-id="f1d02-193">String</span></span>|<span data-ttu-id="f1d02-194">Número de série</span><span class="sxs-lookup"><span data-stu-id="f1d02-194">Serial number</span></span>|
|<span data-ttu-id="f1d02-195">certificateKeyLength</span><span class="sxs-lookup"><span data-stu-id="f1d02-195">certificateKeyLength</span></span>|<span data-ttu-id="f1d02-196">Int32</span><span class="sxs-lookup"><span data-stu-id="f1d02-196">Int32</span></span>|<span data-ttu-id="f1d02-197">Comprimento da chave</span><span class="sxs-lookup"><span data-stu-id="f1d02-197">Key length</span></span>|
|<span data-ttu-id="f1d02-198">certificateEnhancedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="f1d02-198">certificateEnhancedKeyUsage</span></span>|<span data-ttu-id="f1d02-199">String</span><span class="sxs-lookup"><span data-stu-id="f1d02-199">String</span></span>|<span data-ttu-id="f1d02-200">Uso estendido de chave</span><span class="sxs-lookup"><span data-stu-id="f1d02-200">Extended key usage</span></span>|
|<span data-ttu-id="f1d02-201">certificateValidityPeriod</span><span class="sxs-lookup"><span data-stu-id="f1d02-201">certificateValidityPeriod</span></span>|<span data-ttu-id="f1d02-202">Int32</span><span class="sxs-lookup"><span data-stu-id="f1d02-202">Int32</span></span>|<span data-ttu-id="f1d02-203">Período de validade</span><span class="sxs-lookup"><span data-stu-id="f1d02-203">Validity period</span></span>|
|<span data-ttu-id="f1d02-204">certificateSubjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="f1d02-204">certificateSubjectNameFormatString</span></span>|<span data-ttu-id="f1d02-205">String</span><span class="sxs-lookup"><span data-stu-id="f1d02-205">String</span></span>|<span data-ttu-id="f1d02-206">Sequência de formato de nome de entidade para formatos de nome de entidade personalizada</span><span class="sxs-lookup"><span data-stu-id="f1d02-206">Subject name format string for custom subject name formats</span></span>|
|<span data-ttu-id="f1d02-207">certificateSubjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="f1d02-207">certificateSubjectAlternativeNameFormatString</span></span>|<span data-ttu-id="f1d02-208">String</span><span class="sxs-lookup"><span data-stu-id="f1d02-208">String</span></span>|<span data-ttu-id="f1d02-209">Sequência de formato de nome alternativo de entidade para formatos personalizados</span><span class="sxs-lookup"><span data-stu-id="f1d02-209">Subject alternative name format string for custom formats</span></span>|
|<span data-ttu-id="f1d02-210">certificateIssuanceDateTime</span><span class="sxs-lookup"><span data-stu-id="f1d02-210">certificateIssuanceDateTime</span></span>|<span data-ttu-id="f1d02-211">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1d02-211">DateTimeOffset</span></span>|<span data-ttu-id="f1d02-212">Data de emissão</span><span class="sxs-lookup"><span data-stu-id="f1d02-212">Issuance date</span></span>|
|<span data-ttu-id="f1d02-213">certificateErrorCode</span><span class="sxs-lookup"><span data-stu-id="f1d02-213">certificateErrorCode</span></span>|<span data-ttu-id="f1d02-214">Int32</span><span class="sxs-lookup"><span data-stu-id="f1d02-214">Int32</span></span>|<span data-ttu-id="f1d02-215">Código de erro</span><span class="sxs-lookup"><span data-stu-id="f1d02-215">Error code</span></span>|



## <a name="response"></a><span data-ttu-id="f1d02-216">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1d02-216">Response</span></span>
<span data-ttu-id="f1d02-217">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f1d02-217">If successful, this method returns a `201 Created` response code and a [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1d02-218">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f1d02-218">Example</span></span>

### <a name="request"></a><span data-ttu-id="f1d02-219">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f1d02-219">Request</span></span>
<span data-ttu-id="f1d02-220">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f1d02-220">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f1d02-221">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1d02-221">Response</span></span>
<span data-ttu-id="f1d02-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f1d02-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




