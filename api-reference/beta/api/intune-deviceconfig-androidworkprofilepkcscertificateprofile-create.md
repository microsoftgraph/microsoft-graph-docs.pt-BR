---
title: Criar androidWorkProfilePkcsCertificateProfile
description: Criar um novo objeto androidWorkProfilePkcsCertificateProfile.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 167b0a69d0be0ed18cf4a420b2f043f4b7207267
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42758359"
---
# <a name="create-androidworkprofilepkcscertificateprofile"></a><span data-ttu-id="30d24-103">Criar androidWorkProfilePkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="30d24-103">Create androidWorkProfilePkcsCertificateProfile</span></span>

> <span data-ttu-id="30d24-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="30d24-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="30d24-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="30d24-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="30d24-106">Criar um novo objeto [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="30d24-106">Create a new [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="30d24-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="30d24-107">Prerequisites</span></span>
<span data-ttu-id="30d24-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30d24-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30d24-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="30d24-110">Permission type</span></span>|<span data-ttu-id="30d24-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="30d24-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="30d24-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="30d24-112">Delegated (work or school account)</span></span>|<span data-ttu-id="30d24-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30d24-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="30d24-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="30d24-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="30d24-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="30d24-115">Not supported.</span></span>|
|<span data-ttu-id="30d24-116">Application</span><span class="sxs-lookup"><span data-stu-id="30d24-116">Application</span></span>|<span data-ttu-id="30d24-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30d24-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="30d24-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="30d24-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="30d24-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="30d24-119">Request headers</span></span>
|<span data-ttu-id="30d24-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="30d24-120">Header</span></span>|<span data-ttu-id="30d24-121">Valor</span><span class="sxs-lookup"><span data-stu-id="30d24-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="30d24-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="30d24-122">Authorization</span></span>|<span data-ttu-id="30d24-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="30d24-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="30d24-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="30d24-124">Accept</span></span>|<span data-ttu-id="30d24-125">application/json</span><span class="sxs-lookup"><span data-stu-id="30d24-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="30d24-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="30d24-126">Request body</span></span>
<span data-ttu-id="30d24-127">No corpo da solicitação, forneça uma representação JSON do objeto androidWorkProfilePkcsCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="30d24-127">In the request body, supply a JSON representation for the androidWorkProfilePkcsCertificateProfile object.</span></span>

<span data-ttu-id="30d24-128">A tabela a seguir mostra as propriedades que são necessárias ao criar androidWorkProfilePkcsCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="30d24-128">The following table shows the properties that are required when you create the androidWorkProfilePkcsCertificateProfile.</span></span>

|<span data-ttu-id="30d24-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="30d24-129">Property</span></span>|<span data-ttu-id="30d24-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="30d24-130">Type</span></span>|<span data-ttu-id="30d24-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="30d24-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30d24-132">id</span><span class="sxs-lookup"><span data-stu-id="30d24-132">id</span></span>|<span data-ttu-id="30d24-133">String</span><span class="sxs-lookup"><span data-stu-id="30d24-133">String</span></span>|<span data-ttu-id="30d24-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="30d24-134">Key of the entity.</span></span> <span data-ttu-id="30d24-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="30d24-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="30d24-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="30d24-136">lastModifiedDateTime</span></span>|<span data-ttu-id="30d24-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="30d24-137">DateTimeOffset</span></span>|<span data-ttu-id="30d24-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="30d24-138">DateTime the object was last modified.</span></span> <span data-ttu-id="30d24-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="30d24-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="30d24-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="30d24-140">roleScopeTagIds</span></span>|<span data-ttu-id="30d24-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="30d24-141">String collection</span></span>|<span data-ttu-id="30d24-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="30d24-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="30d24-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="30d24-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="30d24-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="30d24-144">supportsScopeTags</span></span>|<span data-ttu-id="30d24-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="30d24-145">Boolean</span></span>|<span data-ttu-id="30d24-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="30d24-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="30d24-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="30d24-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="30d24-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="30d24-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="30d24-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="30d24-149">This property is read-only.</span></span> <span data-ttu-id="30d24-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="30d24-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="30d24-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="30d24-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="30d24-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="30d24-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="30d24-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="30d24-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="30d24-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="30d24-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="30d24-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="30d24-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="30d24-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="30d24-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="30d24-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="30d24-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="30d24-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="30d24-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="30d24-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="30d24-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="30d24-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="30d24-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="30d24-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="30d24-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="30d24-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="30d24-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="30d24-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="30d24-163">createdDateTime</span></span>|<span data-ttu-id="30d24-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="30d24-164">DateTimeOffset</span></span>|<span data-ttu-id="30d24-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="30d24-165">DateTime the object was created.</span></span> <span data-ttu-id="30d24-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="30d24-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="30d24-167">description</span><span class="sxs-lookup"><span data-stu-id="30d24-167">description</span></span>|<span data-ttu-id="30d24-168">String</span><span class="sxs-lookup"><span data-stu-id="30d24-168">String</span></span>|<span data-ttu-id="30d24-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="30d24-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="30d24-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="30d24-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="30d24-171">displayName</span><span class="sxs-lookup"><span data-stu-id="30d24-171">displayName</span></span>|<span data-ttu-id="30d24-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="30d24-172">String</span></span>|<span data-ttu-id="30d24-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="30d24-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="30d24-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="30d24-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="30d24-175">versão</span><span class="sxs-lookup"><span data-stu-id="30d24-175">version</span></span>|<span data-ttu-id="30d24-176">Int32</span><span class="sxs-lookup"><span data-stu-id="30d24-176">Int32</span></span>|<span data-ttu-id="30d24-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="30d24-177">Version of the device configuration.</span></span> <span data-ttu-id="30d24-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="30d24-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="30d24-179">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="30d24-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="30d24-180">Int32</span><span class="sxs-lookup"><span data-stu-id="30d24-180">Int32</span></span>|<span data-ttu-id="30d24-181">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="30d24-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="30d24-182">Valores válidos de 1 a 99 herdados de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="30d24-182">Valid values 1 to 99 Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="30d24-183">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="30d24-183">subjectNameFormat</span></span>|[<span data-ttu-id="30d24-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="30d24-184">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="30d24-185">Formato do nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="30d24-185">Certificate Subject Name Format.</span></span> <span data-ttu-id="30d24-186">Herdado de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="30d24-186">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="30d24-187">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="30d24-187">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="30d24-188">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="30d24-188">certificateValidityPeriodValue</span></span>|<span data-ttu-id="30d24-189">Int32</span><span class="sxs-lookup"><span data-stu-id="30d24-189">Int32</span></span>|<span data-ttu-id="30d24-190">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="30d24-190">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="30d24-191">Herdado de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="30d24-191">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="30d24-192">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="30d24-192">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="30d24-193">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="30d24-193">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="30d24-194">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="30d24-194">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="30d24-195">Herdado de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="30d24-195">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="30d24-196">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="30d24-196">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="30d24-197">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="30d24-197">extendedKeyUsages</span></span>|<span data-ttu-id="30d24-198">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="30d24-198">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="30d24-199">Configurações de EKU (uso estendido de chave).</span><span class="sxs-lookup"><span data-stu-id="30d24-199">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="30d24-200">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="30d24-200">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="30d24-201">Herdado de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="30d24-201">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="30d24-202">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="30d24-202">subjectAlternativeNameType</span></span>|[<span data-ttu-id="30d24-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="30d24-203">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="30d24-204">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="30d24-204">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="30d24-205">Herdado de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="30d24-205">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="30d24-206">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="30d24-206">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="30d24-207">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="30d24-207">certificationAuthority</span></span>|<span data-ttu-id="30d24-208">String</span><span class="sxs-lookup"><span data-stu-id="30d24-208">String</span></span>|<span data-ttu-id="30d24-209">Autoridade de certificação PKCS</span><span class="sxs-lookup"><span data-stu-id="30d24-209">PKCS Certification Authority</span></span>|
|<span data-ttu-id="30d24-210">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="30d24-210">certificationAuthorityName</span></span>|<span data-ttu-id="30d24-211">String</span><span class="sxs-lookup"><span data-stu-id="30d24-211">String</span></span>|<span data-ttu-id="30d24-212">Nome da autoridade de certificação PKCS</span><span class="sxs-lookup"><span data-stu-id="30d24-212">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="30d24-213">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="30d24-213">certificateTemplateName</span></span>|<span data-ttu-id="30d24-214">String</span><span class="sxs-lookup"><span data-stu-id="30d24-214">String</span></span>|<span data-ttu-id="30d24-215">Nome do modelo de certificado PKCS</span><span class="sxs-lookup"><span data-stu-id="30d24-215">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="30d24-216">Subjectalternativenameformatstring foi</span><span class="sxs-lookup"><span data-stu-id="30d24-216">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="30d24-217">String</span><span class="sxs-lookup"><span data-stu-id="30d24-217">String</span></span>|<span data-ttu-id="30d24-218">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="30d24-218">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="30d24-219">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="30d24-219">subjectNameFormatString</span></span>|<span data-ttu-id="30d24-220">String</span><span class="sxs-lookup"><span data-stu-id="30d24-220">String</span></span>|<span data-ttu-id="30d24-221">Formato personalizado a ser usado com SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="30d24-221">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="30d24-222">Exemplo: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = usuários corporativos, O = Contoso Corporation, L = Redmond, ST = WA, C = br</span><span class="sxs-lookup"><span data-stu-id="30d24-222">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="30d24-223">certificateStore</span><span class="sxs-lookup"><span data-stu-id="30d24-223">certificateStore</span></span>|[<span data-ttu-id="30d24-224">certificateStore</span><span class="sxs-lookup"><span data-stu-id="30d24-224">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="30d24-225">Certificado de repositório de destino.</span><span class="sxs-lookup"><span data-stu-id="30d24-225">Target store certificate.</span></span> <span data-ttu-id="30d24-226">Os valores possíveis são: `user` e `machine`.</span><span class="sxs-lookup"><span data-stu-id="30d24-226">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="30d24-227">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="30d24-227">customSubjectAlternativeNames</span></span>|<span data-ttu-id="30d24-228">coleção [customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="30d24-228">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="30d24-229">Configurações de nome alternativo de entidade personalizada.</span><span class="sxs-lookup"><span data-stu-id="30d24-229">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="30d24-230">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="30d24-230">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="30d24-231">Resposta</span><span class="sxs-lookup"><span data-stu-id="30d24-231">Response</span></span>
<span data-ttu-id="30d24-232">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="30d24-232">If successful, this method returns a `201 Created` response code and a [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30d24-233">Exemplo</span><span class="sxs-lookup"><span data-stu-id="30d24-233">Example</span></span>

### <a name="request"></a><span data-ttu-id="30d24-234">Solicitação</span><span class="sxs-lookup"><span data-stu-id="30d24-234">Request</span></span>
<span data-ttu-id="30d24-235">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="30d24-235">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2032

{
  "@odata.type": "#microsoft.graph.androidWorkProfilePkcsCertificateProfile",
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
  "subjectNameFormat": "commonNameIncludingEmail",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "subjectAlternativeNameType": "emailAddress",
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

### <a name="response"></a><span data-ttu-id="30d24-236">Resposta</span><span class="sxs-lookup"><span data-stu-id="30d24-236">Response</span></span>
<span data-ttu-id="30d24-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="30d24-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2204

{
  "@odata.type": "#microsoft.graph.androidWorkProfilePkcsCertificateProfile",
  "id": "a7d4a505-a505-a7d4-05a5-d4a705a5d4a7",
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
  "subjectNameFormat": "commonNameIncludingEmail",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "subjectAlternativeNameType": "emailAddress",
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




