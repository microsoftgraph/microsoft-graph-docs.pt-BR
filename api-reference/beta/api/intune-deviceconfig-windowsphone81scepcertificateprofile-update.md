---
title: Atualizar windowsPhone81SCEPCertificateProfile
description: Atualiza as propriedades de um objeto windowsPhone81SCEPCertificateProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3e6e3b57a693e6fbc6cf478c872ed6e9ecfc73d7
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36313871"
---
# <a name="update-windowsphone81scepcertificateprofile"></a><span data-ttu-id="76ef4-103">Atualizar windowsPhone81SCEPCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="76ef4-103">Update windowsPhone81SCEPCertificateProfile</span></span>

> <span data-ttu-id="76ef4-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="76ef4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="76ef4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="76ef4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76ef4-106">Atualiza as propriedades de um objeto [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="76ef4-106">Update the properties of a [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="76ef4-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="76ef4-107">Prerequisites</span></span>
<span data-ttu-id="76ef4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76ef4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76ef4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="76ef4-110">Permission type</span></span>|<span data-ttu-id="76ef4-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="76ef4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="76ef4-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="76ef4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="76ef4-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76ef4-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="76ef4-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="76ef4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="76ef4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="76ef4-115">Not supported.</span></span>|
|<span data-ttu-id="76ef4-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="76ef4-116">Application</span></span>|<span data-ttu-id="76ef4-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76ef4-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="76ef4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="76ef4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="76ef4-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="76ef4-119">Request headers</span></span>
|<span data-ttu-id="76ef4-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="76ef4-120">Header</span></span>|<span data-ttu-id="76ef4-121">Valor</span><span class="sxs-lookup"><span data-stu-id="76ef4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="76ef4-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="76ef4-122">Authorization</span></span>|<span data-ttu-id="76ef4-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="76ef4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="76ef4-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="76ef4-124">Accept</span></span>|<span data-ttu-id="76ef4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="76ef4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="76ef4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="76ef4-126">Request body</span></span>
<span data-ttu-id="76ef4-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="76ef4-127">In the request body, supply a JSON representation for the [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object.</span></span>

<span data-ttu-id="76ef4-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="76ef4-128">The following table shows the properties that are required when you create the [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md).</span></span>

