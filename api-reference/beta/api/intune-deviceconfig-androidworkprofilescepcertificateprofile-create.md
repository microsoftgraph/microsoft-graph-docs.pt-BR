---
title: Criar Entidadeandroidworkprofilescepcertificateprofile
description: Criar um novo objeto Entidadeandroidworkprofilescepcertificateprofile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c57b2742f8ff2faac436fe90358de1ee7f162f31
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39949970"
---
# <a name="create-androidworkprofilescepcertificateprofile"></a><span data-ttu-id="088f4-103">Criar Entidadeandroidworkprofilescepcertificateprofile</span><span class="sxs-lookup"><span data-stu-id="088f4-103">Create androidWorkProfileScepCertificateProfile</span></span>

> <span data-ttu-id="088f4-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="088f4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="088f4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="088f4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="088f4-106">Criar um novo objeto [entidadeandroidworkprofilescepcertificateprofile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="088f4-106">Create a new [androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="088f4-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="088f4-107">Prerequisites</span></span>
<span data-ttu-id="088f4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="088f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="088f4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="088f4-110">Permission type</span></span>|<span data-ttu-id="088f4-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="088f4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="088f4-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="088f4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="088f4-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="088f4-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="088f4-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="088f4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="088f4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="088f4-115">Not supported.</span></span>|
|<span data-ttu-id="088f4-116">Application</span><span class="sxs-lookup"><span data-stu-id="088f4-116">Application</span></span>|<span data-ttu-id="088f4-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="088f4-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="088f4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="088f4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="088f4-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="088f4-119">Request headers</span></span>
|<span data-ttu-id="088f4-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="088f4-120">Header</span></span>|<span data-ttu-id="088f4-121">Valor</span><span class="sxs-lookup"><span data-stu-id="088f4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="088f4-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="088f4-122">Authorization</span></span>|<span data-ttu-id="088f4-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="088f4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="088f4-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="088f4-124">Accept</span></span>|<span data-ttu-id="088f4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="088f4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="088f4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="088f4-126">Request body</span></span>
<span data-ttu-id="088f4-127">No corpo da solicitação, forneça uma representação JSON do objeto Entidadeandroidworkprofilescepcertificateprofile.</span><span class="sxs-lookup"><span data-stu-id="088f4-127">In the request body, supply a JSON representation for the androidWorkProfileScepCertificateProfile object.</span></span>

<span data-ttu-id="088f4-128">A tabela a seguir mostra as propriedades que são necessárias ao criar Entidadeandroidworkprofilescepcertificateprofile.</span><span class="sxs-lookup"><span data-stu-id="088f4-128">The following table shows the properties that are required when you create the androidWorkProfileScepCertificateProfile.</span></span>

|<span data-ttu-id="088f4-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="088f4-129">Property</span></span>|<span data-ttu-id="088f4-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="088f4-130">Type</span></span>|<span data-ttu-id="088f4-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="088f4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="088f4-132">id</span><span class="sxs-lookup"><span data-stu-id="088f4-132">id</span></span>|<span data-ttu-id="088f4-133">String</span><span class="sxs-lookup"><span data-stu-id="088f4-133">String</span></span>|<span data-ttu-id="088f4-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="088f4-134">Key of the entity.</span></span> <span data-ttu-id="088f4-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="088f4-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="088f4-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="088f4-136">lastModifiedDateTime</span></span>|<span data-ttu-id="088f4-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="088f4-137">DateTimeOffset</span></span>|<span data-ttu-id="088f4-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="088f4-138">DateTime the object was last modified.</span></span> <span data-ttu-id="088f4-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="088f4-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="088f4-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="088f4-140">roleScopeTagIds</span></span>|<span data-ttu-id="088f4-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="088f4-141">String collection</span></span>|<span data-ttu-id="088f4-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="088f4-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="088f4-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="088f4-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="088f4-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="088f4-144">supportsScopeTags</span></span>|<span data-ttu-id="088f4-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="088f4-145">Boolean</span></span>|<span data-ttu-id="088f4-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="088f4-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="088f4-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="088f4-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="088f4-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="088f4-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="088f4-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="088f4-149">This property is read-only.</span></span> <span data-ttu-id="088f4-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="088f4-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="088f4-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="088f4-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="088f4-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="088f4-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="088f4-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="088f4-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="088f4-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="088f4-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="088f4-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="088f4-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="088f4-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="088f4-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="088f4-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="088f4-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="088f4-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="088f4-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="088f4-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="088f4-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="088f4-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="088f4-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="088f4-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="088f4-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="088f4-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="088f4-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="088f4-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="088f4-163">createdDateTime</span></span>|<span data-ttu-id="088f4-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="088f4-164">DateTimeOffset</span></span>|<span data-ttu-id="088f4-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="088f4-165">DateTime the object was created.</span></span> <span data-ttu-id="088f4-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="088f4-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="088f4-167">description</span><span class="sxs-lookup"><span data-stu-id="088f4-167">description</span></span>|<span data-ttu-id="088f4-168">String</span><span class="sxs-lookup"><span data-stu-id="088f4-168">String</span></span>|<span data-ttu-id="088f4-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="088f4-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="088f4-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="088f4-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="088f4-171">displayName</span><span class="sxs-lookup"><span data-stu-id="088f4-171">displayName</span></span>|<span data-ttu-id="088f4-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="088f4-172">String</span></span>|<span data-ttu-id="088f4-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="088f4-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="088f4-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="088f4-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="088f4-175">versão</span><span class="sxs-lookup"><span data-stu-id="088f4-175">version</span></span>|<span data-ttu-id="088f4-176">Int32</span><span class="sxs-lookup"><span data-stu-id="088f4-176">Int32</span></span>|<span data-ttu-id="088f4-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="088f4-177">Version of the device configuration.</span></span> <span data-ttu-id="088f4-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="088f4-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="088f4-179">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="088f4-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="088f4-180">Int32</span><span class="sxs-lookup"><span data-stu-id="088f4-180">Int32</span></span>|<span data-ttu-id="088f4-181">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="088f4-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="088f4-182">Valores válidos de 1 a 99 herdados de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="088f4-182">Valid values 1 to 99 Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="088f4-183">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="088f4-183">subjectNameFormat</span></span>|[<span data-ttu-id="088f4-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="088f4-184">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="088f4-185">Formato do nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="088f4-185">Certificate Subject Name Format.</span></span> <span data-ttu-id="088f4-186">Herdado de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="088f4-186">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="088f4-187">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="088f4-187">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="088f4-188">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="088f4-188">certificateValidityPeriodValue</span></span>|<span data-ttu-id="088f4-189">Int32</span><span class="sxs-lookup"><span data-stu-id="088f4-189">Int32</span></span>|<span data-ttu-id="088f4-190">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="088f4-190">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="088f4-191">Herdado de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="088f4-191">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="088f4-192">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="088f4-192">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="088f4-193">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="088f4-193">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="088f4-194">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="088f4-194">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="088f4-195">Herdado de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="088f4-195">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="088f4-196">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="088f4-196">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="088f4-197">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="088f4-197">extendedKeyUsages</span></span>|<span data-ttu-id="088f4-198">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="088f4-198">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="088f4-199">Configurações de EKU (uso estendido de chave).</span><span class="sxs-lookup"><span data-stu-id="088f4-199">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="088f4-200">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="088f4-200">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="088f4-201">Herdado de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="088f4-201">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="088f4-202">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="088f4-202">subjectAlternativeNameType</span></span>|[<span data-ttu-id="088f4-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="088f4-203">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="088f4-204">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="088f4-204">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="088f4-205">Herdado de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="088f4-205">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="088f4-206">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="088f4-206">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="088f4-207">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="088f4-207">scepServerUrls</span></span>|<span data-ttu-id="088f4-208">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="088f4-208">String collection</span></span>|<span data-ttu-id="088f4-209">URL (s) do servidor de SCEP</span><span class="sxs-lookup"><span data-stu-id="088f4-209">SCEP Server Url(s)</span></span>|
|<span data-ttu-id="088f4-210">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="088f4-210">subjectNameFormatString</span></span>|<span data-ttu-id="088f4-211">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="088f4-211">String</span></span>|<span data-ttu-id="088f4-212">Formato personalizado a ser usado com SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="088f4-212">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="088f4-213">Exemplo: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = usuários corporativos, O = Contoso Corporation, L = Redmond, ST = WA, C = br</span><span class="sxs-lookup"><span data-stu-id="088f4-213">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="088f4-214">uso de</span><span class="sxs-lookup"><span data-stu-id="088f4-214">keyUsage</span></span>|[<span data-ttu-id="088f4-215">usos de</span><span class="sxs-lookup"><span data-stu-id="088f4-215">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="088f4-216">Uso da chave do SCEP.</span><span class="sxs-lookup"><span data-stu-id="088f4-216">SCEP Key Usage.</span></span> <span data-ttu-id="088f4-217">Os valores possíveis são: `keyEncipherment` e `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="088f4-217">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="088f4-218">keySize</span><span class="sxs-lookup"><span data-stu-id="088f4-218">keySize</span></span>|[<span data-ttu-id="088f4-219">keySize</span><span class="sxs-lookup"><span data-stu-id="088f4-219">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="088f4-220">Tamanho da chave SCEP.</span><span class="sxs-lookup"><span data-stu-id="088f4-220">SCEP Key Size.</span></span> <span data-ttu-id="088f4-221">Os valores possíveis são: `size1024` e `size2048`.</span><span class="sxs-lookup"><span data-stu-id="088f4-221">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="088f4-222">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="088f4-222">hashAlgorithm</span></span>|[<span data-ttu-id="088f4-223">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="088f4-223">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="088f4-224">Algoritmo de hash do SCEP.</span><span class="sxs-lookup"><span data-stu-id="088f4-224">SCEP Hash Algorithm.</span></span> <span data-ttu-id="088f4-225">Os valores possíveis são: `sha1` e `sha2`.</span><span class="sxs-lookup"><span data-stu-id="088f4-225">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="088f4-226">Subjectalternativenameformatstring foi</span><span class="sxs-lookup"><span data-stu-id="088f4-226">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="088f4-227">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="088f4-227">String</span></span>|<span data-ttu-id="088f4-228">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="088f4-228">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="088f4-229">certificateStore</span><span class="sxs-lookup"><span data-stu-id="088f4-229">certificateStore</span></span>|[<span data-ttu-id="088f4-230">certificateStore</span><span class="sxs-lookup"><span data-stu-id="088f4-230">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="088f4-231">Certificado de repositório de destino.</span><span class="sxs-lookup"><span data-stu-id="088f4-231">Target store certificate.</span></span> <span data-ttu-id="088f4-232">Os valores possíveis são: `user` e `machine`.</span><span class="sxs-lookup"><span data-stu-id="088f4-232">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="088f4-233">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="088f4-233">customSubjectAlternativeNames</span></span>|<span data-ttu-id="088f4-234">coleção [customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="088f4-234">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="088f4-235">Configurações de nome alternativo de entidade personalizada.</span><span class="sxs-lookup"><span data-stu-id="088f4-235">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="088f4-236">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="088f4-236">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="088f4-237">Resposta</span><span class="sxs-lookup"><span data-stu-id="088f4-237">Response</span></span>
<span data-ttu-id="088f4-238">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [entidadeandroidworkprofilescepcertificateprofile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="088f4-238">If successful, this method returns a `201 Created` response code and a [androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="088f4-239">Exemplo</span><span class="sxs-lookup"><span data-stu-id="088f4-239">Example</span></span>

### <a name="request"></a><span data-ttu-id="088f4-240">Solicitação</span><span class="sxs-lookup"><span data-stu-id="088f4-240">Request</span></span>
<span data-ttu-id="088f4-241">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="088f4-241">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1982

{
  "@odata.type": "#microsoft.graph.androidWorkProfileScepCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="088f4-242">Resposta</span><span class="sxs-lookup"><span data-stu-id="088f4-242">Response</span></span>
<span data-ttu-id="088f4-p125">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="088f4-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2154

{
  "@odata.type": "#microsoft.graph.androidWorkProfileScepCertificateProfile",
  "id": "6f494abf-4abf-6f49-bf4a-496fbf4a496f",
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





