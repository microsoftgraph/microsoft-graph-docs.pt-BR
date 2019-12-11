---
title: Atualizar iosPkcsCertificateProfile
description: Atualiza as propriedades de um objeto iosPkcsCertificateProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f6016a134aecad45edb2f2d60d5fc1a9132519c1
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39948750"
---
# <a name="update-iospkcscertificateprofile"></a><span data-ttu-id="7d7ec-103">Atualizar iosPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="7d7ec-103">Update iosPkcsCertificateProfile</span></span>

> <span data-ttu-id="7d7ec-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7d7ec-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7d7ec-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7d7ec-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7d7ec-106">Atualiza as propriedades de um objeto [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="7d7ec-106">Update the properties of a [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7d7ec-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7d7ec-107">Prerequisites</span></span>
<span data-ttu-id="7d7ec-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d7ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d7ec-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7d7ec-110">Permission type</span></span>|<span data-ttu-id="7d7ec-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7d7ec-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7d7ec-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7d7ec-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7d7ec-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d7ec-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7d7ec-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7d7ec-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7d7ec-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7d7ec-115">Not supported.</span></span>|
|<span data-ttu-id="7d7ec-116">Application</span><span class="sxs-lookup"><span data-stu-id="7d7ec-116">Application</span></span>|<span data-ttu-id="7d7ec-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d7ec-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7d7ec-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7d7ec-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="7d7ec-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7d7ec-119">Request headers</span></span>
|<span data-ttu-id="7d7ec-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7d7ec-120">Header</span></span>|<span data-ttu-id="7d7ec-121">Valor</span><span class="sxs-lookup"><span data-stu-id="7d7ec-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7d7ec-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7d7ec-122">Authorization</span></span>|<span data-ttu-id="7d7ec-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7d7ec-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7d7ec-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7d7ec-124">Accept</span></span>|<span data-ttu-id="7d7ec-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7d7ec-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d7ec-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7d7ec-126">Request body</span></span>
<span data-ttu-id="7d7ec-127">No corpo da solicitação, forneça uma representação JSON do objeto [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="7d7ec-127">In the request body, supply a JSON representation for the [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) object.</span></span>

<span data-ttu-id="7d7ec-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="7d7ec-128">The following table shows the properties that are required when you create the [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md).</span></span>

|<span data-ttu-id="7d7ec-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7d7ec-129">Property</span></span>|<span data-ttu-id="7d7ec-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="7d7ec-130">Type</span></span>|<span data-ttu-id="7d7ec-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d7ec-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d7ec-132">id</span><span class="sxs-lookup"><span data-stu-id="7d7ec-132">id</span></span>|<span data-ttu-id="7d7ec-133">String</span><span class="sxs-lookup"><span data-stu-id="7d7ec-133">String</span></span>|<span data-ttu-id="7d7ec-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="7d7ec-134">Key of the entity.</span></span> <span data-ttu-id="7d7ec-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7d7ec-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d7ec-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7d7ec-136">lastModifiedDateTime</span></span>|<span data-ttu-id="7d7ec-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d7ec-137">DateTimeOffset</span></span>|<span data-ttu-id="7d7ec-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="7d7ec-138">DateTime the object was last modified.</span></span> <span data-ttu-id="7d7ec-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7d7ec-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d7ec-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7d7ec-140">roleScopeTagIds</span></span>|<span data-ttu-id="7d7ec-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="7d7ec-141">String collection</span></span>|<span data-ttu-id="7d7ec-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="7d7ec-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="7d7ec-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7d7ec-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d7ec-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="7d7ec-144">supportsScopeTags</span></span>|<span data-ttu-id="7d7ec-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="7d7ec-145">Boolean</span></span>|<span data-ttu-id="7d7ec-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="7d7ec-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="7d7ec-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="7d7ec-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="7d7ec-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="7d7ec-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="7d7ec-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7d7ec-149">This property is read-only.</span></span> <span data-ttu-id="7d7ec-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7d7ec-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d7ec-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="7d7ec-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="7d7ec-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="7d7ec-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="7d7ec-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="7d7ec-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="7d7ec-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7d7ec-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d7ec-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="7d7ec-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="7d7ec-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="7d7ec-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="7d7ec-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="7d7ec-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="7d7ec-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7d7ec-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d7ec-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="7d7ec-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="7d7ec-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="7d7ec-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="7d7ec-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="7d7ec-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="7d7ec-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7d7ec-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d7ec-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7d7ec-163">createdDateTime</span></span>|<span data-ttu-id="7d7ec-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d7ec-164">DateTimeOffset</span></span>|<span data-ttu-id="7d7ec-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="7d7ec-165">DateTime the object was created.</span></span> <span data-ttu-id="7d7ec-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7d7ec-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d7ec-167">description</span><span class="sxs-lookup"><span data-stu-id="7d7ec-167">description</span></span>|<span data-ttu-id="7d7ec-168">String</span><span class="sxs-lookup"><span data-stu-id="7d7ec-168">String</span></span>|<span data-ttu-id="7d7ec-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7d7ec-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7d7ec-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7d7ec-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d7ec-171">displayName</span><span class="sxs-lookup"><span data-stu-id="7d7ec-171">displayName</span></span>|<span data-ttu-id="7d7ec-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7d7ec-172">String</span></span>|<span data-ttu-id="7d7ec-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7d7ec-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7d7ec-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7d7ec-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d7ec-175">versão</span><span class="sxs-lookup"><span data-stu-id="7d7ec-175">version</span></span>|<span data-ttu-id="7d7ec-176">Int32</span><span class="sxs-lookup"><span data-stu-id="7d7ec-176">Int32</span></span>|<span data-ttu-id="7d7ec-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7d7ec-177">Version of the device configuration.</span></span> <span data-ttu-id="7d7ec-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7d7ec-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d7ec-179">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="7d7ec-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="7d7ec-180">Int32</span><span class="sxs-lookup"><span data-stu-id="7d7ec-180">Int32</span></span>|<span data-ttu-id="7d7ec-181">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="7d7ec-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="7d7ec-182">Valores válidos de 1 a 99 herdados de [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="7d7ec-182">Valid values 1 to 99 Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="7d7ec-183">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="7d7ec-183">subjectNameFormat</span></span>|[<span data-ttu-id="7d7ec-184">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="7d7ec-184">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="7d7ec-185">Formato do nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="7d7ec-185">Certificate Subject Name Format.</span></span> <span data-ttu-id="7d7ec-186">Herdado de [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="7d7ec-186">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="7d7ec-187">Os possíveis valores são: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="7d7ec-187">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="7d7ec-188">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="7d7ec-188">subjectAlternativeNameType</span></span>|[<span data-ttu-id="7d7ec-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="7d7ec-189">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="7d7ec-190">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="7d7ec-190">Certificate Subject Alternative Name type.</span></span> <span data-ttu-id="7d7ec-191">Herdado de [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="7d7ec-191">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="7d7ec-192">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="7d7ec-192">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="7d7ec-193">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="7d7ec-193">certificateValidityPeriodValue</span></span>|<span data-ttu-id="7d7ec-194">Int32</span><span class="sxs-lookup"><span data-stu-id="7d7ec-194">Int32</span></span>|<span data-ttu-id="7d7ec-195">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="7d7ec-195">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="7d7ec-196">Herdado de [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="7d7ec-196">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="7d7ec-197">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="7d7ec-197">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="7d7ec-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="7d7ec-198">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="7d7ec-199">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="7d7ec-199">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="7d7ec-200">Herdado de [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="7d7ec-200">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="7d7ec-201">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="7d7ec-201">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="7d7ec-202">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="7d7ec-202">certificationAuthority</span></span>|<span data-ttu-id="7d7ec-203">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="7d7ec-203">String</span></span>|<span data-ttu-id="7d7ec-204">Autoridade de certificação PKCS.</span><span class="sxs-lookup"><span data-stu-id="7d7ec-204">PKCS Certification Authority.</span></span>|
|<span data-ttu-id="7d7ec-205">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="7d7ec-205">certificationAuthorityName</span></span>|<span data-ttu-id="7d7ec-206">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="7d7ec-206">String</span></span>|<span data-ttu-id="7d7ec-207">Nome da autoridade de certificação PKCS.</span><span class="sxs-lookup"><span data-stu-id="7d7ec-207">PKCS Certification Authority Name.</span></span>|
|<span data-ttu-id="7d7ec-208">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="7d7ec-208">certificateTemplateName</span></span>|<span data-ttu-id="7d7ec-209">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="7d7ec-209">String</span></span>|<span data-ttu-id="7d7ec-210">Nome do modelo de certificado PKCS.</span><span class="sxs-lookup"><span data-stu-id="7d7ec-210">PKCS Certificate Template Name.</span></span>|
|<span data-ttu-id="7d7ec-211">Subjectalternativenameformatstring foi</span><span class="sxs-lookup"><span data-stu-id="7d7ec-211">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="7d7ec-212">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="7d7ec-212">String</span></span>|<span data-ttu-id="7d7ec-213">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="7d7ec-213">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="7d7ec-214">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="7d7ec-214">subjectNameFormatString</span></span>|<span data-ttu-id="7d7ec-215">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="7d7ec-215">String</span></span>|<span data-ttu-id="7d7ec-216">Formato personalizado a ser usado com SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="7d7ec-216">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="7d7ec-217">Exemplo: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = usuários corporativos, O = Contoso Corporation, L = Redmond, ST = WA, C = br</span><span class="sxs-lookup"><span data-stu-id="7d7ec-217">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="7d7ec-218">certificateStore</span><span class="sxs-lookup"><span data-stu-id="7d7ec-218">certificateStore</span></span>|[<span data-ttu-id="7d7ec-219">certificateStore</span><span class="sxs-lookup"><span data-stu-id="7d7ec-219">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="7d7ec-220">Certificado de repositório de destino.</span><span class="sxs-lookup"><span data-stu-id="7d7ec-220">Target store certificate.</span></span> <span data-ttu-id="7d7ec-221">Os valores possíveis são: `user` e `machine`.</span><span class="sxs-lookup"><span data-stu-id="7d7ec-221">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="7d7ec-222">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="7d7ec-222">customSubjectAlternativeNames</span></span>|<span data-ttu-id="7d7ec-223">coleção [customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="7d7ec-223">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="7d7ec-224">Configurações de nome alternativo de entidade personalizada.</span><span class="sxs-lookup"><span data-stu-id="7d7ec-224">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="7d7ec-225">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="7d7ec-225">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="7d7ec-226">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d7ec-226">Response</span></span>
<span data-ttu-id="7d7ec-227">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7d7ec-227">If successful, this method returns a `200 OK` response code and an updated [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d7ec-228">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7d7ec-228">Example</span></span>

### <a name="request"></a><span data-ttu-id="7d7ec-229">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7d7ec-229">Request</span></span>
<span data-ttu-id="7d7ec-230">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7d7ec-230">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1824

{
  "@odata.type": "#microsoft.graph.iosPkcsCertificateProfile",
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
  "subjectNameFormat": "commonNameAsEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "subjectNameFormatString": "Subject Name Format String value",
  "certificateStore": "machine",
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="7d7ec-231">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d7ec-231">Response</span></span>
<span data-ttu-id="7d7ec-p121">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7d7ec-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1996

{
  "@odata.type": "#microsoft.graph.iosPkcsCertificateProfile",
  "id": "ed0264dd-64dd-ed02-dd64-02eddd6402ed",
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
  "subjectNameFormat": "commonNameAsEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "subjectNameFormatString": "Subject Name Format String value",
  "certificateStore": "machine",
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
    }
  ]
}
```