|<span data-ttu-id="76ef4-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="76ef4-129">Property</span></span>|<span data-ttu-id="76ef4-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="76ef4-130">Type</span></span>|<span data-ttu-id="76ef4-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="76ef4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76ef4-132">id</span><span class="sxs-lookup"><span data-stu-id="76ef4-132">id</span></span>|<span data-ttu-id="76ef4-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="76ef4-133">String</span></span>|<span data-ttu-id="76ef4-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="76ef4-134">Key of the entity.</span></span> <span data-ttu-id="76ef4-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76ef4-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76ef4-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="76ef4-136">lastModifiedDateTime</span></span>|<span data-ttu-id="76ef4-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76ef4-137">DateTimeOffset</span></span>|<span data-ttu-id="76ef4-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="76ef4-138">DateTime the object was last modified.</span></span> <span data-ttu-id="76ef4-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76ef4-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76ef4-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="76ef4-140">roleScopeTagIds</span></span>|<span data-ttu-id="76ef4-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="76ef4-141">String collection</span></span>|<span data-ttu-id="76ef4-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="76ef4-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="76ef4-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76ef4-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76ef4-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="76ef4-144">supportsScopeTags</span></span>|<span data-ttu-id="76ef4-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="76ef4-145">Boolean</span></span>|<span data-ttu-id="76ef4-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="76ef4-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="76ef4-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="76ef4-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="76ef4-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="76ef4-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="76ef4-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="76ef4-149">This property is read-only.</span></span> <span data-ttu-id="76ef4-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76ef4-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76ef4-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="76ef4-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="76ef4-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="76ef4-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="76ef4-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="76ef4-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="76ef4-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76ef4-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76ef4-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="76ef4-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="76ef4-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="76ef4-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="76ef4-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="76ef4-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="76ef4-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76ef4-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76ef4-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="76ef4-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="76ef4-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="76ef4-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="76ef4-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="76ef4-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="76ef4-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76ef4-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76ef4-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="76ef4-163">createdDateTime</span></span>|<span data-ttu-id="76ef4-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76ef4-164">DateTimeOffset</span></span>|<span data-ttu-id="76ef4-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="76ef4-165">DateTime the object was created.</span></span> <span data-ttu-id="76ef4-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76ef4-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76ef4-167">descrição</span><span class="sxs-lookup"><span data-stu-id="76ef4-167">description</span></span>|<span data-ttu-id="76ef4-168">String</span><span class="sxs-lookup"><span data-stu-id="76ef4-168">String</span></span>|<span data-ttu-id="76ef4-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="76ef4-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="76ef4-170">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76ef4-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76ef4-171">displayName</span><span class="sxs-lookup"><span data-stu-id="76ef4-171">displayName</span></span>|<span data-ttu-id="76ef4-172">String</span><span class="sxs-lookup"><span data-stu-id="76ef4-172">String</span></span>|<span data-ttu-id="76ef4-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="76ef4-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="76ef4-174">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76ef4-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76ef4-175">versão</span><span class="sxs-lookup"><span data-stu-id="76ef4-175">version</span></span>|<span data-ttu-id="76ef4-176">Int32</span><span class="sxs-lookup"><span data-stu-id="76ef4-176">Int32</span></span>|<span data-ttu-id="76ef4-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="76ef4-177">Version of the device configuration.</span></span> <span data-ttu-id="76ef4-178">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76ef4-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76ef4-179">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="76ef4-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="76ef4-180">Int32</span><span class="sxs-lookup"><span data-stu-id="76ef4-180">Int32</span></span>|<span data-ttu-id="76ef4-181">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="76ef4-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="76ef4-182">Herdado de [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="76ef4-182">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="76ef4-183">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="76ef4-183">keyStorageProvider</span></span>|[<span data-ttu-id="76ef4-184">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="76ef4-184">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="76ef4-185">Provedor de armazenamento de chaves (KSP).</span><span class="sxs-lookup"><span data-stu-id="76ef4-185">Key Storage Provider (KSP).</span></span> <span data-ttu-id="76ef4-186">Herdado de [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="76ef4-186">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="76ef4-187">Os valores possíveis são: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="76ef4-187">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="76ef4-188">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="76ef4-188">subjectNameFormat</span></span>|[<span data-ttu-id="76ef4-189">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="76ef4-189">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="76ef4-190">Formato do nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="76ef4-190">Certificate Subject Name Format.</span></span> <span data-ttu-id="76ef4-191">Herdado de [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="76ef4-191">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="76ef4-192">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="76ef4-192">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="76ef4-193">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="76ef4-193">subjectAlternativeNameType</span></span>|[<span data-ttu-id="76ef4-194">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="76ef4-194">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="76ef4-195">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="76ef4-195">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="76ef4-196">Herdado de [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="76ef4-196">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="76ef4-197">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="76ef4-197">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="76ef4-198">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="76ef4-198">certificateValidityPeriodValue</span></span>|<span data-ttu-id="76ef4-199">Int32</span><span class="sxs-lookup"><span data-stu-id="76ef4-199">Int32</span></span>|<span data-ttu-id="76ef4-200">Valor para o período de Validtiy do certificado.</span><span class="sxs-lookup"><span data-stu-id="76ef4-200">Value for the Certificate Validtiy Period.</span></span> <span data-ttu-id="76ef4-201">Herdado de [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="76ef4-201">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="76ef4-202">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="76ef4-202">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="76ef4-203">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="76ef4-203">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="76ef4-204">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="76ef4-204">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="76ef4-205">Herdado de [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="76ef4-205">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="76ef4-206">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="76ef4-206">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="76ef4-207">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="76ef4-207">extendedKeyUsages</span></span>|<span data-ttu-id="76ef4-208">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="76ef4-208">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="76ef4-209">Configurações de EKU (uso estendido de chave).</span><span class="sxs-lookup"><span data-stu-id="76ef4-209">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="76ef4-210">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="76ef4-210">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="76ef4-211">Herdado de [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="76ef4-211">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="76ef4-212">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="76ef4-212">scepServerUrls</span></span>|<span data-ttu-id="76ef4-213">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="76ef4-213">String collection</span></span>|<span data-ttu-id="76ef4-214">URL (s) do servidor de SCEP.</span><span class="sxs-lookup"><span data-stu-id="76ef4-214">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="76ef4-215">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="76ef4-215">subjectNameFormatString</span></span>|<span data-ttu-id="76ef4-216">String</span><span class="sxs-lookup"><span data-stu-id="76ef4-216">String</span></span>|<span data-ttu-id="76ef4-217">Formato personalizado a ser usado com SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="76ef4-217">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="76ef4-218">Exemplo: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = usuários corporativos, O = Contoso Corporation, L = Redmond, ST = WA, C = br</span><span class="sxs-lookup"><span data-stu-id="76ef4-218">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="76ef4-219">uso de</span><span class="sxs-lookup"><span data-stu-id="76ef4-219">keyUsage</span></span>|[<span data-ttu-id="76ef4-220">usos de</span><span class="sxs-lookup"><span data-stu-id="76ef4-220">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="76ef4-221">Uso da chave do SCEP.</span><span class="sxs-lookup"><span data-stu-id="76ef4-221">SCEP Key Usage.</span></span> <span data-ttu-id="76ef4-222">Os valores possíveis são: `keyEncipherment` e `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="76ef4-222">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="76ef4-223">keySize</span><span class="sxs-lookup"><span data-stu-id="76ef4-223">keySize</span></span>|[<span data-ttu-id="76ef4-224">keySize</span><span class="sxs-lookup"><span data-stu-id="76ef4-224">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="76ef4-225">Tamanho da chave SCEP.</span><span class="sxs-lookup"><span data-stu-id="76ef4-225">SCEP Key Size.</span></span> <span data-ttu-id="76ef4-226">Os valores possíveis são: `size1024` e `size2048`.</span><span class="sxs-lookup"><span data-stu-id="76ef4-226">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="76ef4-227">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="76ef4-227">hashAlgorithm</span></span>|[<span data-ttu-id="76ef4-228">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="76ef4-228">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="76ef4-229">Algoritmo de hash do SCEP.</span><span class="sxs-lookup"><span data-stu-id="76ef4-229">SCEP Hash Algorithm.</span></span> <span data-ttu-id="76ef4-230">Os valores possíveis são: `sha1` e `sha2`.</span><span class="sxs-lookup"><span data-stu-id="76ef4-230">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="76ef4-231">Subjectalternativenameformatstring foi</span><span class="sxs-lookup"><span data-stu-id="76ef4-231">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="76ef4-232">String</span><span class="sxs-lookup"><span data-stu-id="76ef4-232">String</span></span>|<span data-ttu-id="76ef4-233">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="76ef4-233">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="76ef4-234">Resposta</span><span class="sxs-lookup"><span data-stu-id="76ef4-234">Response</span></span>
<span data-ttu-id="76ef4-235">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="76ef4-235">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76ef4-236">Exemplo</span><span class="sxs-lookup"><span data-stu-id="76ef4-236">Example</span></span>

### <a name="request"></a><span data-ttu-id="76ef4-237">Solicitação</span><span class="sxs-lookup"><span data-stu-id="76ef4-237">Request</span></span>
<span data-ttu-id="76ef4-238">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="76ef4-238">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="76ef4-239">Resposta</span><span class="sxs-lookup"><span data-stu-id="76ef4-239">Response</span></span>
<span data-ttu-id="76ef4-p124">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="76ef4-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






