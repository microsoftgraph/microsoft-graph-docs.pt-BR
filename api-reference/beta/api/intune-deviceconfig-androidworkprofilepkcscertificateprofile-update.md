---
title: Atualizar androidWorkProfilePkcsCertificateProfile
description: Atualiza as propriedades de um objeto androidWorkProfilePkcsCertificateProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b2a4e9abfe01d000e7b060db03adf7e347f7d3db
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35950557"
---
# <a name="update-androidworkprofilepkcscertificateprofile"></a><span data-ttu-id="f11de-103">Atualizar androidWorkProfilePkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="f11de-103">Update androidWorkProfilePkcsCertificateProfile</span></span>

> <span data-ttu-id="f11de-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f11de-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f11de-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f11de-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f11de-106">Atualiza as propriedades de um objeto [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="f11de-106">Update the properties of a [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f11de-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f11de-107">Prerequisites</span></span>
<span data-ttu-id="f11de-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f11de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f11de-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f11de-110">Permission type</span></span>|<span data-ttu-id="f11de-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f11de-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f11de-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f11de-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f11de-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f11de-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f11de-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f11de-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f11de-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f11de-115">Not supported.</span></span>|
|<span data-ttu-id="f11de-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f11de-116">Application</span></span>|<span data-ttu-id="f11de-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f11de-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f11de-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f11de-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f11de-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f11de-119">Request headers</span></span>
|<span data-ttu-id="f11de-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f11de-120">Header</span></span>|<span data-ttu-id="f11de-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f11de-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f11de-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f11de-122">Authorization</span></span>|<span data-ttu-id="f11de-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f11de-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f11de-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f11de-124">Accept</span></span>|<span data-ttu-id="f11de-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f11de-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f11de-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f11de-126">Request body</span></span>
<span data-ttu-id="f11de-127">No corpo da solicitação, forneça uma representação JSON do objeto [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="f11de-127">In the request body, supply a JSON representation for the [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) object.</span></span>

<span data-ttu-id="f11de-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="f11de-128">The following table shows the properties that are required when you create the [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md).</span></span>

|<span data-ttu-id="f11de-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f11de-129">Property</span></span>|<span data-ttu-id="f11de-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f11de-130">Type</span></span>|<span data-ttu-id="f11de-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f11de-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f11de-132">id</span><span class="sxs-lookup"><span data-stu-id="f11de-132">id</span></span>|<span data-ttu-id="f11de-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f11de-133">String</span></span>|<span data-ttu-id="f11de-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f11de-134">Key of the entity.</span></span> <span data-ttu-id="f11de-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f11de-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f11de-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f11de-136">lastModifiedDateTime</span></span>|<span data-ttu-id="f11de-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f11de-137">DateTimeOffset</span></span>|<span data-ttu-id="f11de-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="f11de-138">DateTime the object was last modified.</span></span> <span data-ttu-id="f11de-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f11de-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f11de-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f11de-140">roleScopeTagIds</span></span>|<span data-ttu-id="f11de-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f11de-141">String collection</span></span>|<span data-ttu-id="f11de-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="f11de-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f11de-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f11de-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f11de-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f11de-144">supportsScopeTags</span></span>|<span data-ttu-id="f11de-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="f11de-145">Boolean</span></span>|<span data-ttu-id="f11de-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="f11de-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f11de-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="f11de-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f11de-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="f11de-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f11de-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f11de-149">This property is read-only.</span></span> <span data-ttu-id="f11de-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f11de-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f11de-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f11de-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="f11de-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f11de-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="f11de-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="f11de-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="f11de-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f11de-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f11de-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f11de-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="f11de-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f11de-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="f11de-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="f11de-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="f11de-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f11de-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f11de-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f11de-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="f11de-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f11de-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="f11de-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="f11de-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="f11de-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f11de-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f11de-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f11de-163">createdDateTime</span></span>|<span data-ttu-id="f11de-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f11de-164">DateTimeOffset</span></span>|<span data-ttu-id="f11de-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="f11de-165">DateTime the object was created.</span></span> <span data-ttu-id="f11de-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f11de-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f11de-167">descrição</span><span class="sxs-lookup"><span data-stu-id="f11de-167">description</span></span>|<span data-ttu-id="f11de-168">String</span><span class="sxs-lookup"><span data-stu-id="f11de-168">String</span></span>|<span data-ttu-id="f11de-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f11de-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f11de-170">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f11de-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f11de-171">displayName</span><span class="sxs-lookup"><span data-stu-id="f11de-171">displayName</span></span>|<span data-ttu-id="f11de-172">String</span><span class="sxs-lookup"><span data-stu-id="f11de-172">String</span></span>|<span data-ttu-id="f11de-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f11de-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f11de-174">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f11de-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f11de-175">versão</span><span class="sxs-lookup"><span data-stu-id="f11de-175">version</span></span>|<span data-ttu-id="f11de-176">Int32</span><span class="sxs-lookup"><span data-stu-id="f11de-176">Int32</span></span>|<span data-ttu-id="f11de-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f11de-177">Version of the device configuration.</span></span> <span data-ttu-id="f11de-178">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f11de-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f11de-179">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="f11de-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="f11de-180">Int32</span><span class="sxs-lookup"><span data-stu-id="f11de-180">Int32</span></span>|<span data-ttu-id="f11de-181">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="f11de-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="f11de-182">Valores válidos de 1 a 99 herdados de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="f11de-182">Valid values 1 to 99 Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="f11de-183">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="f11de-183">subjectNameFormat</span></span>|[<span data-ttu-id="f11de-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="f11de-184">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="f11de-185">Formato do nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="f11de-185">Certificate Subject Name Format.</span></span> <span data-ttu-id="f11de-186">Herdado de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="f11de-186">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="f11de-187">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="f11de-187">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="f11de-188">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="f11de-188">certificateValidityPeriodValue</span></span>|<span data-ttu-id="f11de-189">Int32</span><span class="sxs-lookup"><span data-stu-id="f11de-189">Int32</span></span>|<span data-ttu-id="f11de-190">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="f11de-190">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="f11de-191">Herdado de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="f11de-191">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="f11de-192">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="f11de-192">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="f11de-193">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="f11de-193">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="f11de-194">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="f11de-194">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="f11de-195">Herdado de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="f11de-195">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="f11de-196">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="f11de-196">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="f11de-197">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="f11de-197">extendedKeyUsages</span></span>|<span data-ttu-id="f11de-198">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="f11de-198">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="f11de-199">Configurações de EKU (uso estendido de chave).</span><span class="sxs-lookup"><span data-stu-id="f11de-199">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="f11de-200">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="f11de-200">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="f11de-201">Herdado de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="f11de-201">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="f11de-202">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="f11de-202">subjectAlternativeNameType</span></span>|[<span data-ttu-id="f11de-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="f11de-203">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="f11de-204">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="f11de-204">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="f11de-205">Herdado de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="f11de-205">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="f11de-206">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="f11de-206">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="f11de-207">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="f11de-207">certificationAuthority</span></span>|<span data-ttu-id="f11de-208">String</span><span class="sxs-lookup"><span data-stu-id="f11de-208">String</span></span>|<span data-ttu-id="f11de-209">Autoridade de certificação PKCS</span><span class="sxs-lookup"><span data-stu-id="f11de-209">PKCS Certification Authority</span></span>|
|<span data-ttu-id="f11de-210">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="f11de-210">certificationAuthorityName</span></span>|<span data-ttu-id="f11de-211">String</span><span class="sxs-lookup"><span data-stu-id="f11de-211">String</span></span>|<span data-ttu-id="f11de-212">Nome da autoridade de certificação PKCS</span><span class="sxs-lookup"><span data-stu-id="f11de-212">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="f11de-213">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="f11de-213">certificateTemplateName</span></span>|<span data-ttu-id="f11de-214">String</span><span class="sxs-lookup"><span data-stu-id="f11de-214">String</span></span>|<span data-ttu-id="f11de-215">Nome do modelo de certificado PKCS</span><span class="sxs-lookup"><span data-stu-id="f11de-215">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="f11de-216">Subjectalternativenameformatstring foi</span><span class="sxs-lookup"><span data-stu-id="f11de-216">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="f11de-217">String</span><span class="sxs-lookup"><span data-stu-id="f11de-217">String</span></span>|<span data-ttu-id="f11de-218">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="f11de-218">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="f11de-219">Resposta</span><span class="sxs-lookup"><span data-stu-id="f11de-219">Response</span></span>
<span data-ttu-id="f11de-220">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f11de-220">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f11de-221">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f11de-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="f11de-222">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f11de-222">Request</span></span>
<span data-ttu-id="f11de-223">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f11de-223">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1742

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
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```

### <a name="response"></a><span data-ttu-id="f11de-224">Resposta</span><span class="sxs-lookup"><span data-stu-id="f11de-224">Response</span></span>
<span data-ttu-id="f11de-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f11de-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1914

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
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```





