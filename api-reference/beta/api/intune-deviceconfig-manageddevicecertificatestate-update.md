---
title: Atualizar managedDeviceCertificateState
description: Atualiza as propriedades de um objeto managedDeviceCertificateState.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fba7cadcf11c03bd7dcff0cc3b50b7cd8775c6f1
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/31/2020
ms.locfileid: "41635772"
---
# <a name="update-manageddevicecertificatestate"></a><span data-ttu-id="a1e55-103">Atualizar managedDeviceCertificateState</span><span class="sxs-lookup"><span data-stu-id="a1e55-103">Update managedDeviceCertificateState</span></span>

> <span data-ttu-id="a1e55-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a1e55-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a1e55-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a1e55-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1e55-106">Atualiza as propriedades de um objeto [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="a1e55-106">Update the properties of a [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a1e55-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a1e55-107">Prerequisites</span></span>
<span data-ttu-id="a1e55-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1e55-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1e55-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a1e55-110">Permission type</span></span>|<span data-ttu-id="a1e55-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a1e55-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1e55-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a1e55-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a1e55-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1e55-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a1e55-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a1e55-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1e55-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1e55-115">Not supported.</span></span>|
|<span data-ttu-id="a1e55-116">Application</span><span class="sxs-lookup"><span data-stu-id="a1e55-116">Application</span></span>|<span data-ttu-id="a1e55-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1e55-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1e55-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a1e55-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfilePkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfileScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidForWorkImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/microsoft.graph.windowsPhone81SCEPCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/microsoft.graph.macOSPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/microsoft.graph.macOSScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/microsoft.graph.macOSImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10PkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows81SCEPCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10ImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windowsPhone81ImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
```

## <a name="request-headers"></a><span data-ttu-id="a1e55-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a1e55-119">Request headers</span></span>
|<span data-ttu-id="a1e55-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a1e55-120">Header</span></span>|<span data-ttu-id="a1e55-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a1e55-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1e55-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a1e55-122">Authorization</span></span>|<span data-ttu-id="a1e55-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a1e55-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1e55-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a1e55-124">Accept</span></span>|<span data-ttu-id="a1e55-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a1e55-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1e55-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a1e55-126">Request body</span></span>
<span data-ttu-id="a1e55-127">No corpo da solicitação, forneça uma representação JSON do objeto [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="a1e55-127">In the request body, supply a JSON representation for the [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object.</span></span>

<span data-ttu-id="a1e55-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md).</span><span class="sxs-lookup"><span data-stu-id="a1e55-128">The following table shows the properties that are required when you create the [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md).</span></span>

|<span data-ttu-id="a1e55-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a1e55-129">Property</span></span>|<span data-ttu-id="a1e55-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a1e55-130">Type</span></span>|<span data-ttu-id="a1e55-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1e55-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1e55-132">id</span><span class="sxs-lookup"><span data-stu-id="a1e55-132">id</span></span>|<span data-ttu-id="a1e55-133">String</span><span class="sxs-lookup"><span data-stu-id="a1e55-133">String</span></span>|<span data-ttu-id="a1e55-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a1e55-134">Key of the entity.</span></span>|
|<span data-ttu-id="a1e55-135">devicePlatform</span><span class="sxs-lookup"><span data-stu-id="a1e55-135">devicePlatform</span></span>|[<span data-ttu-id="a1e55-136">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="a1e55-136">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="a1e55-137">Plataforma de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a1e55-137">Device platform.</span></span> <span data-ttu-id="a1e55-138">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="a1e55-138">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="a1e55-139">certificateKeyUsage</span><span class="sxs-lookup"><span data-stu-id="a1e55-139">certificateKeyUsage</span></span>|[<span data-ttu-id="a1e55-140">usos de</span><span class="sxs-lookup"><span data-stu-id="a1e55-140">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="a1e55-141">Uso de chave.</span><span class="sxs-lookup"><span data-stu-id="a1e55-141">Key usage.</span></span> <span data-ttu-id="a1e55-142">Os valores possíveis são: `keyEncipherment` e `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="a1e55-142">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="a1e55-143">certificateValidityPeriodUnits</span><span class="sxs-lookup"><span data-stu-id="a1e55-143">certificateValidityPeriodUnits</span></span>|[<span data-ttu-id="a1e55-144">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="a1e55-144">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="a1e55-145">Unidades de período de validade.</span><span class="sxs-lookup"><span data-stu-id="a1e55-145">Validity period units.</span></span> <span data-ttu-id="a1e55-146">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="a1e55-146">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="a1e55-147">certificateIssuanceState</span><span class="sxs-lookup"><span data-stu-id="a1e55-147">certificateIssuanceState</span></span>|[<span data-ttu-id="a1e55-148">certificateIssuanceStates</span><span class="sxs-lookup"><span data-stu-id="a1e55-148">certificateIssuanceStates</span></span>](../resources/intune-deviceconfig-certificateissuancestates.md)|<span data-ttu-id="a1e55-149">Estado de emissão.</span><span class="sxs-lookup"><span data-stu-id="a1e55-149">Issuance State.</span></span> <span data-ttu-id="a1e55-150">Os valores possíveis são `unknown`: `challengeIssued`, `challengeIssueFailed`, `requestCreationFailed`, `requestSubmitFailed` `challengeValidationSucceeded` `challengeValidationFailed`,,, `issueFailed`, `issuePending`, `issued` `responseProcessingFailed` `responsePending`,,, `enrollmentSucceeded`, `enrollmentNotNeeded`, `revoked`, `removedFromCollection`, `renewVerified`, `installFailed`, `installed` `deleteFailed` `deleted` `renewalRequested`,,,, `requested`,,,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="a1e55-150">Possible values are: `unknown`, `challengeIssued`, `challengeIssueFailed`, `requestCreationFailed`, `requestSubmitFailed`, `challengeValidationSucceeded`, `challengeValidationFailed`, `issueFailed`, `issuePending`, `issued`, `responseProcessingFailed`, `responsePending`, `enrollmentSucceeded`, `enrollmentNotNeeded`, `revoked`, `removedFromCollection`, `renewVerified`, `installFailed`, `installed`, `deleteFailed`, `deleted`, `renewalRequested`, `requested`.</span></span>|
|<span data-ttu-id="a1e55-151">certificateKeyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="a1e55-151">certificateKeyStorageProvider</span></span>|[<span data-ttu-id="a1e55-152">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="a1e55-152">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="a1e55-153">Provedor de armazenamento de chave.</span><span class="sxs-lookup"><span data-stu-id="a1e55-153">Key Storage Provider.</span></span> <span data-ttu-id="a1e55-154">Os valores possíveis são: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="a1e55-154">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="a1e55-155">certificateSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="a1e55-155">certificateSubjectNameFormat</span></span>|[<span data-ttu-id="a1e55-156">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="a1e55-156">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="a1e55-157">Formato do nome da entidade.</span><span class="sxs-lookup"><span data-stu-id="a1e55-157">Subject name format.</span></span> <span data-ttu-id="a1e55-158">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="a1e55-158">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="a1e55-159">certificateSubjectAlternativeNameFormat</span><span class="sxs-lookup"><span data-stu-id="a1e55-159">certificateSubjectAlternativeNameFormat</span></span>|[<span data-ttu-id="a1e55-160">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="a1e55-160">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="a1e55-161">Formato de nome alternativo da entidade.</span><span class="sxs-lookup"><span data-stu-id="a1e55-161">Subject alternative name format.</span></span> <span data-ttu-id="a1e55-162">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="a1e55-162">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="a1e55-163">certificateRevokeStatus</span><span class="sxs-lookup"><span data-stu-id="a1e55-163">certificateRevokeStatus</span></span>|[<span data-ttu-id="a1e55-164">certificateRevocationStatus</span><span class="sxs-lookup"><span data-stu-id="a1e55-164">certificateRevocationStatus</span></span>](../resources/intune-deviceconfig-certificaterevocationstatus.md)|<span data-ttu-id="a1e55-165">Revogar status.</span><span class="sxs-lookup"><span data-stu-id="a1e55-165">Revoke status.</span></span> <span data-ttu-id="a1e55-166">Os valores possíveis são: `none`, `pending`, `issued`, `failed`, `revoked`.</span><span class="sxs-lookup"><span data-stu-id="a1e55-166">Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.</span></span>|
|<span data-ttu-id="a1e55-167">certificateProfileDisplayName</span><span class="sxs-lookup"><span data-stu-id="a1e55-167">certificateProfileDisplayName</span></span>|<span data-ttu-id="a1e55-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a1e55-168">String</span></span>|<span data-ttu-id="a1e55-169">Nome de exibição do perfil do certificado</span><span class="sxs-lookup"><span data-stu-id="a1e55-169">Certificate profile display name</span></span>|
|<span data-ttu-id="a1e55-170">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="a1e55-170">deviceDisplayName</span></span>|<span data-ttu-id="a1e55-171">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a1e55-171">String</span></span>|<span data-ttu-id="a1e55-172">Nome de exibição do dispositivo</span><span class="sxs-lookup"><span data-stu-id="a1e55-172">Device display name</span></span>|
|<span data-ttu-id="a1e55-173">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="a1e55-173">userDisplayName</span></span>|<span data-ttu-id="a1e55-174">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a1e55-174">String</span></span>|<span data-ttu-id="a1e55-175">Nome de exibição do usuário</span><span class="sxs-lookup"><span data-stu-id="a1e55-175">User display name</span></span>|
|<span data-ttu-id="a1e55-176">certificateExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="a1e55-176">certificateExpirationDateTime</span></span>|<span data-ttu-id="a1e55-177">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1e55-177">DateTimeOffset</span></span>|<span data-ttu-id="a1e55-178">Data de vencimento do certificado</span><span class="sxs-lookup"><span data-stu-id="a1e55-178">Certificate expiry date</span></span>|
|<span data-ttu-id="a1e55-179">certificateLastIssuanceStateChangedDateTime</span><span class="sxs-lookup"><span data-stu-id="a1e55-179">certificateLastIssuanceStateChangedDateTime</span></span>|<span data-ttu-id="a1e55-180">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1e55-180">DateTimeOffset</span></span>|<span data-ttu-id="a1e55-181">Última alteração no estado de emissão de certificado</span><span class="sxs-lookup"><span data-stu-id="a1e55-181">Last certificate issuance state change</span></span>|
|<span data-ttu-id="a1e55-182">lastCertificateStateChangeDateTime</span><span class="sxs-lookup"><span data-stu-id="a1e55-182">lastCertificateStateChangeDateTime</span></span>|<span data-ttu-id="a1e55-183">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1e55-183">DateTimeOffset</span></span>|<span data-ttu-id="a1e55-184">Última alteração no estado de emissão de certificado</span><span class="sxs-lookup"><span data-stu-id="a1e55-184">Last certificate issuance state change</span></span>|
|<span data-ttu-id="a1e55-185">certificateIssuer</span><span class="sxs-lookup"><span data-stu-id="a1e55-185">certificateIssuer</span></span>|<span data-ttu-id="a1e55-186">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a1e55-186">String</span></span>|<span data-ttu-id="a1e55-187">Emissor</span><span class="sxs-lookup"><span data-stu-id="a1e55-187">Issuer</span></span>|
|<span data-ttu-id="a1e55-188">certificateThumbprint</span><span class="sxs-lookup"><span data-stu-id="a1e55-188">certificateThumbprint</span></span>|<span data-ttu-id="a1e55-189">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a1e55-189">String</span></span>|<span data-ttu-id="a1e55-190">Identificação</span><span class="sxs-lookup"><span data-stu-id="a1e55-190">Thumbprint</span></span>|
|<span data-ttu-id="a1e55-191">certificateSerialNumber</span><span class="sxs-lookup"><span data-stu-id="a1e55-191">certificateSerialNumber</span></span>|<span data-ttu-id="a1e55-192">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a1e55-192">String</span></span>|<span data-ttu-id="a1e55-193">Número de série</span><span class="sxs-lookup"><span data-stu-id="a1e55-193">Serial number</span></span>|
|<span data-ttu-id="a1e55-194">certificateKeyLength</span><span class="sxs-lookup"><span data-stu-id="a1e55-194">certificateKeyLength</span></span>|<span data-ttu-id="a1e55-195">Int32</span><span class="sxs-lookup"><span data-stu-id="a1e55-195">Int32</span></span>|<span data-ttu-id="a1e55-196">Comprimento de chave</span><span class="sxs-lookup"><span data-stu-id="a1e55-196">Key length</span></span>|
|<span data-ttu-id="a1e55-197">certificateEnhancedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="a1e55-197">certificateEnhancedKeyUsage</span></span>|<span data-ttu-id="a1e55-198">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a1e55-198">String</span></span>|<span data-ttu-id="a1e55-199">Uso estendido de chave</span><span class="sxs-lookup"><span data-stu-id="a1e55-199">Extended key usage</span></span>|
|<span data-ttu-id="a1e55-200">certificateValidityPeriod</span><span class="sxs-lookup"><span data-stu-id="a1e55-200">certificateValidityPeriod</span></span>|<span data-ttu-id="a1e55-201">Int32</span><span class="sxs-lookup"><span data-stu-id="a1e55-201">Int32</span></span>|<span data-ttu-id="a1e55-202">Período de validade</span><span class="sxs-lookup"><span data-stu-id="a1e55-202">Validity period</span></span>|
|<span data-ttu-id="a1e55-203">certificateSubjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="a1e55-203">certificateSubjectNameFormatString</span></span>|<span data-ttu-id="a1e55-204">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a1e55-204">String</span></span>|<span data-ttu-id="a1e55-205">Cadeia de caracteres de formato de nome de entidade para formatos de nome de entidade personalizados</span><span class="sxs-lookup"><span data-stu-id="a1e55-205">Subject name format string for custom subject name formats</span></span>|
|<span data-ttu-id="a1e55-206">certificateSubjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="a1e55-206">certificateSubjectAlternativeNameFormatString</span></span>|<span data-ttu-id="a1e55-207">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a1e55-207">String</span></span>|<span data-ttu-id="a1e55-208">Cadeia de caracteres de formato de nome alternativo da entidade para formatos personalizados</span><span class="sxs-lookup"><span data-stu-id="a1e55-208">Subject alternative name format string for custom formats</span></span>|
|<span data-ttu-id="a1e55-209">certificateIssuanceDateTime</span><span class="sxs-lookup"><span data-stu-id="a1e55-209">certificateIssuanceDateTime</span></span>|<span data-ttu-id="a1e55-210">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1e55-210">DateTimeOffset</span></span>|<span data-ttu-id="a1e55-211">Data de emissão</span><span class="sxs-lookup"><span data-stu-id="a1e55-211">Issuance date</span></span>|
|<span data-ttu-id="a1e55-212">certificateErrorCode</span><span class="sxs-lookup"><span data-stu-id="a1e55-212">certificateErrorCode</span></span>|<span data-ttu-id="a1e55-213">Int32</span><span class="sxs-lookup"><span data-stu-id="a1e55-213">Int32</span></span>|<span data-ttu-id="a1e55-214">Código de erro</span><span class="sxs-lookup"><span data-stu-id="a1e55-214">Error code</span></span>|



## <a name="response"></a><span data-ttu-id="a1e55-215">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1e55-215">Response</span></span>
<span data-ttu-id="a1e55-216">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a1e55-216">If successful, this method returns a `200 OK` response code and an updated [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1e55-217">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a1e55-217">Example</span></span>

### <a name="request"></a><span data-ttu-id="a1e55-218">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a1e55-218">Request</span></span>
<span data-ttu-id="a1e55-219">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a1e55-219">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
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

### <a name="response"></a><span data-ttu-id="a1e55-220">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1e55-220">Response</span></span>
<span data-ttu-id="a1e55-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a1e55-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





