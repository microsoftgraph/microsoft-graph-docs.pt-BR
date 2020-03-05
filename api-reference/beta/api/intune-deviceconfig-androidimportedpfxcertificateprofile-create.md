---
title: Criar androidImportedPFXCertificateProfile
description: Criar um novo objeto androidImportedPFXCertificateProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5eb8af17765067feac7302631ec96867233bd31d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42449716"
---
# <a name="create-androidimportedpfxcertificateprofile"></a><span data-ttu-id="fabcd-103">Criar androidImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="fabcd-103">Create androidImportedPFXCertificateProfile</span></span>

<span data-ttu-id="fabcd-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="fabcd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fabcd-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fabcd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fabcd-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fabcd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fabcd-107">Criar um novo objeto [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="fabcd-107">Create a new [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fabcd-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fabcd-108">Prerequisites</span></span>
<span data-ttu-id="fabcd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fabcd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fabcd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fabcd-111">Permission type</span></span>|<span data-ttu-id="fabcd-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fabcd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fabcd-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fabcd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fabcd-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fabcd-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fabcd-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fabcd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fabcd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fabcd-116">Not supported.</span></span>|
|<span data-ttu-id="fabcd-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fabcd-117">Application</span></span>|<span data-ttu-id="fabcd-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fabcd-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fabcd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fabcd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="fabcd-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fabcd-120">Request headers</span></span>
|<span data-ttu-id="fabcd-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fabcd-121">Header</span></span>|<span data-ttu-id="fabcd-122">Valor</span><span class="sxs-lookup"><span data-stu-id="fabcd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fabcd-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fabcd-123">Authorization</span></span>|<span data-ttu-id="fabcd-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fabcd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fabcd-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fabcd-125">Accept</span></span>|<span data-ttu-id="fabcd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fabcd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fabcd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fabcd-127">Request body</span></span>
<span data-ttu-id="fabcd-128">No corpo da solicitação, forneça uma representação JSON do objeto androidImportedPFXCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="fabcd-128">In the request body, supply a JSON representation for the androidImportedPFXCertificateProfile object.</span></span>

<span data-ttu-id="fabcd-129">A tabela a seguir mostra as propriedades que são necessárias ao criar androidImportedPFXCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="fabcd-129">The following table shows the properties that are required when you create the androidImportedPFXCertificateProfile.</span></span>

