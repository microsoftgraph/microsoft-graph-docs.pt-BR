---
title: Criar windowsPhone81SCEPCertificateProfile
description: Criar um novo objeto windowsPhone81SCEPCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7eb76822424a471290190f83496325edd50cce57
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43429481"
---
# <a name="create-windowsphone81scepcertificateprofile"></a><span data-ttu-id="305ae-103">Criar windowsPhone81SCEPCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="305ae-103">Create windowsPhone81SCEPCertificateProfile</span></span>

<span data-ttu-id="305ae-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="305ae-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="305ae-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="305ae-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="305ae-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="305ae-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="305ae-107">Criar um novo objeto [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="305ae-107">Create a new [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="305ae-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="305ae-108">Prerequisites</span></span>
<span data-ttu-id="305ae-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="305ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="305ae-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="305ae-111">Permission type</span></span>|<span data-ttu-id="305ae-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="305ae-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="305ae-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="305ae-113">Delegated (work or school account)</span></span>|<span data-ttu-id="305ae-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="305ae-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="305ae-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="305ae-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="305ae-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="305ae-116">Not supported.</span></span>|
|<span data-ttu-id="305ae-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="305ae-117">Application</span></span>|<span data-ttu-id="305ae-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="305ae-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="305ae-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="305ae-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="305ae-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="305ae-120">Request headers</span></span>
|<span data-ttu-id="305ae-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="305ae-121">Header</span></span>|<span data-ttu-id="305ae-122">Valor</span><span class="sxs-lookup"><span data-stu-id="305ae-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="305ae-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="305ae-123">Authorization</span></span>|<span data-ttu-id="305ae-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="305ae-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="305ae-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="305ae-125">Accept</span></span>|<span data-ttu-id="305ae-126">application/json</span><span class="sxs-lookup"><span data-stu-id="305ae-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="305ae-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="305ae-127">Request body</span></span>
<span data-ttu-id="305ae-128">No corpo da solicitação, forneça uma representação JSON do objeto windowsPhone81SCEPCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="305ae-128">In the request body, supply a JSON representation for the windowsPhone81SCEPCertificateProfile object.</span></span>

<span data-ttu-id="305ae-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsPhone81SCEPCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="305ae-129">The following table shows the properties that are required when you create the windowsPhone81SCEPCertificateProfile.</span></span>

|<span data-ttu-id="305ae-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="305ae-130">Property</span></span>|<span data-ttu-id="305ae-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="305ae-131">Type</span></span>|<span data-ttu-id="305ae-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="305ae-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="305ae-133">id</span><span class="sxs-lookup"><span data-stu-id="305ae-133">id</span></span>|<span data-ttu-id="305ae-134">String</span><span class="sxs-lookup"><span data-stu-id="305ae-134">String</span></span>|<span data-ttu-id="305ae-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="305ae-135">Key of the entity.</span></span> <span data-ttu-id="305ae-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="305ae-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="305ae-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="305ae-137">lastModifiedDateTime</span></span>|<span data-ttu-id="305ae-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="305ae-138">DateTimeOffset</span></span>|<span data-ttu-id="305ae-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="305ae-139">DateTime the object was last modified.</span></span> <span data-ttu-id="305ae-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="305ae-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="305ae-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="305ae-141">roleScopeTagIds</span></span>|<span data-ttu-id="305ae-142">Coleção String</span><span class="sxs-lookup"><span data-stu-id="305ae-142">String collection</span></span>|<span data-ttu-id="305ae-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="305ae-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="305ae-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="305ae-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="305ae-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="305ae-145">supportsScopeTags</span></span>|<span data-ttu-id="305ae-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="305ae-146">Boolean</span></span>|<span data-ttu-id="305ae-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="305ae-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="305ae-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="305ae-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="305ae-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="305ae-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="305ae-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="305ae-150">This property is read-only.</span></span> <span data-ttu-id="305ae-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="305ae-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="305ae-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="305ae-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="305ae-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="305ae-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="305ae-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="305ae-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="305ae-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="305ae-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="305ae-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="305ae-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="305ae-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="305ae-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="305ae-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="305ae-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="305ae-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="305ae-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="305ae-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="305ae-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="305ae-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="305ae-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="305ae-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="305ae-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="305ae-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="305ae-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="305ae-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="305ae-164">createdDateTime</span></span>|<span data-ttu-id="305ae-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="305ae-165">DateTimeOffset</span></span>|<span data-ttu-id="305ae-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="305ae-166">DateTime the object was created.</span></span> <span data-ttu-id="305ae-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="305ae-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="305ae-168">description</span><span class="sxs-lookup"><span data-stu-id="305ae-168">description</span></span>|<span data-ttu-id="305ae-169">String</span><span class="sxs-lookup"><span data-stu-id="305ae-169">String</span></span>|<span data-ttu-id="305ae-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="305ae-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="305ae-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="305ae-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="305ae-172">displayName</span><span class="sxs-lookup"><span data-stu-id="305ae-172">displayName</span></span>|<span data-ttu-id="305ae-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="305ae-173">String</span></span>|<span data-ttu-id="305ae-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="305ae-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="305ae-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="305ae-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="305ae-176">versão</span><span class="sxs-lookup"><span data-stu-id="305ae-176">version</span></span>|<span data-ttu-id="305ae-177">Int32</span><span class="sxs-lookup"><span data-stu-id="305ae-177">Int32</span></span>|<span data-ttu-id="305ae-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="305ae-178">Version of the device configuration.</span></span> <span data-ttu-id="305ae-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="305ae-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="305ae-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="305ae-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="305ae-181">Int32</span><span class="sxs-lookup"><span data-stu-id="305ae-181">Int32</span></span>|<span data-ttu-id="305ae-182">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="305ae-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="305ae-183">Herdado de [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="305ae-183">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="305ae-184">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="305ae-184">keyStorageProvider</span></span>|[<span data-ttu-id="305ae-185">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="305ae-185">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="305ae-186">Provedor de armazenamento de chaves (KSP).</span><span class="sxs-lookup"><span data-stu-id="305ae-186">Key Storage Provider (KSP).</span></span> <span data-ttu-id="305ae-187">Herdado de [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="305ae-187">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="305ae-188">Os valores possíveis são: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="305ae-188">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="305ae-189">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="305ae-189">subjectNameFormat</span></span>|[<span data-ttu-id="305ae-190">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="305ae-190">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="305ae-191">Formato do nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="305ae-191">Certificate Subject Name Format.</span></span> <span data-ttu-id="305ae-192">Herdado de [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="305ae-192">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="305ae-193">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="305ae-193">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="305ae-194">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="305ae-194">subjectAlternativeNameType</span></span>|[<span data-ttu-id="305ae-195">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="305ae-195">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="305ae-196">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="305ae-196">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="305ae-197">Herdado de [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="305ae-197">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="305ae-198">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="305ae-198">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="305ae-199">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="305ae-199">certificateValidityPeriodValue</span></span>|<span data-ttu-id="305ae-200">Int32</span><span class="sxs-lookup"><span data-stu-id="305ae-200">Int32</span></span>|<span data-ttu-id="305ae-201">Valor para o período de Validtiy do certificado.</span><span class="sxs-lookup"><span data-stu-id="305ae-201">Value for the Certificate Validtiy Period.</span></span> <span data-ttu-id="305ae-202">Herdado de [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="305ae-202">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="305ae-203">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="305ae-203">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="305ae-204">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="305ae-204">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="305ae-205">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="305ae-205">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="305ae-206">Herdado de [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="305ae-206">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="305ae-207">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="305ae-207">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="305ae-208">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="305ae-208">extendedKeyUsages</span></span>|<span data-ttu-id="305ae-209">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="305ae-209">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="305ae-210">Configurações de EKU (uso estendido de chave).</span><span class="sxs-lookup"><span data-stu-id="305ae-210">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="305ae-211">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="305ae-211">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="305ae-212">Herdado de [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="305ae-212">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="305ae-213">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="305ae-213">scepServerUrls</span></span>|<span data-ttu-id="305ae-214">Coleção String</span><span class="sxs-lookup"><span data-stu-id="305ae-214">String collection</span></span>|<span data-ttu-id="305ae-215">URL (s) do servidor de SCEP.</span><span class="sxs-lookup"><span data-stu-id="305ae-215">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="305ae-216">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="305ae-216">subjectNameFormatString</span></span>|<span data-ttu-id="305ae-217">String</span><span class="sxs-lookup"><span data-stu-id="305ae-217">String</span></span>|<span data-ttu-id="305ae-218">Formato personalizado a ser usado com SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="305ae-218">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="305ae-219">Exemplo: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = usuários corporativos, O = Contoso Corporation, L = Redmond, ST = WA, C = br</span><span class="sxs-lookup"><span data-stu-id="305ae-219">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="305ae-220">uso de</span><span class="sxs-lookup"><span data-stu-id="305ae-220">keyUsage</span></span>|[<span data-ttu-id="305ae-221">usos de</span><span class="sxs-lookup"><span data-stu-id="305ae-221">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="305ae-222">Uso da chave do SCEP.</span><span class="sxs-lookup"><span data-stu-id="305ae-222">SCEP Key Usage.</span></span> <span data-ttu-id="305ae-223">Os valores possíveis são: `keyEncipherment` e `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="305ae-223">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="305ae-224">keySize</span><span class="sxs-lookup"><span data-stu-id="305ae-224">keySize</span></span>|[<span data-ttu-id="305ae-225">keySize</span><span class="sxs-lookup"><span data-stu-id="305ae-225">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="305ae-226">Tamanho da chave SCEP.</span><span class="sxs-lookup"><span data-stu-id="305ae-226">SCEP Key Size.</span></span> <span data-ttu-id="305ae-227">Os valores possíveis são: `size1024` e `size2048`.</span><span class="sxs-lookup"><span data-stu-id="305ae-227">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="305ae-228">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="305ae-228">hashAlgorithm</span></span>|[<span data-ttu-id="305ae-229">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="305ae-229">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="305ae-230">Algoritmo de hash do SCEP.</span><span class="sxs-lookup"><span data-stu-id="305ae-230">SCEP Hash Algorithm.</span></span> <span data-ttu-id="305ae-231">Os valores possíveis são: `sha1` e `sha2`.</span><span class="sxs-lookup"><span data-stu-id="305ae-231">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="305ae-232">Subjectalternativenameformatstring foi</span><span class="sxs-lookup"><span data-stu-id="305ae-232">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="305ae-233">String</span><span class="sxs-lookup"><span data-stu-id="305ae-233">String</span></span>|<span data-ttu-id="305ae-234">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="305ae-234">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="305ae-235">Resposta</span><span class="sxs-lookup"><span data-stu-id="305ae-235">Response</span></span>
<span data-ttu-id="305ae-236">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="305ae-236">If successful, this method returns a `201 Created` response code and a [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="305ae-237">Exemplo</span><span class="sxs-lookup"><span data-stu-id="305ae-237">Example</span></span>

### <a name="request"></a><span data-ttu-id="305ae-238">Solicitação</span><span class="sxs-lookup"><span data-stu-id="305ae-238">Request</span></span>
<span data-ttu-id="305ae-239">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="305ae-239">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="305ae-240">Resposta</span><span class="sxs-lookup"><span data-stu-id="305ae-240">Response</span></span>
<span data-ttu-id="305ae-p124">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="305ae-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



