---
title: Criar androidImportedPFXCertificateProfile
description: Criar um novo objeto androidImportedPFXCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3951f0aedf6305d39038f94abe0458fadf288acb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48025120"
---
# <a name="create-androidimportedpfxcertificateprofile"></a><span data-ttu-id="c94b6-103">Criar androidImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="c94b6-103">Create androidImportedPFXCertificateProfile</span></span>

<span data-ttu-id="c94b6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c94b6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c94b6-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c94b6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c94b6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c94b6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c94b6-107">Criar um novo objeto [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="c94b6-107">Create a new [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c94b6-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c94b6-108">Prerequisites</span></span>
<span data-ttu-id="c94b6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c94b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c94b6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c94b6-111">Permission type</span></span>|<span data-ttu-id="c94b6-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c94b6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c94b6-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c94b6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c94b6-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c94b6-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c94b6-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c94b6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c94b6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c94b6-116">Not supported.</span></span>|
|<span data-ttu-id="c94b6-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c94b6-117">Application</span></span>|<span data-ttu-id="c94b6-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c94b6-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c94b6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c94b6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c94b6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c94b6-120">Request headers</span></span>
|<span data-ttu-id="c94b6-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c94b6-121">Header</span></span>|<span data-ttu-id="c94b6-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c94b6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c94b6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c94b6-123">Authorization</span></span>|<span data-ttu-id="c94b6-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c94b6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c94b6-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c94b6-125">Accept</span></span>|<span data-ttu-id="c94b6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c94b6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c94b6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c94b6-127">Request body</span></span>
<span data-ttu-id="c94b6-128">No corpo da solicitação, forneça uma representação JSON do objeto androidImportedPFXCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="c94b6-128">In the request body, supply a JSON representation for the androidImportedPFXCertificateProfile object.</span></span>

<span data-ttu-id="c94b6-129">A tabela a seguir mostra as propriedades que são necessárias ao criar androidImportedPFXCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="c94b6-129">The following table shows the properties that are required when you create the androidImportedPFXCertificateProfile.</span></span>

|<span data-ttu-id="c94b6-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c94b6-130">Property</span></span>|<span data-ttu-id="c94b6-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c94b6-131">Type</span></span>|<span data-ttu-id="c94b6-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c94b6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c94b6-133">id</span><span class="sxs-lookup"><span data-stu-id="c94b6-133">id</span></span>|<span data-ttu-id="c94b6-134">String</span><span class="sxs-lookup"><span data-stu-id="c94b6-134">String</span></span>|<span data-ttu-id="c94b6-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c94b6-135">Key of the entity.</span></span> <span data-ttu-id="c94b6-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c94b6-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c94b6-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c94b6-137">lastModifiedDateTime</span></span>|<span data-ttu-id="c94b6-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c94b6-138">DateTimeOffset</span></span>|<span data-ttu-id="c94b6-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="c94b6-139">DateTime the object was last modified.</span></span> <span data-ttu-id="c94b6-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c94b6-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c94b6-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c94b6-141">roleScopeTagIds</span></span>|<span data-ttu-id="c94b6-142">Coleção String</span><span class="sxs-lookup"><span data-stu-id="c94b6-142">String collection</span></span>|<span data-ttu-id="c94b6-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="c94b6-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c94b6-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c94b6-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c94b6-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c94b6-145">supportsScopeTags</span></span>|<span data-ttu-id="c94b6-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="c94b6-146">Boolean</span></span>|<span data-ttu-id="c94b6-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="c94b6-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c94b6-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="c94b6-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c94b6-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="c94b6-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c94b6-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c94b6-150">This property is read-only.</span></span> <span data-ttu-id="c94b6-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c94b6-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c94b6-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c94b6-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="c94b6-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c94b6-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="c94b6-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="c94b6-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="c94b6-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c94b6-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c94b6-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c94b6-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="c94b6-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c94b6-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="c94b6-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="c94b6-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="c94b6-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c94b6-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c94b6-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c94b6-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="c94b6-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c94b6-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="c94b6-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="c94b6-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="c94b6-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c94b6-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c94b6-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c94b6-164">createdDateTime</span></span>|<span data-ttu-id="c94b6-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c94b6-165">DateTimeOffset</span></span>|<span data-ttu-id="c94b6-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="c94b6-166">DateTime the object was created.</span></span> <span data-ttu-id="c94b6-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c94b6-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c94b6-168">description</span><span class="sxs-lookup"><span data-stu-id="c94b6-168">description</span></span>|<span data-ttu-id="c94b6-169">String</span><span class="sxs-lookup"><span data-stu-id="c94b6-169">String</span></span>|<span data-ttu-id="c94b6-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c94b6-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c94b6-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c94b6-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c94b6-172">displayName</span><span class="sxs-lookup"><span data-stu-id="c94b6-172">displayName</span></span>|<span data-ttu-id="c94b6-173">String</span><span class="sxs-lookup"><span data-stu-id="c94b6-173">String</span></span>|<span data-ttu-id="c94b6-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c94b6-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c94b6-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c94b6-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c94b6-176">versão</span><span class="sxs-lookup"><span data-stu-id="c94b6-176">version</span></span>|<span data-ttu-id="c94b6-177">Int32</span><span class="sxs-lookup"><span data-stu-id="c94b6-177">Int32</span></span>|<span data-ttu-id="c94b6-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c94b6-178">Version of the device configuration.</span></span> <span data-ttu-id="c94b6-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c94b6-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c94b6-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="c94b6-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="c94b6-181">Int32</span><span class="sxs-lookup"><span data-stu-id="c94b6-181">Int32</span></span>|<span data-ttu-id="c94b6-182">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="c94b6-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="c94b6-183">Valores válidos de 1 a 99 herdados de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="c94b6-183">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="c94b6-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="c94b6-184">subjectNameFormat</span></span>|[<span data-ttu-id="c94b6-185">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="c94b6-185">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="c94b6-186">Formato do nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="c94b6-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="c94b6-187">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="c94b6-187">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="c94b6-188">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="c94b6-188">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="c94b6-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="c94b6-189">subjectAlternativeNameType</span></span>|[<span data-ttu-id="c94b6-190">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="c94b6-190">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="c94b6-191">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="c94b6-191">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="c94b6-192">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="c94b6-192">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="c94b6-193">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="c94b6-193">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="c94b6-194">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="c94b6-194">certificateValidityPeriodValue</span></span>|<span data-ttu-id="c94b6-195">Int32</span><span class="sxs-lookup"><span data-stu-id="c94b6-195">Int32</span></span>|<span data-ttu-id="c94b6-196">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="c94b6-196">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="c94b6-197">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="c94b6-197">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="c94b6-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="c94b6-198">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="c94b6-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="c94b6-199">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="c94b6-200">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="c94b6-200">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="c94b6-201">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="c94b6-201">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="c94b6-202">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="c94b6-202">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="c94b6-203">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="c94b6-203">extendedKeyUsages</span></span>|<span data-ttu-id="c94b6-204">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="c94b6-204">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="c94b6-205">Configurações de EKU (uso estendido de chave).</span><span class="sxs-lookup"><span data-stu-id="c94b6-205">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="c94b6-206">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="c94b6-206">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="c94b6-207">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="c94b6-207">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="c94b6-208">Da intendedpurpose</span><span class="sxs-lookup"><span data-stu-id="c94b6-208">intendedPurpose</span></span>|[<span data-ttu-id="c94b6-209">Da intendedpurpose</span><span class="sxs-lookup"><span data-stu-id="c94b6-209">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="c94b6-210">Finalidade do perfil do certificado, que pode ser não atribuído, SmimeEncryption, SmimeSigning, etc. Os valores possíveis são: `unassigned` , `smimeEncryption` , `smimeSigning` , `vpn` , `wifi` .</span><span class="sxs-lookup"><span data-stu-id="c94b6-210">Intended Purpose of the Certificate Profile - which could be Unassigned, SmimeEncryption, SmimeSigning etc. Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="c94b6-211">Resposta</span><span class="sxs-lookup"><span data-stu-id="c94b6-211">Response</span></span>
<span data-ttu-id="c94b6-212">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c94b6-212">If successful, this method returns a `201 Created` response code and a [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c94b6-213">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c94b6-213">Example</span></span>

### <a name="request"></a><span data-ttu-id="c94b6-214">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c94b6-214">Request</span></span>
<span data-ttu-id="c94b6-215">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c94b6-215">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1492

{
  "@odata.type": "#microsoft.graph.androidImportedPFXCertificateProfile",
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
  "intendedPurpose": "smimeEncryption"
}
```

### <a name="response"></a><span data-ttu-id="c94b6-216">Resposta</span><span class="sxs-lookup"><span data-stu-id="c94b6-216">Response</span></span>
<span data-ttu-id="c94b6-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c94b6-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1664

{
  "@odata.type": "#microsoft.graph.androidImportedPFXCertificateProfile",
  "id": "1cd3b0a6-b0a6-1cd3-a6b0-d31ca6b0d31c",
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
  "intendedPurpose": "smimeEncryption"
}
```






