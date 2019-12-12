---
title: Atualizar androidWorkProfilePkcsCertificateProfile
description: Atualiza as propriedades de um objeto androidWorkProfilePkcsCertificateProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bbe8fd96ec0b6e0f51a106becf2fb1f6f4d585f9
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39949977"
---
# <a name="update-androidworkprofilepkcscertificateprofile"></a><span data-ttu-id="0ddc8-103">Atualizar androidWorkProfilePkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="0ddc8-103">Update androidWorkProfilePkcsCertificateProfile</span></span>

> <span data-ttu-id="0ddc8-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0ddc8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0ddc8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0ddc8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ddc8-106">Atualiza as propriedades de um objeto [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="0ddc8-106">Update the properties of a [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0ddc8-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0ddc8-107">Prerequisites</span></span>
<span data-ttu-id="0ddc8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ddc8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ddc8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0ddc8-110">Permission type</span></span>|<span data-ttu-id="0ddc8-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0ddc8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ddc8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0ddc8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0ddc8-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ddc8-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0ddc8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0ddc8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ddc8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0ddc8-115">Not supported.</span></span>|
|<span data-ttu-id="0ddc8-116">Application</span><span class="sxs-lookup"><span data-stu-id="0ddc8-116">Application</span></span>|<span data-ttu-id="0ddc8-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ddc8-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ddc8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0ddc8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="0ddc8-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0ddc8-119">Request headers</span></span>
|<span data-ttu-id="0ddc8-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0ddc8-120">Header</span></span>|<span data-ttu-id="0ddc8-121">Valor</span><span class="sxs-lookup"><span data-stu-id="0ddc8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0ddc8-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0ddc8-122">Authorization</span></span>|<span data-ttu-id="0ddc8-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0ddc8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0ddc8-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0ddc8-124">Accept</span></span>|<span data-ttu-id="0ddc8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0ddc8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ddc8-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0ddc8-126">Request body</span></span>
<span data-ttu-id="0ddc8-127">No corpo da solicitação, forneça uma representação JSON do objeto [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="0ddc8-127">In the request body, supply a JSON representation for the [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) object.</span></span>

<span data-ttu-id="0ddc8-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="0ddc8-128">The following table shows the properties that are required when you create the [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md).</span></span>

|<span data-ttu-id="0ddc8-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0ddc8-129">Property</span></span>|<span data-ttu-id="0ddc8-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="0ddc8-130">Type</span></span>|<span data-ttu-id="0ddc8-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ddc8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ddc8-132">id</span><span class="sxs-lookup"><span data-stu-id="0ddc8-132">id</span></span>|<span data-ttu-id="0ddc8-133">String</span><span class="sxs-lookup"><span data-stu-id="0ddc8-133">String</span></span>|<span data-ttu-id="0ddc8-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0ddc8-134">Key of the entity.</span></span> <span data-ttu-id="0ddc8-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ddc8-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ddc8-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0ddc8-136">lastModifiedDateTime</span></span>|<span data-ttu-id="0ddc8-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ddc8-137">DateTimeOffset</span></span>|<span data-ttu-id="0ddc8-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="0ddc8-138">DateTime the object was last modified.</span></span> <span data-ttu-id="0ddc8-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ddc8-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ddc8-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0ddc8-140">roleScopeTagIds</span></span>|<span data-ttu-id="0ddc8-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0ddc8-141">String collection</span></span>|<span data-ttu-id="0ddc8-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="0ddc8-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0ddc8-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ddc8-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ddc8-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="0ddc8-144">supportsScopeTags</span></span>|<span data-ttu-id="0ddc8-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ddc8-145">Boolean</span></span>|<span data-ttu-id="0ddc8-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="0ddc8-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0ddc8-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="0ddc8-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0ddc8-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="0ddc8-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0ddc8-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0ddc8-149">This property is read-only.</span></span> <span data-ttu-id="0ddc8-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ddc8-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ddc8-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0ddc8-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="0ddc8-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0ddc8-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="0ddc8-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="0ddc8-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="0ddc8-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ddc8-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ddc8-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0ddc8-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="0ddc8-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0ddc8-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="0ddc8-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="0ddc8-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="0ddc8-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ddc8-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ddc8-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="0ddc8-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="0ddc8-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="0ddc8-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="0ddc8-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="0ddc8-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="0ddc8-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ddc8-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ddc8-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0ddc8-163">createdDateTime</span></span>|<span data-ttu-id="0ddc8-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ddc8-164">DateTimeOffset</span></span>|<span data-ttu-id="0ddc8-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="0ddc8-165">DateTime the object was created.</span></span> <span data-ttu-id="0ddc8-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ddc8-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ddc8-167">description</span><span class="sxs-lookup"><span data-stu-id="0ddc8-167">description</span></span>|<span data-ttu-id="0ddc8-168">String</span><span class="sxs-lookup"><span data-stu-id="0ddc8-168">String</span></span>|<span data-ttu-id="0ddc8-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0ddc8-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0ddc8-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ddc8-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ddc8-171">displayName</span><span class="sxs-lookup"><span data-stu-id="0ddc8-171">displayName</span></span>|<span data-ttu-id="0ddc8-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0ddc8-172">String</span></span>|<span data-ttu-id="0ddc8-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0ddc8-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0ddc8-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ddc8-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ddc8-175">versão</span><span class="sxs-lookup"><span data-stu-id="0ddc8-175">version</span></span>|<span data-ttu-id="0ddc8-176">Int32</span><span class="sxs-lookup"><span data-stu-id="0ddc8-176">Int32</span></span>|<span data-ttu-id="0ddc8-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0ddc8-177">Version of the device configuration.</span></span> <span data-ttu-id="0ddc8-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ddc8-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ddc8-179">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="0ddc8-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="0ddc8-180">Int32</span><span class="sxs-lookup"><span data-stu-id="0ddc8-180">Int32</span></span>|<span data-ttu-id="0ddc8-181">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="0ddc8-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="0ddc8-182">Valores válidos de 1 a 99 herdados de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="0ddc8-182">Valid values 1 to 99 Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="0ddc8-183">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="0ddc8-183">subjectNameFormat</span></span>|[<span data-ttu-id="0ddc8-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="0ddc8-184">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="0ddc8-185">Formato do nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="0ddc8-185">Certificate Subject Name Format.</span></span> <span data-ttu-id="0ddc8-186">Herdado de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="0ddc8-186">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="0ddc8-187">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="0ddc8-187">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="0ddc8-188">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="0ddc8-188">certificateValidityPeriodValue</span></span>|<span data-ttu-id="0ddc8-189">Int32</span><span class="sxs-lookup"><span data-stu-id="0ddc8-189">Int32</span></span>|<span data-ttu-id="0ddc8-190">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="0ddc8-190">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="0ddc8-191">Herdado de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="0ddc8-191">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="0ddc8-192">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="0ddc8-192">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="0ddc8-193">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="0ddc8-193">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="0ddc8-194">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="0ddc8-194">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="0ddc8-195">Herdado de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="0ddc8-195">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="0ddc8-196">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="0ddc8-196">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="0ddc8-197">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="0ddc8-197">extendedKeyUsages</span></span>|<span data-ttu-id="0ddc8-198">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="0ddc8-198">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="0ddc8-199">Configurações de EKU (uso estendido de chave).</span><span class="sxs-lookup"><span data-stu-id="0ddc8-199">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="0ddc8-200">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="0ddc8-200">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="0ddc8-201">Herdado de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="0ddc8-201">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="0ddc8-202">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="0ddc8-202">subjectAlternativeNameType</span></span>|[<span data-ttu-id="0ddc8-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="0ddc8-203">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="0ddc8-204">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="0ddc8-204">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="0ddc8-205">Herdado de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="0ddc8-205">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="0ddc8-206">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="0ddc8-206">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="0ddc8-207">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="0ddc8-207">certificationAuthority</span></span>|<span data-ttu-id="0ddc8-208">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="0ddc8-208">String</span></span>|<span data-ttu-id="0ddc8-209">Autoridade de certificação PKCS</span><span class="sxs-lookup"><span data-stu-id="0ddc8-209">PKCS Certification Authority</span></span>|
|<span data-ttu-id="0ddc8-210">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="0ddc8-210">certificationAuthorityName</span></span>|<span data-ttu-id="0ddc8-211">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="0ddc8-211">String</span></span>|<span data-ttu-id="0ddc8-212">Nome da autoridade de certificação PKCS</span><span class="sxs-lookup"><span data-stu-id="0ddc8-212">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="0ddc8-213">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="0ddc8-213">certificateTemplateName</span></span>|<span data-ttu-id="0ddc8-214">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="0ddc8-214">String</span></span>|<span data-ttu-id="0ddc8-215">Nome do modelo de certificado PKCS</span><span class="sxs-lookup"><span data-stu-id="0ddc8-215">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="0ddc8-216">Subjectalternativenameformatstring foi</span><span class="sxs-lookup"><span data-stu-id="0ddc8-216">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="0ddc8-217">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="0ddc8-217">String</span></span>|<span data-ttu-id="0ddc8-218">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="0ddc8-218">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="0ddc8-219">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="0ddc8-219">subjectNameFormatString</span></span>|<span data-ttu-id="0ddc8-220">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="0ddc8-220">String</span></span>|<span data-ttu-id="0ddc8-221">Formato personalizado a ser usado com SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="0ddc8-221">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="0ddc8-222">Exemplo: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = usuários corporativos, O = Contoso Corporation, L = Redmond, ST = WA, C = br</span><span class="sxs-lookup"><span data-stu-id="0ddc8-222">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="0ddc8-223">certificateStore</span><span class="sxs-lookup"><span data-stu-id="0ddc8-223">certificateStore</span></span>|[<span data-ttu-id="0ddc8-224">certificateStore</span><span class="sxs-lookup"><span data-stu-id="0ddc8-224">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="0ddc8-225">Certificado de repositório de destino.</span><span class="sxs-lookup"><span data-stu-id="0ddc8-225">Target store certificate.</span></span> <span data-ttu-id="0ddc8-226">Os valores possíveis são: `user` e `machine`.</span><span class="sxs-lookup"><span data-stu-id="0ddc8-226">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="0ddc8-227">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="0ddc8-227">customSubjectAlternativeNames</span></span>|<span data-ttu-id="0ddc8-228">coleção [customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="0ddc8-228">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="0ddc8-229">Configurações de nome alternativo de entidade personalizada.</span><span class="sxs-lookup"><span data-stu-id="0ddc8-229">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="0ddc8-230">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="0ddc8-230">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="0ddc8-231">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ddc8-231">Response</span></span>
<span data-ttu-id="0ddc8-232">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0ddc8-232">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ddc8-233">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0ddc8-233">Example</span></span>

### <a name="request"></a><span data-ttu-id="0ddc8-234">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0ddc8-234">Request</span></span>
<span data-ttu-id="0ddc8-235">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0ddc8-235">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0ddc8-236">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ddc8-236">Response</span></span>
<span data-ttu-id="0ddc8-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0ddc8-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





