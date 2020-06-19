---
title: Atualizar managedDeviceCertificateState
description: Atualiza as propriedades de um objeto managedDeviceCertificateState.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bbf49fd7811ce9319d8c8425ef9c4cd0292c28b4
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792678"
---
# <a name="update-manageddevicecertificatestate"></a><span data-ttu-id="78ed6-103">Atualizar managedDeviceCertificateState</span><span class="sxs-lookup"><span data-stu-id="78ed6-103">Update managedDeviceCertificateState</span></span>

<span data-ttu-id="78ed6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78ed6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="78ed6-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="78ed6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="78ed6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="78ed6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="78ed6-107">Atualiza as propriedades de um objeto [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="78ed6-107">Update the properties of a [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="78ed6-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="78ed6-108">Prerequisites</span></span>
<span data-ttu-id="78ed6-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="78ed6-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="78ed6-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="78ed6-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78ed6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="78ed6-111">Permission type</span></span>|<span data-ttu-id="78ed6-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="78ed6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="78ed6-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="78ed6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="78ed6-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78ed6-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="78ed6-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="78ed6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="78ed6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="78ed6-116">Not supported.</span></span>|
|<span data-ttu-id="78ed6-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="78ed6-117">Application</span></span>|<span data-ttu-id="78ed6-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78ed6-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="78ed6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="78ed6-119">HTTP Request</span></span>
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
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfilePkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfileScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidForWorkImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
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
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerEnterpriseWiFiConfiguration/identityCertificateForClientAuthentication/microsoft.graph.androidDeviceOwnerPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerEnterpriseWiFiConfiguration/identityCertificateForClientAuthentication/microsoft.graph.androidDeviceOwnerScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerEnterpriseWiFiConfiguration/identityCertificateForClientAuthentication/microsoft.graph.androidDeviceOwnerImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
```

## <a name="request-headers"></a><span data-ttu-id="78ed6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="78ed6-120">Request headers</span></span>
|<span data-ttu-id="78ed6-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="78ed6-121">Header</span></span>|<span data-ttu-id="78ed6-122">Valor</span><span class="sxs-lookup"><span data-stu-id="78ed6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="78ed6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="78ed6-123">Authorization</span></span>|<span data-ttu-id="78ed6-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="78ed6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="78ed6-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="78ed6-125">Accept</span></span>|<span data-ttu-id="78ed6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="78ed6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="78ed6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="78ed6-127">Request body</span></span>
<span data-ttu-id="78ed6-128">No corpo da solicitação, forneça uma representação JSON do objeto [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="78ed6-128">In the request body, supply a JSON representation for the [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object.</span></span>

<span data-ttu-id="78ed6-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md).</span><span class="sxs-lookup"><span data-stu-id="78ed6-129">The following table shows the properties that are required when you create the [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md).</span></span>

|<span data-ttu-id="78ed6-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="78ed6-130">Property</span></span>|<span data-ttu-id="78ed6-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="78ed6-131">Type</span></span>|<span data-ttu-id="78ed6-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="78ed6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78ed6-133">id</span><span class="sxs-lookup"><span data-stu-id="78ed6-133">id</span></span>|<span data-ttu-id="78ed6-134">String</span><span class="sxs-lookup"><span data-stu-id="78ed6-134">String</span></span>|<span data-ttu-id="78ed6-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="78ed6-135">Key of the entity.</span></span>|
|<span data-ttu-id="78ed6-136">devicePlatform</span><span class="sxs-lookup"><span data-stu-id="78ed6-136">devicePlatform</span></span>|[<span data-ttu-id="78ed6-137">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="78ed6-137">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="78ed6-138">Plataforma de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="78ed6-138">Device platform.</span></span> <span data-ttu-id="78ed6-139">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="78ed6-139">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="78ed6-140">certificateKeyUsage</span><span class="sxs-lookup"><span data-stu-id="78ed6-140">certificateKeyUsage</span></span>|[<span data-ttu-id="78ed6-141">usos de</span><span class="sxs-lookup"><span data-stu-id="78ed6-141">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="78ed6-142">Uso de chave.</span><span class="sxs-lookup"><span data-stu-id="78ed6-142">Key usage.</span></span> <span data-ttu-id="78ed6-143">Os valores possíveis são: `keyEncipherment` e `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="78ed6-143">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="78ed6-144">certificateValidityPeriodUnits</span><span class="sxs-lookup"><span data-stu-id="78ed6-144">certificateValidityPeriodUnits</span></span>|[<span data-ttu-id="78ed6-145">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="78ed6-145">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="78ed6-146">Unidades de período de validade.</span><span class="sxs-lookup"><span data-stu-id="78ed6-146">Validity period units.</span></span> <span data-ttu-id="78ed6-147">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="78ed6-147">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="78ed6-148">certificateIssuanceState</span><span class="sxs-lookup"><span data-stu-id="78ed6-148">certificateIssuanceState</span></span>|[<span data-ttu-id="78ed6-149">certificateIssuanceStates</span><span class="sxs-lookup"><span data-stu-id="78ed6-149">certificateIssuanceStates</span></span>](../resources/intune-deviceconfig-certificateissuancestates.md)|<span data-ttu-id="78ed6-150">Estado de emissão.</span><span class="sxs-lookup"><span data-stu-id="78ed6-150">Issuance State.</span></span> <span data-ttu-id="78ed6-151">Os valores possíveis são:,,,,,,,,,,,,,,,,,,,, `unknown` `challengeIssued` `challengeIssueFailed` `requestCreationFailed` `requestSubmitFailed` `challengeValidationSucceeded` `challengeValidationFailed` `issueFailed` `issuePending` `issued` `responseProcessingFailed` `responsePending` `enrollmentSucceeded` , `enrollmentNotNeeded` , `revoked` ,, `removedFromCollection` `renewVerified` , `installFailed` `installed` `deleteFailed` `deleted` `renewalRequested` `requested` ,,,,,.</span><span class="sxs-lookup"><span data-stu-id="78ed6-151">Possible values are: `unknown`, `challengeIssued`, `challengeIssueFailed`, `requestCreationFailed`, `requestSubmitFailed`, `challengeValidationSucceeded`, `challengeValidationFailed`, `issueFailed`, `issuePending`, `issued`, `responseProcessingFailed`, `responsePending`, `enrollmentSucceeded`, `enrollmentNotNeeded`, `revoked`, `removedFromCollection`, `renewVerified`, `installFailed`, `installed`, `deleteFailed`, `deleted`, `renewalRequested`, `requested`.</span></span>|
|<span data-ttu-id="78ed6-152">certificateKeyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="78ed6-152">certificateKeyStorageProvider</span></span>|[<span data-ttu-id="78ed6-153">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="78ed6-153">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="78ed6-154">Provedor de armazenamento de chave.</span><span class="sxs-lookup"><span data-stu-id="78ed6-154">Key Storage Provider.</span></span> <span data-ttu-id="78ed6-155">Os valores possíveis são: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="78ed6-155">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="78ed6-156">certificateSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="78ed6-156">certificateSubjectNameFormat</span></span>|[<span data-ttu-id="78ed6-157">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="78ed6-157">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="78ed6-158">Formato do nome da entidade.</span><span class="sxs-lookup"><span data-stu-id="78ed6-158">Subject name format.</span></span> <span data-ttu-id="78ed6-159">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="78ed6-159">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="78ed6-160">certificateSubjectAlternativeNameFormat</span><span class="sxs-lookup"><span data-stu-id="78ed6-160">certificateSubjectAlternativeNameFormat</span></span>|[<span data-ttu-id="78ed6-161">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="78ed6-161">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="78ed6-162">Formato de nome alternativo da entidade.</span><span class="sxs-lookup"><span data-stu-id="78ed6-162">Subject alternative name format.</span></span> <span data-ttu-id="78ed6-163">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="78ed6-163">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="78ed6-164">certificateRevokeStatus</span><span class="sxs-lookup"><span data-stu-id="78ed6-164">certificateRevokeStatus</span></span>|[<span data-ttu-id="78ed6-165">certificateRevocationStatus</span><span class="sxs-lookup"><span data-stu-id="78ed6-165">certificateRevocationStatus</span></span>](../resources/intune-deviceconfig-certificaterevocationstatus.md)|<span data-ttu-id="78ed6-166">Revogar status.</span><span class="sxs-lookup"><span data-stu-id="78ed6-166">Revoke status.</span></span> <span data-ttu-id="78ed6-167">Os valores possíveis são: `none`, `pending`, `issued`, `failed`, `revoked`.</span><span class="sxs-lookup"><span data-stu-id="78ed6-167">Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.</span></span>|
|<span data-ttu-id="78ed6-168">certificateProfileDisplayName</span><span class="sxs-lookup"><span data-stu-id="78ed6-168">certificateProfileDisplayName</span></span>|<span data-ttu-id="78ed6-169">String</span><span class="sxs-lookup"><span data-stu-id="78ed6-169">String</span></span>|<span data-ttu-id="78ed6-170">Nome de exibição do perfil do certificado</span><span class="sxs-lookup"><span data-stu-id="78ed6-170">Certificate profile display name</span></span>|
|<span data-ttu-id="78ed6-171">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="78ed6-171">deviceDisplayName</span></span>|<span data-ttu-id="78ed6-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="78ed6-172">String</span></span>|<span data-ttu-id="78ed6-173">Nome de exibição do dispositivo</span><span class="sxs-lookup"><span data-stu-id="78ed6-173">Device display name</span></span>|
|<span data-ttu-id="78ed6-174">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="78ed6-174">userDisplayName</span></span>|<span data-ttu-id="78ed6-175">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="78ed6-175">String</span></span>|<span data-ttu-id="78ed6-176">Nome de exibição do usuário</span><span class="sxs-lookup"><span data-stu-id="78ed6-176">User display name</span></span>|
|<span data-ttu-id="78ed6-177">certificateExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="78ed6-177">certificateExpirationDateTime</span></span>|<span data-ttu-id="78ed6-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78ed6-178">DateTimeOffset</span></span>|<span data-ttu-id="78ed6-179">Data de vencimento do certificado</span><span class="sxs-lookup"><span data-stu-id="78ed6-179">Certificate expiry date</span></span>|
|<span data-ttu-id="78ed6-180">certificateLastIssuanceStateChangedDateTime</span><span class="sxs-lookup"><span data-stu-id="78ed6-180">certificateLastIssuanceStateChangedDateTime</span></span>|<span data-ttu-id="78ed6-181">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78ed6-181">DateTimeOffset</span></span>|<span data-ttu-id="78ed6-182">Última alteração no estado de emissão de certificado</span><span class="sxs-lookup"><span data-stu-id="78ed6-182">Last certificate issuance state change</span></span>|
|<span data-ttu-id="78ed6-183">lastCertificateStateChangeDateTime</span><span class="sxs-lookup"><span data-stu-id="78ed6-183">lastCertificateStateChangeDateTime</span></span>|<span data-ttu-id="78ed6-184">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78ed6-184">DateTimeOffset</span></span>|<span data-ttu-id="78ed6-185">Última alteração no estado de emissão de certificado</span><span class="sxs-lookup"><span data-stu-id="78ed6-185">Last certificate issuance state change</span></span>|
|<span data-ttu-id="78ed6-186">certificateIssuer</span><span class="sxs-lookup"><span data-stu-id="78ed6-186">certificateIssuer</span></span>|<span data-ttu-id="78ed6-187">String</span><span class="sxs-lookup"><span data-stu-id="78ed6-187">String</span></span>|<span data-ttu-id="78ed6-188">Emissor</span><span class="sxs-lookup"><span data-stu-id="78ed6-188">Issuer</span></span>|
|<span data-ttu-id="78ed6-189">certificateThumbprint</span><span class="sxs-lookup"><span data-stu-id="78ed6-189">certificateThumbprint</span></span>|<span data-ttu-id="78ed6-190">String</span><span class="sxs-lookup"><span data-stu-id="78ed6-190">String</span></span>|<span data-ttu-id="78ed6-191">Identificação</span><span class="sxs-lookup"><span data-stu-id="78ed6-191">Thumbprint</span></span>|
|<span data-ttu-id="78ed6-192">certificateSerialNumber</span><span class="sxs-lookup"><span data-stu-id="78ed6-192">certificateSerialNumber</span></span>|<span data-ttu-id="78ed6-193">String</span><span class="sxs-lookup"><span data-stu-id="78ed6-193">String</span></span>|<span data-ttu-id="78ed6-194">Número de série</span><span class="sxs-lookup"><span data-stu-id="78ed6-194">Serial number</span></span>|
|<span data-ttu-id="78ed6-195">certificateKeyLength</span><span class="sxs-lookup"><span data-stu-id="78ed6-195">certificateKeyLength</span></span>|<span data-ttu-id="78ed6-196">Int32</span><span class="sxs-lookup"><span data-stu-id="78ed6-196">Int32</span></span>|<span data-ttu-id="78ed6-197">Comprimento de chave</span><span class="sxs-lookup"><span data-stu-id="78ed6-197">Key length</span></span>|
|<span data-ttu-id="78ed6-198">certificateEnhancedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="78ed6-198">certificateEnhancedKeyUsage</span></span>|<span data-ttu-id="78ed6-199">String</span><span class="sxs-lookup"><span data-stu-id="78ed6-199">String</span></span>|<span data-ttu-id="78ed6-200">Uso estendido de chave</span><span class="sxs-lookup"><span data-stu-id="78ed6-200">Extended key usage</span></span>|
|<span data-ttu-id="78ed6-201">certificateValidityPeriod</span><span class="sxs-lookup"><span data-stu-id="78ed6-201">certificateValidityPeriod</span></span>|<span data-ttu-id="78ed6-202">Int32</span><span class="sxs-lookup"><span data-stu-id="78ed6-202">Int32</span></span>|<span data-ttu-id="78ed6-203">Período de validade</span><span class="sxs-lookup"><span data-stu-id="78ed6-203">Validity period</span></span>|
|<span data-ttu-id="78ed6-204">certificateSubjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="78ed6-204">certificateSubjectNameFormatString</span></span>|<span data-ttu-id="78ed6-205">String</span><span class="sxs-lookup"><span data-stu-id="78ed6-205">String</span></span>|<span data-ttu-id="78ed6-206">Cadeia de caracteres de formato de nome de entidade para formatos de nome de entidade personalizados</span><span class="sxs-lookup"><span data-stu-id="78ed6-206">Subject name format string for custom subject name formats</span></span>|
|<span data-ttu-id="78ed6-207">certificateSubjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="78ed6-207">certificateSubjectAlternativeNameFormatString</span></span>|<span data-ttu-id="78ed6-208">String</span><span class="sxs-lookup"><span data-stu-id="78ed6-208">String</span></span>|<span data-ttu-id="78ed6-209">Cadeia de caracteres de formato de nome alternativo da entidade para formatos personalizados</span><span class="sxs-lookup"><span data-stu-id="78ed6-209">Subject alternative name format string for custom formats</span></span>|
|<span data-ttu-id="78ed6-210">certificateIssuanceDateTime</span><span class="sxs-lookup"><span data-stu-id="78ed6-210">certificateIssuanceDateTime</span></span>|<span data-ttu-id="78ed6-211">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78ed6-211">DateTimeOffset</span></span>|<span data-ttu-id="78ed6-212">Data de emissão</span><span class="sxs-lookup"><span data-stu-id="78ed6-212">Issuance date</span></span>|
|<span data-ttu-id="78ed6-213">certificateErrorCode</span><span class="sxs-lookup"><span data-stu-id="78ed6-213">certificateErrorCode</span></span>|<span data-ttu-id="78ed6-214">Int32</span><span class="sxs-lookup"><span data-stu-id="78ed6-214">Int32</span></span>|<span data-ttu-id="78ed6-215">Código de erro</span><span class="sxs-lookup"><span data-stu-id="78ed6-215">Error code</span></span>|



## <a name="response"></a><span data-ttu-id="78ed6-216">Resposta</span><span class="sxs-lookup"><span data-stu-id="78ed6-216">Response</span></span>
<span data-ttu-id="78ed6-217">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="78ed6-217">If successful, this method returns a `200 OK` response code and an updated [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78ed6-218">Exemplo</span><span class="sxs-lookup"><span data-stu-id="78ed6-218">Example</span></span>

### <a name="request"></a><span data-ttu-id="78ed6-219">Solicitação</span><span class="sxs-lookup"><span data-stu-id="78ed6-219">Request</span></span>
<span data-ttu-id="78ed6-220">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="78ed6-220">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="78ed6-221">Resposta</span><span class="sxs-lookup"><span data-stu-id="78ed6-221">Response</span></span>
<span data-ttu-id="78ed6-222">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="78ed6-222">Here is an example of the response.</span></span> <span data-ttu-id="78ed6-223">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="78ed6-223">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="78ed6-224">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="78ed6-224">All of the properties will be returned from an actual call.</span></span>
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