|<span data-ttu-id="fabcd-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fabcd-130">Property</span></span>|<span data-ttu-id="fabcd-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="fabcd-131">Type</span></span>|<span data-ttu-id="fabcd-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="fabcd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fabcd-133">id</span><span class="sxs-lookup"><span data-stu-id="fabcd-133">id</span></span>|<span data-ttu-id="fabcd-134">String</span><span class="sxs-lookup"><span data-stu-id="fabcd-134">String</span></span>|<span data-ttu-id="fabcd-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="fabcd-135">Key of the entity.</span></span> <span data-ttu-id="fabcd-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fabcd-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fabcd-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fabcd-137">lastModifiedDateTime</span></span>|<span data-ttu-id="fabcd-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fabcd-138">DateTimeOffset</span></span>|<span data-ttu-id="fabcd-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="fabcd-139">DateTime the object was last modified.</span></span> <span data-ttu-id="fabcd-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fabcd-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fabcd-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="fabcd-141">roleScopeTagIds</span></span>|<span data-ttu-id="fabcd-142">String collection</span><span class="sxs-lookup"><span data-stu-id="fabcd-142">String collection</span></span>|<span data-ttu-id="fabcd-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="fabcd-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="fabcd-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fabcd-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fabcd-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="fabcd-145">supportsScopeTags</span></span>|<span data-ttu-id="fabcd-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="fabcd-146">Boolean</span></span>|<span data-ttu-id="fabcd-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="fabcd-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="fabcd-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="fabcd-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="fabcd-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="fabcd-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="fabcd-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fabcd-150">This property is read-only.</span></span> <span data-ttu-id="fabcd-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fabcd-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fabcd-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="fabcd-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="fabcd-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="fabcd-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="fabcd-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="fabcd-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="fabcd-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fabcd-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fabcd-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="fabcd-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="fabcd-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="fabcd-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="fabcd-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="fabcd-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="fabcd-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fabcd-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fabcd-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="fabcd-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="fabcd-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="fabcd-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="fabcd-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="fabcd-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="fabcd-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fabcd-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fabcd-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fabcd-164">createdDateTime</span></span>|<span data-ttu-id="fabcd-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fabcd-165">DateTimeOffset</span></span>|<span data-ttu-id="fabcd-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="fabcd-166">DateTime the object was created.</span></span> <span data-ttu-id="fabcd-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fabcd-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fabcd-168">description</span><span class="sxs-lookup"><span data-stu-id="fabcd-168">description</span></span>|<span data-ttu-id="fabcd-169">String</span><span class="sxs-lookup"><span data-stu-id="fabcd-169">String</span></span>|<span data-ttu-id="fabcd-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fabcd-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="fabcd-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fabcd-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fabcd-172">displayName</span><span class="sxs-lookup"><span data-stu-id="fabcd-172">displayName</span></span>|<span data-ttu-id="fabcd-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fabcd-173">String</span></span>|<span data-ttu-id="fabcd-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fabcd-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="fabcd-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fabcd-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fabcd-176">versão</span><span class="sxs-lookup"><span data-stu-id="fabcd-176">version</span></span>|<span data-ttu-id="fabcd-177">Int32</span><span class="sxs-lookup"><span data-stu-id="fabcd-177">Int32</span></span>|<span data-ttu-id="fabcd-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fabcd-178">Version of the device configuration.</span></span> <span data-ttu-id="fabcd-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fabcd-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fabcd-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="fabcd-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="fabcd-181">Int32</span><span class="sxs-lookup"><span data-stu-id="fabcd-181">Int32</span></span>|<span data-ttu-id="fabcd-182">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="fabcd-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="fabcd-183">Valores válidos de 1 a 99 herdados de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="fabcd-183">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="fabcd-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="fabcd-184">subjectNameFormat</span></span>|[<span data-ttu-id="fabcd-185">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="fabcd-185">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="fabcd-186">Formato do nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="fabcd-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="fabcd-187">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="fabcd-187">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="fabcd-188">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="fabcd-188">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="fabcd-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="fabcd-189">subjectAlternativeNameType</span></span>|[<span data-ttu-id="fabcd-190">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="fabcd-190">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="fabcd-191">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="fabcd-191">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="fabcd-192">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="fabcd-192">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="fabcd-193">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="fabcd-193">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="fabcd-194">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="fabcd-194">certificateValidityPeriodValue</span></span>|<span data-ttu-id="fabcd-195">Int32</span><span class="sxs-lookup"><span data-stu-id="fabcd-195">Int32</span></span>|<span data-ttu-id="fabcd-196">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="fabcd-196">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="fabcd-197">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="fabcd-197">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="fabcd-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="fabcd-198">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="fabcd-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="fabcd-199">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="fabcd-200">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="fabcd-200">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="fabcd-201">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="fabcd-201">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="fabcd-202">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="fabcd-202">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="fabcd-203">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="fabcd-203">extendedKeyUsages</span></span>|<span data-ttu-id="fabcd-204">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="fabcd-204">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="fabcd-205">Configurações de EKU (uso estendido de chave).</span><span class="sxs-lookup"><span data-stu-id="fabcd-205">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="fabcd-206">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="fabcd-206">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="fabcd-207">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="fabcd-207">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="fabcd-208">Da intendedpurpose</span><span class="sxs-lookup"><span data-stu-id="fabcd-208">intendedPurpose</span></span>|[<span data-ttu-id="fabcd-209">Da intendedpurpose</span><span class="sxs-lookup"><span data-stu-id="fabcd-209">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="fabcd-210">Finalidade do perfil do certificado, que pode ser não atribuído, SmimeEncryption, SmimeSigning, etc. Os valores possíveis são `unassigned`: `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`,.</span><span class="sxs-lookup"><span data-stu-id="fabcd-210">Intended Purpose of the Certificate Profile - which could be Unassigned, SmimeEncryption, SmimeSigning etc. Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="fabcd-211">Resposta</span><span class="sxs-lookup"><span data-stu-id="fabcd-211">Response</span></span>
<span data-ttu-id="fabcd-212">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fabcd-212">If successful, this method returns a `201 Created` response code and a [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fabcd-213">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fabcd-213">Example</span></span>

### <a name="request"></a><span data-ttu-id="fabcd-214">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fabcd-214">Request</span></span>
<span data-ttu-id="fabcd-215">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fabcd-215">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fabcd-216">Resposta</span><span class="sxs-lookup"><span data-stu-id="fabcd-216">Response</span></span>
<span data-ttu-id="fabcd-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fabcd-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





