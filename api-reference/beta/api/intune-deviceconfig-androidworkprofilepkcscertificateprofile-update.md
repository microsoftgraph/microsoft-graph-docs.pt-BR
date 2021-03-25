---
title: Atualizar androidWorkProfilePkcsCertificateProfile
description: Atualize as propriedades de um objeto androidWorkProfilePkcsCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 842dc5776622a5a01d933443c9f4d594f743c18f
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51151792"
---
# <a name="update-androidworkprofilepkcscertificateprofile"></a><span data-ttu-id="40099-103">Atualizar androidWorkProfilePkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="40099-103">Update androidWorkProfilePkcsCertificateProfile</span></span>

<span data-ttu-id="40099-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40099-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="40099-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="40099-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="40099-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="40099-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40099-107">Atualize as propriedades de [um objeto androidWorkProfilePkcsCertificateProfile.](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="40099-107">Update the properties of a [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="40099-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="40099-108">Prerequisites</span></span>
<span data-ttu-id="40099-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40099-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40099-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="40099-111">Permission type</span></span>|<span data-ttu-id="40099-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="40099-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40099-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="40099-113">Delegated (work or school account)</span></span>|<span data-ttu-id="40099-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40099-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="40099-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="40099-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40099-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="40099-116">Not supported.</span></span>|
|<span data-ttu-id="40099-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="40099-117">Application</span></span>|<span data-ttu-id="40099-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40099-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="40099-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="40099-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="40099-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="40099-120">Request headers</span></span>
|<span data-ttu-id="40099-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="40099-121">Header</span></span>|<span data-ttu-id="40099-122">Valor</span><span class="sxs-lookup"><span data-stu-id="40099-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="40099-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="40099-123">Authorization</span></span>|<span data-ttu-id="40099-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="40099-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="40099-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="40099-125">Accept</span></span>|<span data-ttu-id="40099-126">application/json</span><span class="sxs-lookup"><span data-stu-id="40099-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="40099-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="40099-127">Request body</span></span>
<span data-ttu-id="40099-128">No corpo da solicitação, fornece uma representação JSON para o [objeto androidWorkProfilePkcsCertificateProfile.](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="40099-128">In the request body, supply a JSON representation for the [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) object.</span></span>

<span data-ttu-id="40099-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="40099-129">The following table shows the properties that are required when you create the [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md).</span></span>

|<span data-ttu-id="40099-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="40099-130">Property</span></span>|<span data-ttu-id="40099-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="40099-131">Type</span></span>|<span data-ttu-id="40099-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="40099-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40099-133">id</span><span class="sxs-lookup"><span data-stu-id="40099-133">id</span></span>|<span data-ttu-id="40099-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="40099-134">String</span></span>|<span data-ttu-id="40099-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="40099-135">Key of the entity.</span></span> <span data-ttu-id="40099-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="40099-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="40099-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="40099-137">lastModifiedDateTime</span></span>|<span data-ttu-id="40099-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40099-138">DateTimeOffset</span></span>|<span data-ttu-id="40099-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="40099-139">DateTime the object was last modified.</span></span> <span data-ttu-id="40099-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="40099-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="40099-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="40099-141">roleScopeTagIds</span></span>|<span data-ttu-id="40099-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="40099-142">String collection</span></span>|<span data-ttu-id="40099-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="40099-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="40099-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="40099-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="40099-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="40099-145">supportsScopeTags</span></span>|<span data-ttu-id="40099-146">Booleano</span><span class="sxs-lookup"><span data-stu-id="40099-146">Boolean</span></span>|<span data-ttu-id="40099-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="40099-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="40099-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="40099-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="40099-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="40099-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="40099-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="40099-150">This property is read-only.</span></span> <span data-ttu-id="40099-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="40099-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="40099-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="40099-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="40099-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="40099-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="40099-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="40099-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="40099-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="40099-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="40099-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="40099-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="40099-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="40099-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="40099-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="40099-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="40099-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="40099-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="40099-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="40099-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="40099-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="40099-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="40099-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="40099-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="40099-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="40099-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="40099-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="40099-164">createdDateTime</span></span>|<span data-ttu-id="40099-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40099-165">DateTimeOffset</span></span>|<span data-ttu-id="40099-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="40099-166">DateTime the object was created.</span></span> <span data-ttu-id="40099-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="40099-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="40099-168">descrição</span><span class="sxs-lookup"><span data-stu-id="40099-168">description</span></span>|<span data-ttu-id="40099-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="40099-169">String</span></span>|<span data-ttu-id="40099-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="40099-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="40099-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="40099-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="40099-172">displayName</span><span class="sxs-lookup"><span data-stu-id="40099-172">displayName</span></span>|<span data-ttu-id="40099-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="40099-173">String</span></span>|<span data-ttu-id="40099-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="40099-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="40099-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="40099-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="40099-176">versão</span><span class="sxs-lookup"><span data-stu-id="40099-176">version</span></span>|<span data-ttu-id="40099-177">Int32</span><span class="sxs-lookup"><span data-stu-id="40099-177">Int32</span></span>|<span data-ttu-id="40099-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="40099-178">Version of the device configuration.</span></span> <span data-ttu-id="40099-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="40099-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="40099-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="40099-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="40099-181">Int32</span><span class="sxs-lookup"><span data-stu-id="40099-181">Int32</span></span>|<span data-ttu-id="40099-182">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="40099-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="40099-183">Valores válidos de 1 a 99 Herdados [do androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="40099-183">Valid values 1 to 99 Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="40099-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="40099-184">subjectNameFormat</span></span>|[<span data-ttu-id="40099-185">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="40099-185">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="40099-186">Formato de Nome do Assunto do Certificado.</span><span class="sxs-lookup"><span data-stu-id="40099-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="40099-187">Herdado [do androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="40099-187">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="40099-188">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="40099-188">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="40099-189">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="40099-189">certificateValidityPeriodValue</span></span>|<span data-ttu-id="40099-190">Int32</span><span class="sxs-lookup"><span data-stu-id="40099-190">Int32</span></span>|<span data-ttu-id="40099-191">Valor do Período de Validade do Certificado.</span><span class="sxs-lookup"><span data-stu-id="40099-191">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="40099-192">Herdado [do androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="40099-192">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="40099-193">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="40099-193">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="40099-194">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="40099-194">certificateValidityPeriodScale</span></span>](../resources/intune-shared-certificatevalidityperiodscale.md)|<span data-ttu-id="40099-195">Dimensione para o Período de Validade do Certificado.</span><span class="sxs-lookup"><span data-stu-id="40099-195">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="40099-196">Herdado [do androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="40099-196">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="40099-197">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="40099-197">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="40099-198">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="40099-198">extendedKeyUsages</span></span>|<span data-ttu-id="40099-199">[Coleção extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="40099-199">[extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="40099-200">Configurações de Uso de Chave Estendida (EKU).</span><span class="sxs-lookup"><span data-stu-id="40099-200">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="40099-201">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="40099-201">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="40099-202">Herdado [do androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="40099-202">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="40099-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="40099-203">subjectAlternativeNameType</span></span>|[<span data-ttu-id="40099-204">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="40099-204">subjectAlternativeNameType</span></span>](../resources/intune-shared-subjectalternativenametype.md)|<span data-ttu-id="40099-205">Tipo de nome alternativo do assunto do certificado.</span><span class="sxs-lookup"><span data-stu-id="40099-205">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="40099-206">Herdado [do androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="40099-206">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="40099-207">Os possíveis valores são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span><span class="sxs-lookup"><span data-stu-id="40099-207">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span></span>|
|<span data-ttu-id="40099-208">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="40099-208">certificationAuthority</span></span>|<span data-ttu-id="40099-209">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="40099-209">String</span></span>|<span data-ttu-id="40099-210">Autoridade de Certificação PKCS</span><span class="sxs-lookup"><span data-stu-id="40099-210">PKCS Certification Authority</span></span>|
|<span data-ttu-id="40099-211">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="40099-211">certificationAuthorityName</span></span>|<span data-ttu-id="40099-212">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="40099-212">String</span></span>|<span data-ttu-id="40099-213">Nome da autoridade de certificação PKCS</span><span class="sxs-lookup"><span data-stu-id="40099-213">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="40099-214">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="40099-214">certificateTemplateName</span></span>|<span data-ttu-id="40099-215">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="40099-215">String</span></span>|<span data-ttu-id="40099-216">Nome do modelo de certificado PKCS</span><span class="sxs-lookup"><span data-stu-id="40099-216">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="40099-217">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="40099-217">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="40099-218">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="40099-218">String</span></span>|<span data-ttu-id="40099-219">Cadeia de caracteres personalizada que define o Atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="40099-219">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="40099-220">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="40099-220">subjectNameFormatString</span></span>|<span data-ttu-id="40099-221">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="40099-221">String</span></span>|<span data-ttu-id="40099-222">Formato personalizado a ser usado com SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="40099-222">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="40099-223">Exemplo: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span><span class="sxs-lookup"><span data-stu-id="40099-223">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="40099-224">certificateStore</span><span class="sxs-lookup"><span data-stu-id="40099-224">certificateStore</span></span>|[<span data-ttu-id="40099-225">certificateStore</span><span class="sxs-lookup"><span data-stu-id="40099-225">certificateStore</span></span>](../resources/intune-shared-certificatestore.md)|<span data-ttu-id="40099-226">Certificado de armazenamento de destino.</span><span class="sxs-lookup"><span data-stu-id="40099-226">Target store certificate.</span></span> <span data-ttu-id="40099-227">Os valores possíveis são: `user` e `machine`.</span><span class="sxs-lookup"><span data-stu-id="40099-227">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="40099-228">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="40099-228">customSubjectAlternativeNames</span></span>|<span data-ttu-id="40099-229">[Coleção customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="40099-229">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="40099-230">Configurações personalizadas de nome alternativo do assunto.</span><span class="sxs-lookup"><span data-stu-id="40099-230">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="40099-231">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="40099-231">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="40099-232">Resposta</span><span class="sxs-lookup"><span data-stu-id="40099-232">Response</span></span>
<span data-ttu-id="40099-233">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="40099-233">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40099-234">Exemplo</span><span class="sxs-lookup"><span data-stu-id="40099-234">Example</span></span>

### <a name="request"></a><span data-ttu-id="40099-235">Solicitação</span><span class="sxs-lookup"><span data-stu-id="40099-235">Request</span></span>
<span data-ttu-id="40099-236">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="40099-236">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="40099-237">Resposta</span><span class="sxs-lookup"><span data-stu-id="40099-237">Response</span></span>
<span data-ttu-id="40099-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="40099-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




