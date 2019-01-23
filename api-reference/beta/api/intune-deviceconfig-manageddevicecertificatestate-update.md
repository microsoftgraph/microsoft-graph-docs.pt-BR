---
title: Atualizar managedDeviceCertificateState
description: Atualize as propriedades de um objeto managedDeviceCertificateState.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3f092cd6adcaf1e8da0846c0ce7af354770319b2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409801"
---
# <a name="update-manageddevicecertificatestate"></a><span data-ttu-id="a16b3-103">Atualizar managedDeviceCertificateState</span><span class="sxs-lookup"><span data-stu-id="a16b3-103">Update managedDeviceCertificateState</span></span>

> <span data-ttu-id="a16b3-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="a16b3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a16b3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a16b3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a16b3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="a16b3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a16b3-107">Atualize as propriedades de um objeto [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="a16b3-107">Update the properties of a [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a16b3-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a16b3-108">Prerequisites</span></span>
<span data-ttu-id="a16b3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a16b3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a16b3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a16b3-111">Permission type</span></span>|<span data-ttu-id="a16b3-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a16b3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a16b3-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a16b3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a16b3-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a16b3-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a16b3-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a16b3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a16b3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a16b3-116">Not supported.</span></span>|
|<span data-ttu-id="a16b3-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a16b3-117">Application</span></span>|<span data-ttu-id="a16b3-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a16b3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a16b3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a16b3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfileScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidForWorkImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/microsoft.graph.windowsPhone81SCEPCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10PkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows81SCEPCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10ImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windowsPhone81ImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
```

## <a name="request-headers"></a><span data-ttu-id="a16b3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a16b3-120">Request headers</span></span>
|<span data-ttu-id="a16b3-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a16b3-121">Header</span></span>|<span data-ttu-id="a16b3-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a16b3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a16b3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a16b3-123">Authorization</span></span>|<span data-ttu-id="a16b3-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a16b3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a16b3-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a16b3-125">Accept</span></span>|<span data-ttu-id="a16b3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a16b3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a16b3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a16b3-127">Request body</span></span>
<span data-ttu-id="a16b3-128">No corpo da solicitação, fornece uma representação JSON para o objeto [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="a16b3-128">In the request body, supply a JSON representation for the [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object.</span></span>

<span data-ttu-id="a16b3-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md).</span><span class="sxs-lookup"><span data-stu-id="a16b3-129">The following table shows the properties that are required when you create the [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md).</span></span>

|<span data-ttu-id="a16b3-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a16b3-130">Property</span></span>|<span data-ttu-id="a16b3-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a16b3-131">Type</span></span>|<span data-ttu-id="a16b3-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a16b3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a16b3-133">id</span><span class="sxs-lookup"><span data-stu-id="a16b3-133">id</span></span>|<span data-ttu-id="a16b3-134">String</span><span class="sxs-lookup"><span data-stu-id="a16b3-134">String</span></span>|<span data-ttu-id="a16b3-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a16b3-135">Key of the entity.</span></span>|
|<span data-ttu-id="a16b3-136">devicePlatform</span><span class="sxs-lookup"><span data-stu-id="a16b3-136">devicePlatform</span></span>|[<span data-ttu-id="a16b3-137">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="a16b3-137">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="a16b3-138">Plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a16b3-138">Device platform.</span></span> <span data-ttu-id="a16b3-139">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span><span class="sxs-lookup"><span data-stu-id="a16b3-139">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|
|<span data-ttu-id="a16b3-140">certificateKeyUsage</span><span class="sxs-lookup"><span data-stu-id="a16b3-140">certificateKeyUsage</span></span>|[<span data-ttu-id="a16b3-141">keyUsages</span><span class="sxs-lookup"><span data-stu-id="a16b3-141">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="a16b3-142">Uso da chave.</span><span class="sxs-lookup"><span data-stu-id="a16b3-142">Key usage.</span></span> <span data-ttu-id="a16b3-143">Os valores possíveis são: `keyEncipherment` e `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="a16b3-143">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="a16b3-144">certificateValidityPeriodUnits</span><span class="sxs-lookup"><span data-stu-id="a16b3-144">certificateValidityPeriodUnits</span></span>|[<span data-ttu-id="a16b3-145">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="a16b3-145">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="a16b3-146">Unidades do período de validade.</span><span class="sxs-lookup"><span data-stu-id="a16b3-146">Validity period units.</span></span> <span data-ttu-id="a16b3-147">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="a16b3-147">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="a16b3-148">certificateIssuanceState</span><span class="sxs-lookup"><span data-stu-id="a16b3-148">certificateIssuanceState</span></span>|[<span data-ttu-id="a16b3-149">certificateIssuanceStates</span><span class="sxs-lookup"><span data-stu-id="a16b3-149">certificateIssuanceStates</span></span>](../resources/intune-deviceconfig-certificateissuancestates.md)|<span data-ttu-id="a16b3-150">Estado de emissão.</span><span class="sxs-lookup"><span data-stu-id="a16b3-150">Issuance State.</span></span> <span data-ttu-id="a16b3-151">Os valores possíveis são: `unknown`, `challengeIssued`, `challengeIssueFailed`, `requestCreationFailed`, `requestSubmitFailed`, `challengeValidationSucceeded`, `challengeValidationFailed`, `issueFailed`, `issuePending`, `issued`, `responseProcessingFailed`, `responsePending`, `enrollmentSucceeded`, `enrollmentNotNeeded`, `revoked`, `removedFromCollection`, `renewVerified`, `installFailed`, `installed` , `deleteFailed`, `deleted`, `renewalRequested`, `requested`.</span><span class="sxs-lookup"><span data-stu-id="a16b3-151">Possible values are: `unknown`, `challengeIssued`, `challengeIssueFailed`, `requestCreationFailed`, `requestSubmitFailed`, `challengeValidationSucceeded`, `challengeValidationFailed`, `issueFailed`, `issuePending`, `issued`, `responseProcessingFailed`, `responsePending`, `enrollmentSucceeded`, `enrollmentNotNeeded`, `revoked`, `removedFromCollection`, `renewVerified`, `installFailed`, `installed`, `deleteFailed`, `deleted`, `renewalRequested`, `requested`.</span></span>|
|<span data-ttu-id="a16b3-152">certificateKeyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="a16b3-152">certificateKeyStorageProvider</span></span>|[<span data-ttu-id="a16b3-153">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="a16b3-153">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="a16b3-154">Provedor de armazenamento de chave.</span><span class="sxs-lookup"><span data-stu-id="a16b3-154">Key Storage Provider.</span></span> <span data-ttu-id="a16b3-155">Os valores possíveis são: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="a16b3-155">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="a16b3-156">certificateSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="a16b3-156">certificateSubjectNameFormat</span></span>|[<span data-ttu-id="a16b3-157">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="a16b3-157">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="a16b3-158">Formato de nome de entidade.</span><span class="sxs-lookup"><span data-stu-id="a16b3-158">Subject name format.</span></span> <span data-ttu-id="a16b3-159">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="a16b3-159">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="a16b3-160">certificateSubjectAlternativeNameFormat</span><span class="sxs-lookup"><span data-stu-id="a16b3-160">certificateSubjectAlternativeNameFormat</span></span>|[<span data-ttu-id="a16b3-161">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="a16b3-161">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="a16b3-162">Formato de nome alternativo da entidade.</span><span class="sxs-lookup"><span data-stu-id="a16b3-162">Subject alternative name format.</span></span> <span data-ttu-id="a16b3-163">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="a16b3-163">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="a16b3-164">certificateRevokeStatus</span><span class="sxs-lookup"><span data-stu-id="a16b3-164">certificateRevokeStatus</span></span>|[<span data-ttu-id="a16b3-165">certificateRevocationStatus</span><span class="sxs-lookup"><span data-stu-id="a16b3-165">certificateRevocationStatus</span></span>](../resources/intune-deviceconfig-certificaterevocationstatus.md)|<span data-ttu-id="a16b3-166">Revogar o status.</span><span class="sxs-lookup"><span data-stu-id="a16b3-166">Revoke status.</span></span> <span data-ttu-id="a16b3-167">Os valores possíveis são: `none`, `pending`, `issued`, `failed`, `revoked`.</span><span class="sxs-lookup"><span data-stu-id="a16b3-167">Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.</span></span>|
|<span data-ttu-id="a16b3-168">certificateProfileDisplayName</span><span class="sxs-lookup"><span data-stu-id="a16b3-168">certificateProfileDisplayName</span></span>|<span data-ttu-id="a16b3-169">String</span><span class="sxs-lookup"><span data-stu-id="a16b3-169">String</span></span>|<span data-ttu-id="a16b3-170">Nome de exibição de perfil de certificado</span><span class="sxs-lookup"><span data-stu-id="a16b3-170">Certificate profile display name</span></span>|
|<span data-ttu-id="a16b3-171">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="a16b3-171">deviceDisplayName</span></span>|<span data-ttu-id="a16b3-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a16b3-172">String</span></span>|<span data-ttu-id="a16b3-173">Nome de exibição do dispositivo</span><span class="sxs-lookup"><span data-stu-id="a16b3-173">Device display name</span></span>|
|<span data-ttu-id="a16b3-174">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="a16b3-174">userDisplayName</span></span>|<span data-ttu-id="a16b3-175">String</span><span class="sxs-lookup"><span data-stu-id="a16b3-175">String</span></span>|<span data-ttu-id="a16b3-176">Nome de exibição do usuário</span><span class="sxs-lookup"><span data-stu-id="a16b3-176">User display name</span></span>|
|<span data-ttu-id="a16b3-177">certificateExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="a16b3-177">certificateExpirationDateTime</span></span>|<span data-ttu-id="a16b3-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a16b3-178">DateTimeOffset</span></span>|<span data-ttu-id="a16b3-179">Data de expiração de certificado</span><span class="sxs-lookup"><span data-stu-id="a16b3-179">Certificate expiry date</span></span>|
|<span data-ttu-id="a16b3-180">certificateLastIssuanceStateChangedDateTime</span><span class="sxs-lookup"><span data-stu-id="a16b3-180">certificateLastIssuanceStateChangedDateTime</span></span>|<span data-ttu-id="a16b3-181">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a16b3-181">DateTimeOffset</span></span>|<span data-ttu-id="a16b3-182">Última alteração de estado de emissão de certificado</span><span class="sxs-lookup"><span data-stu-id="a16b3-182">Last certificate issuance state change</span></span>|
|<span data-ttu-id="a16b3-183">lastCertificateStateChangeDateTime</span><span class="sxs-lookup"><span data-stu-id="a16b3-183">lastCertificateStateChangeDateTime</span></span>|<span data-ttu-id="a16b3-184">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a16b3-184">DateTimeOffset</span></span>|<span data-ttu-id="a16b3-185">Última alteração de estado de emissão de certificado</span><span class="sxs-lookup"><span data-stu-id="a16b3-185">Last certificate issuance state change</span></span>|
|<span data-ttu-id="a16b3-186">certificateIssuer</span><span class="sxs-lookup"><span data-stu-id="a16b3-186">certificateIssuer</span></span>|<span data-ttu-id="a16b3-187">String</span><span class="sxs-lookup"><span data-stu-id="a16b3-187">String</span></span>|<span data-ttu-id="a16b3-188">Emissor</span><span class="sxs-lookup"><span data-stu-id="a16b3-188">Issuer</span></span>|
|<span data-ttu-id="a16b3-189">certificateThumbprint</span><span class="sxs-lookup"><span data-stu-id="a16b3-189">certificateThumbprint</span></span>|<span data-ttu-id="a16b3-190">String</span><span class="sxs-lookup"><span data-stu-id="a16b3-190">String</span></span>|<span data-ttu-id="a16b3-191">Impressão digital</span><span class="sxs-lookup"><span data-stu-id="a16b3-191">Thumbprint</span></span>|
|<span data-ttu-id="a16b3-192">Número_serial_do_certificado</span><span class="sxs-lookup"><span data-stu-id="a16b3-192">certificateSerialNumber</span></span>|<span data-ttu-id="a16b3-193">String</span><span class="sxs-lookup"><span data-stu-id="a16b3-193">String</span></span>|<span data-ttu-id="a16b3-194">Número de série</span><span class="sxs-lookup"><span data-stu-id="a16b3-194">Serial number</span></span>|
|<span data-ttu-id="a16b3-195">certificateKeyLength</span><span class="sxs-lookup"><span data-stu-id="a16b3-195">certificateKeyLength</span></span>|<span data-ttu-id="a16b3-196">Int32</span><span class="sxs-lookup"><span data-stu-id="a16b3-196">Int32</span></span>|<span data-ttu-id="a16b3-197">Comprimento da chave</span><span class="sxs-lookup"><span data-stu-id="a16b3-197">Key length</span></span>|
|<span data-ttu-id="a16b3-198">certificateEnhancedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="a16b3-198">certificateEnhancedKeyUsage</span></span>|<span data-ttu-id="a16b3-199">String</span><span class="sxs-lookup"><span data-stu-id="a16b3-199">String</span></span>|<span data-ttu-id="a16b3-200">Uso estendido de chave</span><span class="sxs-lookup"><span data-stu-id="a16b3-200">Extended key usage</span></span>|
|<span data-ttu-id="a16b3-201">certificateValidityPeriod</span><span class="sxs-lookup"><span data-stu-id="a16b3-201">certificateValidityPeriod</span></span>|<span data-ttu-id="a16b3-202">Int32</span><span class="sxs-lookup"><span data-stu-id="a16b3-202">Int32</span></span>|<span data-ttu-id="a16b3-203">Período de validade</span><span class="sxs-lookup"><span data-stu-id="a16b3-203">Validity period</span></span>|
|<span data-ttu-id="a16b3-204">certificateSubjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="a16b3-204">certificateSubjectNameFormatString</span></span>|<span data-ttu-id="a16b3-205">String</span><span class="sxs-lookup"><span data-stu-id="a16b3-205">String</span></span>|<span data-ttu-id="a16b3-206">Sequência de formato de nome de entidade para formatos de nome de entidade personalizada</span><span class="sxs-lookup"><span data-stu-id="a16b3-206">Subject name format string for custom subject name formats</span></span>|
|<span data-ttu-id="a16b3-207">certificateSubjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="a16b3-207">certificateSubjectAlternativeNameFormatString</span></span>|<span data-ttu-id="a16b3-208">String</span><span class="sxs-lookup"><span data-stu-id="a16b3-208">String</span></span>|<span data-ttu-id="a16b3-209">Sequência de formato de nome alternativo de entidade para formatos personalizados</span><span class="sxs-lookup"><span data-stu-id="a16b3-209">Subject alternative name format string for custom formats</span></span>|
|<span data-ttu-id="a16b3-210">certificateIssuanceDateTime</span><span class="sxs-lookup"><span data-stu-id="a16b3-210">certificateIssuanceDateTime</span></span>|<span data-ttu-id="a16b3-211">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a16b3-211">DateTimeOffset</span></span>|<span data-ttu-id="a16b3-212">Data de emissão</span><span class="sxs-lookup"><span data-stu-id="a16b3-212">Issuance date</span></span>|
|<span data-ttu-id="a16b3-213">certificateErrorCode</span><span class="sxs-lookup"><span data-stu-id="a16b3-213">certificateErrorCode</span></span>|<span data-ttu-id="a16b3-214">Int32</span><span class="sxs-lookup"><span data-stu-id="a16b3-214">Int32</span></span>|<span data-ttu-id="a16b3-215">Código de erro</span><span class="sxs-lookup"><span data-stu-id="a16b3-215">Error code</span></span>|



## <a name="response"></a><span data-ttu-id="a16b3-216">Resposta</span><span class="sxs-lookup"><span data-stu-id="a16b3-216">Response</span></span>
<span data-ttu-id="a16b3-217">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a16b3-217">If successful, this method returns a `200 OK` response code and an updated [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a16b3-218">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a16b3-218">Example</span></span>

### <a name="request"></a><span data-ttu-id="a16b3-219">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a16b3-219">Request</span></span>
<span data-ttu-id="a16b3-220">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a16b3-220">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a16b3-221">Resposta</span><span class="sxs-lookup"><span data-stu-id="a16b3-221">Response</span></span>
<span data-ttu-id="a16b3-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a16b3-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




