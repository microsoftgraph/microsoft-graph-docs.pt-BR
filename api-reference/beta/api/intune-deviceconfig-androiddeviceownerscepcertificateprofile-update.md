---
title: Atualizar androidDeviceOwnerScepCertificateProfile
description: Atualiza as propriedades de um objeto androidDeviceOwnerScepCertificateProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 80ed9fe5db9810a3af215eeb1ff39acc7f978153
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37171453"
---
# <a name="update-androiddeviceownerscepcertificateprofile"></a><span data-ttu-id="92783-103">Atualizar androidDeviceOwnerScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="92783-103">Update androidDeviceOwnerScepCertificateProfile</span></span>

> <span data-ttu-id="92783-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="92783-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92783-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="92783-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92783-106">Atualiza as propriedades de um objeto [androidDeviceOwnerScepCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="92783-106">Update the properties of a [androidDeviceOwnerScepCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="92783-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="92783-107">Prerequisites</span></span>
<span data-ttu-id="92783-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92783-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92783-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="92783-110">Permission type</span></span>|<span data-ttu-id="92783-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="92783-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92783-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="92783-112">Delegated (work or school account)</span></span>|<span data-ttu-id="92783-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92783-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="92783-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="92783-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92783-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="92783-115">Not supported.</span></span>|
|<span data-ttu-id="92783-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="92783-116">Application</span></span>|<span data-ttu-id="92783-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92783-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="92783-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="92783-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="92783-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="92783-119">Request headers</span></span>
|<span data-ttu-id="92783-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="92783-120">Header</span></span>|<span data-ttu-id="92783-121">Valor</span><span class="sxs-lookup"><span data-stu-id="92783-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="92783-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="92783-122">Authorization</span></span>|<span data-ttu-id="92783-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="92783-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="92783-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="92783-124">Accept</span></span>|<span data-ttu-id="92783-125">application/json</span><span class="sxs-lookup"><span data-stu-id="92783-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="92783-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="92783-126">Request body</span></span>
<span data-ttu-id="92783-127">No corpo da solicitação, forneça uma representação JSON do objeto [androidDeviceOwnerScepCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="92783-127">In the request body, supply a JSON representation for the [androidDeviceOwnerScepCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerscepcertificateprofile.md) object.</span></span>

<span data-ttu-id="92783-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidDeviceOwnerScepCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerscepcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="92783-128">The following table shows the properties that are required when you create the [androidDeviceOwnerScepCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerscepcertificateprofile.md).</span></span>

|<span data-ttu-id="92783-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="92783-129">Property</span></span>|<span data-ttu-id="92783-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="92783-130">Type</span></span>|<span data-ttu-id="92783-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="92783-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92783-132">id</span><span class="sxs-lookup"><span data-stu-id="92783-132">id</span></span>|<span data-ttu-id="92783-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="92783-133">String</span></span>|<span data-ttu-id="92783-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="92783-134">Key of the entity.</span></span> <span data-ttu-id="92783-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92783-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92783-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="92783-136">lastModifiedDateTime</span></span>|<span data-ttu-id="92783-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92783-137">DateTimeOffset</span></span>|<span data-ttu-id="92783-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="92783-138">DateTime the object was last modified.</span></span> <span data-ttu-id="92783-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92783-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92783-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="92783-140">roleScopeTagIds</span></span>|<span data-ttu-id="92783-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="92783-141">String collection</span></span>|<span data-ttu-id="92783-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="92783-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="92783-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92783-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92783-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="92783-144">supportsScopeTags</span></span>|<span data-ttu-id="92783-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="92783-145">Boolean</span></span>|<span data-ttu-id="92783-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="92783-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="92783-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="92783-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="92783-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="92783-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="92783-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="92783-149">This property is read-only.</span></span> <span data-ttu-id="92783-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92783-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92783-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="92783-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="92783-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="92783-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="92783-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="92783-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="92783-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92783-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92783-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="92783-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="92783-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="92783-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="92783-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="92783-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="92783-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92783-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92783-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="92783-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="92783-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="92783-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="92783-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="92783-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="92783-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92783-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92783-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="92783-163">createdDateTime</span></span>|<span data-ttu-id="92783-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92783-164">DateTimeOffset</span></span>|<span data-ttu-id="92783-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="92783-165">DateTime the object was created.</span></span> <span data-ttu-id="92783-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92783-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92783-167">descrição</span><span class="sxs-lookup"><span data-stu-id="92783-167">description</span></span>|<span data-ttu-id="92783-168">String</span><span class="sxs-lookup"><span data-stu-id="92783-168">String</span></span>|<span data-ttu-id="92783-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="92783-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="92783-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92783-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92783-171">displayName</span><span class="sxs-lookup"><span data-stu-id="92783-171">displayName</span></span>|<span data-ttu-id="92783-172">String</span><span class="sxs-lookup"><span data-stu-id="92783-172">String</span></span>|<span data-ttu-id="92783-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="92783-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="92783-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92783-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92783-175">versão</span><span class="sxs-lookup"><span data-stu-id="92783-175">version</span></span>|<span data-ttu-id="92783-176">Int32</span><span class="sxs-lookup"><span data-stu-id="92783-176">Int32</span></span>|<span data-ttu-id="92783-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="92783-177">Version of the device configuration.</span></span> <span data-ttu-id="92783-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92783-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92783-179">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="92783-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="92783-180">Int32</span><span class="sxs-lookup"><span data-stu-id="92783-180">Int32</span></span>|<span data-ttu-id="92783-181">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="92783-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="92783-182">Valores válidos de 1 a 99 herdados de [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="92783-182">Valid values 1 to 99 Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span></span>|
|<span data-ttu-id="92783-183">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="92783-183">subjectNameFormat</span></span>|[<span data-ttu-id="92783-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="92783-184">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="92783-185">Formato do nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="92783-185">Certificate Subject Name Format.</span></span> <span data-ttu-id="92783-186">Herdado de [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="92783-186">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span></span> <span data-ttu-id="92783-187">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="92783-187">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="92783-188">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="92783-188">certificateValidityPeriodValue</span></span>|<span data-ttu-id="92783-189">Int32</span><span class="sxs-lookup"><span data-stu-id="92783-189">Int32</span></span>|<span data-ttu-id="92783-190">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="92783-190">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="92783-191">Herdado de [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="92783-191">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span></span>|
|<span data-ttu-id="92783-192">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="92783-192">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="92783-193">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="92783-193">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="92783-194">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="92783-194">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="92783-195">Herdado de [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="92783-195">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span></span> <span data-ttu-id="92783-196">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="92783-196">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="92783-197">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="92783-197">extendedKeyUsages</span></span>|<span data-ttu-id="92783-198">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="92783-198">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="92783-199">Configurações de EKU (uso estendido de chave).</span><span class="sxs-lookup"><span data-stu-id="92783-199">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="92783-200">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="92783-200">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="92783-201">Herdado de [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="92783-201">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span></span>|
|<span data-ttu-id="92783-202">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="92783-202">subjectAlternativeNameType</span></span>|[<span data-ttu-id="92783-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="92783-203">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="92783-204">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="92783-204">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="92783-205">Herdado de [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="92783-205">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span></span> <span data-ttu-id="92783-206">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="92783-206">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="92783-207">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="92783-207">scepServerUrls</span></span>|<span data-ttu-id="92783-208">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="92783-208">String collection</span></span>|<span data-ttu-id="92783-209">URL (s) do servidor de SCEP</span><span class="sxs-lookup"><span data-stu-id="92783-209">SCEP Server Url(s)</span></span>|
|<span data-ttu-id="92783-210">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="92783-210">subjectNameFormatString</span></span>|<span data-ttu-id="92783-211">String</span><span class="sxs-lookup"><span data-stu-id="92783-211">String</span></span>|<span data-ttu-id="92783-212">Formato personalizado a ser usado com SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="92783-212">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="92783-213">Exemplo: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = usuários corporativos, O = Contoso Corporation, L = Redmond, ST = WA, C = br</span><span class="sxs-lookup"><span data-stu-id="92783-213">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="92783-214">uso de</span><span class="sxs-lookup"><span data-stu-id="92783-214">keyUsage</span></span>|[<span data-ttu-id="92783-215">usos de</span><span class="sxs-lookup"><span data-stu-id="92783-215">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="92783-216">Uso da chave do SCEP.</span><span class="sxs-lookup"><span data-stu-id="92783-216">SCEP Key Usage.</span></span> <span data-ttu-id="92783-217">Os valores possíveis são: `keyEncipherment` e `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="92783-217">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="92783-218">keySize</span><span class="sxs-lookup"><span data-stu-id="92783-218">keySize</span></span>|[<span data-ttu-id="92783-219">keySize</span><span class="sxs-lookup"><span data-stu-id="92783-219">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="92783-220">Tamanho da chave SCEP.</span><span class="sxs-lookup"><span data-stu-id="92783-220">SCEP Key Size.</span></span> <span data-ttu-id="92783-221">Os valores possíveis são: `size1024` e `size2048`.</span><span class="sxs-lookup"><span data-stu-id="92783-221">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="92783-222">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="92783-222">hashAlgorithm</span></span>|[<span data-ttu-id="92783-223">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="92783-223">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="92783-224">Algoritmo de hash do SCEP.</span><span class="sxs-lookup"><span data-stu-id="92783-224">SCEP Hash Algorithm.</span></span> <span data-ttu-id="92783-225">Os valores possíveis são: `sha1` e `sha2`.</span><span class="sxs-lookup"><span data-stu-id="92783-225">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="92783-226">Subjectalternativenameformatstring foi</span><span class="sxs-lookup"><span data-stu-id="92783-226">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="92783-227">String</span><span class="sxs-lookup"><span data-stu-id="92783-227">String</span></span>|<span data-ttu-id="92783-228">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="92783-228">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="92783-229">certificateStore</span><span class="sxs-lookup"><span data-stu-id="92783-229">certificateStore</span></span>|[<span data-ttu-id="92783-230">certificateStore</span><span class="sxs-lookup"><span data-stu-id="92783-230">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="92783-231">Certificado de repositório de destino.</span><span class="sxs-lookup"><span data-stu-id="92783-231">Target store certificate.</span></span> <span data-ttu-id="92783-232">Os valores possíveis são: `user` e `machine`.</span><span class="sxs-lookup"><span data-stu-id="92783-232">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="92783-233">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="92783-233">customSubjectAlternativeNames</span></span>|<span data-ttu-id="92783-234">coleção [customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="92783-234">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="92783-235">Configurações de nome alternativo de entidade personalizada.</span><span class="sxs-lookup"><span data-stu-id="92783-235">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="92783-236">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="92783-236">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="92783-237">Resposta</span><span class="sxs-lookup"><span data-stu-id="92783-237">Response</span></span>
<span data-ttu-id="92783-238">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [androidDeviceOwnerScepCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerscepcertificateprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="92783-238">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerScepCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92783-239">Exemplo</span><span class="sxs-lookup"><span data-stu-id="92783-239">Example</span></span>

### <a name="request"></a><span data-ttu-id="92783-240">Solicitação</span><span class="sxs-lookup"><span data-stu-id="92783-240">Request</span></span>
<span data-ttu-id="92783-241">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="92783-241">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1982

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerScepCertificateProfile",
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
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
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

### <a name="response"></a><span data-ttu-id="92783-242">Resposta</span><span class="sxs-lookup"><span data-stu-id="92783-242">Response</span></span>
<span data-ttu-id="92783-p125">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="92783-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2154

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerScepCertificateProfile",
  "id": "7d8b9c9a-9c9a-7d8b-9a9c-8b7d9a9c8b7d",
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
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
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




