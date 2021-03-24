---
title: Atualizar windowsPhone81SCEPCertificateProfile
description: Atualize as propriedades de um objeto windowsPhone81SCEPCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0f4be62b347f7a834c8f2000815ebc4c5defe0fa
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51147130"
---
# <a name="update-windowsphone81scepcertificateprofile"></a><span data-ttu-id="93e51-103">Atualizar windowsPhone81SCEPCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="93e51-103">Update windowsPhone81SCEPCertificateProfile</span></span>

<span data-ttu-id="93e51-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93e51-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="93e51-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="93e51-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="93e51-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="93e51-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="93e51-107">Atualize as propriedades de um [objeto windowsPhone81SCEPCertificateProfile.](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="93e51-107">Update the properties of a [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="93e51-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="93e51-108">Prerequisites</span></span>
<span data-ttu-id="93e51-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93e51-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93e51-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="93e51-111">Permission type</span></span>|<span data-ttu-id="93e51-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="93e51-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="93e51-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="93e51-113">Delegated (work or school account)</span></span>|<span data-ttu-id="93e51-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93e51-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="93e51-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="93e51-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="93e51-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="93e51-116">Not supported.</span></span>|
|<span data-ttu-id="93e51-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="93e51-117">Application</span></span>|<span data-ttu-id="93e51-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93e51-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="93e51-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="93e51-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="93e51-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="93e51-120">Request headers</span></span>
|<span data-ttu-id="93e51-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="93e51-121">Header</span></span>|<span data-ttu-id="93e51-122">Valor</span><span class="sxs-lookup"><span data-stu-id="93e51-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="93e51-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="93e51-123">Authorization</span></span>|<span data-ttu-id="93e51-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="93e51-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="93e51-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="93e51-125">Accept</span></span>|<span data-ttu-id="93e51-126">application/json</span><span class="sxs-lookup"><span data-stu-id="93e51-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="93e51-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="93e51-127">Request body</span></span>
<span data-ttu-id="93e51-128">No corpo da solicitação, fornece uma representação JSON para o [objeto windowsPhone81SCEPCertificateProfile.](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="93e51-128">In the request body, supply a JSON representation for the [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object.</span></span>

<span data-ttu-id="93e51-129">A tabela a seguir mostra as propriedades necessárias ao criar [o windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="93e51-129">The following table shows the properties that are required when you create the [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md).</span></span>

|<span data-ttu-id="93e51-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="93e51-130">Property</span></span>|<span data-ttu-id="93e51-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="93e51-131">Type</span></span>|<span data-ttu-id="93e51-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="93e51-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93e51-133">id</span><span class="sxs-lookup"><span data-stu-id="93e51-133">id</span></span>|<span data-ttu-id="93e51-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="93e51-134">String</span></span>|<span data-ttu-id="93e51-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="93e51-135">Key of the entity.</span></span> <span data-ttu-id="93e51-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="93e51-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="93e51-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="93e51-137">lastModifiedDateTime</span></span>|<span data-ttu-id="93e51-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="93e51-138">DateTimeOffset</span></span>|<span data-ttu-id="93e51-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="93e51-139">DateTime the object was last modified.</span></span> <span data-ttu-id="93e51-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="93e51-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="93e51-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="93e51-141">roleScopeTagIds</span></span>|<span data-ttu-id="93e51-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="93e51-142">String collection</span></span>|<span data-ttu-id="93e51-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="93e51-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="93e51-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="93e51-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="93e51-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="93e51-145">supportsScopeTags</span></span>|<span data-ttu-id="93e51-146">Booleano</span><span class="sxs-lookup"><span data-stu-id="93e51-146">Boolean</span></span>|<span data-ttu-id="93e51-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="93e51-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="93e51-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="93e51-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="93e51-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="93e51-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="93e51-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="93e51-150">This property is read-only.</span></span> <span data-ttu-id="93e51-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="93e51-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="93e51-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="93e51-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="93e51-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="93e51-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="93e51-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="93e51-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="93e51-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="93e51-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="93e51-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="93e51-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="93e51-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="93e51-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="93e51-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="93e51-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="93e51-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="93e51-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="93e51-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="93e51-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="93e51-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="93e51-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="93e51-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="93e51-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="93e51-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="93e51-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="93e51-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="93e51-164">createdDateTime</span></span>|<span data-ttu-id="93e51-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="93e51-165">DateTimeOffset</span></span>|<span data-ttu-id="93e51-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="93e51-166">DateTime the object was created.</span></span> <span data-ttu-id="93e51-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="93e51-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="93e51-168">descrição</span><span class="sxs-lookup"><span data-stu-id="93e51-168">description</span></span>|<span data-ttu-id="93e51-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="93e51-169">String</span></span>|<span data-ttu-id="93e51-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="93e51-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="93e51-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="93e51-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="93e51-172">displayName</span><span class="sxs-lookup"><span data-stu-id="93e51-172">displayName</span></span>|<span data-ttu-id="93e51-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="93e51-173">String</span></span>|<span data-ttu-id="93e51-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="93e51-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="93e51-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="93e51-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="93e51-176">versão</span><span class="sxs-lookup"><span data-stu-id="93e51-176">version</span></span>|<span data-ttu-id="93e51-177">Int32</span><span class="sxs-lookup"><span data-stu-id="93e51-177">Int32</span></span>|<span data-ttu-id="93e51-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="93e51-178">Version of the device configuration.</span></span> <span data-ttu-id="93e51-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="93e51-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="93e51-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="93e51-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="93e51-181">Int32</span><span class="sxs-lookup"><span data-stu-id="93e51-181">Int32</span></span>|<span data-ttu-id="93e51-182">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="93e51-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="93e51-183">Herdado [do windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="93e51-183">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="93e51-184">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="93e51-184">keyStorageProvider</span></span>|[<span data-ttu-id="93e51-185">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="93e51-185">keyStorageProviderOption</span></span>](../resources/intune-shared-keystorageprovideroption.md)|<span data-ttu-id="93e51-186">KSP (Provedor de Armazenamento de Chaves).</span><span class="sxs-lookup"><span data-stu-id="93e51-186">Key Storage Provider (KSP).</span></span> <span data-ttu-id="93e51-187">Herdado [do windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="93e51-187">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="93e51-188">Os valores possíveis são: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="93e51-188">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="93e51-189">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="93e51-189">subjectNameFormat</span></span>|[<span data-ttu-id="93e51-190">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="93e51-190">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="93e51-191">Formato de Nome do Assunto do Certificado.</span><span class="sxs-lookup"><span data-stu-id="93e51-191">Certificate Subject Name Format.</span></span> <span data-ttu-id="93e51-192">Herdado [do windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="93e51-192">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="93e51-193">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="93e51-193">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="93e51-194">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="93e51-194">subjectAlternativeNameType</span></span>|[<span data-ttu-id="93e51-195">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="93e51-195">subjectAlternativeNameType</span></span>](../resources/intune-shared-subjectalternativenametype.md)|<span data-ttu-id="93e51-196">Tipo de nome alternativo do assunto do certificado.</span><span class="sxs-lookup"><span data-stu-id="93e51-196">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="93e51-197">Herdado [do windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="93e51-197">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="93e51-198">Os possíveis valores são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span><span class="sxs-lookup"><span data-stu-id="93e51-198">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span></span>|
|<span data-ttu-id="93e51-199">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="93e51-199">certificateValidityPeriodValue</span></span>|<span data-ttu-id="93e51-200">Int32</span><span class="sxs-lookup"><span data-stu-id="93e51-200">Int32</span></span>|<span data-ttu-id="93e51-201">Valor para o Período válido do certificado.</span><span class="sxs-lookup"><span data-stu-id="93e51-201">Value for the Certificate Validtiy Period.</span></span> <span data-ttu-id="93e51-202">Herdado [do windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="93e51-202">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="93e51-203">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="93e51-203">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="93e51-204">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="93e51-204">certificateValidityPeriodScale</span></span>](../resources/intune-shared-certificatevalidityperiodscale.md)|<span data-ttu-id="93e51-205">Dimensione para o Período de Validade do Certificado.</span><span class="sxs-lookup"><span data-stu-id="93e51-205">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="93e51-206">Herdado [do windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="93e51-206">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="93e51-207">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="93e51-207">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="93e51-208">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="93e51-208">extendedKeyUsages</span></span>|<span data-ttu-id="93e51-209">[Coleção extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="93e51-209">[extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="93e51-210">Configurações de Uso de Chave Estendida (EKU).</span><span class="sxs-lookup"><span data-stu-id="93e51-210">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="93e51-211">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="93e51-211">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="93e51-212">Herdado [do windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="93e51-212">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="93e51-213">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="93e51-213">scepServerUrls</span></span>|<span data-ttu-id="93e51-214">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="93e51-214">String collection</span></span>|<span data-ttu-id="93e51-215">Url(s) do servidor SCEP.</span><span class="sxs-lookup"><span data-stu-id="93e51-215">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="93e51-216">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="93e51-216">subjectNameFormatString</span></span>|<span data-ttu-id="93e51-217">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="93e51-217">String</span></span>|<span data-ttu-id="93e51-218">Formato personalizado a ser usado com SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="93e51-218">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="93e51-219">Exemplo: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span><span class="sxs-lookup"><span data-stu-id="93e51-219">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="93e51-220">keyUsage</span><span class="sxs-lookup"><span data-stu-id="93e51-220">keyUsage</span></span>|[<span data-ttu-id="93e51-221">keyUsages</span><span class="sxs-lookup"><span data-stu-id="93e51-221">keyUsages</span></span>](../resources/intune-shared-keyusages.md)|<span data-ttu-id="93e51-222">Uso da chave SCEP.</span><span class="sxs-lookup"><span data-stu-id="93e51-222">SCEP Key Usage.</span></span> <span data-ttu-id="93e51-223">Os valores possíveis são: `keyEncipherment` e `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="93e51-223">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="93e51-224">keySize</span><span class="sxs-lookup"><span data-stu-id="93e51-224">keySize</span></span>|[<span data-ttu-id="93e51-225">keySize</span><span class="sxs-lookup"><span data-stu-id="93e51-225">keySize</span></span>](../resources/intune-shared-keysize.md)|<span data-ttu-id="93e51-226">Tamanho da chave SCEP.</span><span class="sxs-lookup"><span data-stu-id="93e51-226">SCEP Key Size.</span></span> <span data-ttu-id="93e51-227">Os valores possíveis são: `size1024`, `size2048`, `size4096`.</span><span class="sxs-lookup"><span data-stu-id="93e51-227">Possible values are: `size1024`, `size2048`, `size4096`.</span></span>|
|<span data-ttu-id="93e51-228">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="93e51-228">hashAlgorithm</span></span>|[<span data-ttu-id="93e51-229">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="93e51-229">hashAlgorithms</span></span>](../resources/intune-shared-hashalgorithms.md)|<span data-ttu-id="93e51-230">Algoritmo de hash SCEP.</span><span class="sxs-lookup"><span data-stu-id="93e51-230">SCEP Hash Algorithm.</span></span> <span data-ttu-id="93e51-231">Os valores possíveis são: `sha1` e `sha2`.</span><span class="sxs-lookup"><span data-stu-id="93e51-231">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="93e51-232">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="93e51-232">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="93e51-233">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="93e51-233">String</span></span>|<span data-ttu-id="93e51-234">Cadeia de caracteres personalizada que define o Atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="93e51-234">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="93e51-235">Resposta</span><span class="sxs-lookup"><span data-stu-id="93e51-235">Response</span></span>
<span data-ttu-id="93e51-236">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="93e51-236">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="93e51-237">Exemplo</span><span class="sxs-lookup"><span data-stu-id="93e51-237">Example</span></span>

### <a name="request"></a><span data-ttu-id="93e51-238">Solicitação</span><span class="sxs-lookup"><span data-stu-id="93e51-238">Request</span></span>
<span data-ttu-id="93e51-239">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="93e51-239">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1805

{
  "@odata.type": "#microsoft.graph.windowsPhone81SCEPCertificateProfile",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "renewalThresholdPercentage": 10,
  "keyStorageProvider": "useTpmKspOtherwiseFail",
  "subjectNameFormat": "commonNameIncludingEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```

### <a name="response"></a><span data-ttu-id="93e51-240">Resposta</span><span class="sxs-lookup"><span data-stu-id="93e51-240">Response</span></span>
<span data-ttu-id="93e51-p124">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="93e51-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1977

{
  "@odata.type": "#microsoft.graph.windowsPhone81SCEPCertificateProfile",
  "id": "f070e30e-e30e-f070-0ee3-70f00ee370f0",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "renewalThresholdPercentage": 10,
  "keyStorageProvider": "useTpmKspOtherwiseFail",
  "subjectNameFormat": "commonNameIncludingEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```




