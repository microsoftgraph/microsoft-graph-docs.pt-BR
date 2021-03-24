---
title: Criar androidDeviceOwnerImportedPFXCertificateProfile
description: Crie um novo objeto androidDeviceOwnerImportedPFXCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b2db15cadfd07ff03684fca1b63141ede1bb3f71
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51138605"
---
# <a name="create-androiddeviceownerimportedpfxcertificateprofile"></a><span data-ttu-id="d65bd-103">Criar androidDeviceOwnerImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="d65bd-103">Create androidDeviceOwnerImportedPFXCertificateProfile</span></span>

<span data-ttu-id="d65bd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d65bd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d65bd-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d65bd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d65bd-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d65bd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d65bd-107">Crie um novo [objeto androidDeviceOwnerImportedPFXCertificateProfile.](../resources/intune-deviceconfig-androiddeviceownerimportedpfxcertificateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d65bd-107">Create a new [androidDeviceOwnerImportedPFXCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d65bd-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d65bd-108">Prerequisites</span></span>
<span data-ttu-id="d65bd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d65bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d65bd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d65bd-111">Permission type</span></span>|<span data-ttu-id="d65bd-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d65bd-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d65bd-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d65bd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d65bd-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d65bd-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d65bd-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d65bd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d65bd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d65bd-116">Not supported.</span></span>|
|<span data-ttu-id="d65bd-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d65bd-117">Application</span></span>|<span data-ttu-id="d65bd-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d65bd-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d65bd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d65bd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d65bd-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d65bd-120">Request headers</span></span>
|<span data-ttu-id="d65bd-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d65bd-121">Header</span></span>|<span data-ttu-id="d65bd-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d65bd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d65bd-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d65bd-123">Authorization</span></span>|<span data-ttu-id="d65bd-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d65bd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d65bd-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d65bd-125">Accept</span></span>|<span data-ttu-id="d65bd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d65bd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d65bd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d65bd-127">Request body</span></span>
<span data-ttu-id="d65bd-128">No corpo da solicitação, fornece uma representação JSON para o objeto androidDeviceOwnerImportedPFXCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="d65bd-128">In the request body, supply a JSON representation for the androidDeviceOwnerImportedPFXCertificateProfile object.</span></span>

<span data-ttu-id="d65bd-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o androidDeviceOwnerImportedPFXCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="d65bd-129">The following table shows the properties that are required when you create the androidDeviceOwnerImportedPFXCertificateProfile.</span></span>

|<span data-ttu-id="d65bd-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d65bd-130">Property</span></span>|<span data-ttu-id="d65bd-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d65bd-131">Type</span></span>|<span data-ttu-id="d65bd-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d65bd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d65bd-133">id</span><span class="sxs-lookup"><span data-stu-id="d65bd-133">id</span></span>|<span data-ttu-id="d65bd-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d65bd-134">String</span></span>|<span data-ttu-id="d65bd-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d65bd-135">Key of the entity.</span></span> <span data-ttu-id="d65bd-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d65bd-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d65bd-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d65bd-137">lastModifiedDateTime</span></span>|<span data-ttu-id="d65bd-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d65bd-138">DateTimeOffset</span></span>|<span data-ttu-id="d65bd-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="d65bd-139">DateTime the object was last modified.</span></span> <span data-ttu-id="d65bd-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d65bd-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d65bd-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d65bd-141">roleScopeTagIds</span></span>|<span data-ttu-id="d65bd-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d65bd-142">String collection</span></span>|<span data-ttu-id="d65bd-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="d65bd-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d65bd-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d65bd-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d65bd-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d65bd-145">supportsScopeTags</span></span>|<span data-ttu-id="d65bd-146">Booleano</span><span class="sxs-lookup"><span data-stu-id="d65bd-146">Boolean</span></span>|<span data-ttu-id="d65bd-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="d65bd-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d65bd-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="d65bd-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d65bd-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="d65bd-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d65bd-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d65bd-150">This property is read-only.</span></span> <span data-ttu-id="d65bd-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d65bd-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d65bd-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d65bd-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="d65bd-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d65bd-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="d65bd-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="d65bd-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="d65bd-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d65bd-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d65bd-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d65bd-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="d65bd-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d65bd-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="d65bd-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="d65bd-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="d65bd-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d65bd-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d65bd-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d65bd-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="d65bd-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d65bd-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="d65bd-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="d65bd-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="d65bd-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d65bd-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d65bd-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d65bd-164">createdDateTime</span></span>|<span data-ttu-id="d65bd-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d65bd-165">DateTimeOffset</span></span>|<span data-ttu-id="d65bd-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="d65bd-166">DateTime the object was created.</span></span> <span data-ttu-id="d65bd-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d65bd-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d65bd-168">descrição</span><span class="sxs-lookup"><span data-stu-id="d65bd-168">description</span></span>|<span data-ttu-id="d65bd-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d65bd-169">String</span></span>|<span data-ttu-id="d65bd-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d65bd-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d65bd-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d65bd-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d65bd-172">displayName</span><span class="sxs-lookup"><span data-stu-id="d65bd-172">displayName</span></span>|<span data-ttu-id="d65bd-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d65bd-173">String</span></span>|<span data-ttu-id="d65bd-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d65bd-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d65bd-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d65bd-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d65bd-176">versão</span><span class="sxs-lookup"><span data-stu-id="d65bd-176">version</span></span>|<span data-ttu-id="d65bd-177">Int32</span><span class="sxs-lookup"><span data-stu-id="d65bd-177">Int32</span></span>|<span data-ttu-id="d65bd-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d65bd-178">Version of the device configuration.</span></span> <span data-ttu-id="d65bd-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d65bd-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d65bd-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="d65bd-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="d65bd-181">Int32</span><span class="sxs-lookup"><span data-stu-id="d65bd-181">Int32</span></span>|<span data-ttu-id="d65bd-182">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="d65bd-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="d65bd-183">Valores válidos de 1 a 99 Herdados [de androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="d65bd-183">Valid values 1 to 99 Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span></span>|
|<span data-ttu-id="d65bd-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="d65bd-184">subjectNameFormat</span></span>|[<span data-ttu-id="d65bd-185">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="d65bd-185">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="d65bd-186">Formato de Nome do Assunto do Certificado.</span><span class="sxs-lookup"><span data-stu-id="d65bd-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="d65bd-187">Herdado [de androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="d65bd-187">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span></span> <span data-ttu-id="d65bd-188">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="d65bd-188">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="d65bd-189">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="d65bd-189">certificateValidityPeriodValue</span></span>|<span data-ttu-id="d65bd-190">Int32</span><span class="sxs-lookup"><span data-stu-id="d65bd-190">Int32</span></span>|<span data-ttu-id="d65bd-191">Valor do Período de Validade do Certificado.</span><span class="sxs-lookup"><span data-stu-id="d65bd-191">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="d65bd-192">Herdado [de androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="d65bd-192">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span></span>|
|<span data-ttu-id="d65bd-193">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="d65bd-193">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="d65bd-194">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="d65bd-194">certificateValidityPeriodScale</span></span>](../resources/intune-shared-certificatevalidityperiodscale.md)|<span data-ttu-id="d65bd-195">Dimensione para o Período de Validade do Certificado.</span><span class="sxs-lookup"><span data-stu-id="d65bd-195">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="d65bd-196">Herdado [de androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="d65bd-196">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span></span> <span data-ttu-id="d65bd-197">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="d65bd-197">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="d65bd-198">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="d65bd-198">extendedKeyUsages</span></span>|<span data-ttu-id="d65bd-199">[Coleção extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="d65bd-199">[extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="d65bd-200">Configurações de Uso de Chave Estendida (EKU).</span><span class="sxs-lookup"><span data-stu-id="d65bd-200">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="d65bd-201">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="d65bd-201">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="d65bd-202">Herdado [de androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="d65bd-202">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span></span>|
|<span data-ttu-id="d65bd-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="d65bd-203">subjectAlternativeNameType</span></span>|[<span data-ttu-id="d65bd-204">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="d65bd-204">subjectAlternativeNameType</span></span>](../resources/intune-shared-subjectalternativenametype.md)|<span data-ttu-id="d65bd-205">Tipo de nome alternativo do assunto do certificado.</span><span class="sxs-lookup"><span data-stu-id="d65bd-205">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="d65bd-206">Herdado [de androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="d65bd-206">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span></span> <span data-ttu-id="d65bd-207">Os possíveis valores são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span><span class="sxs-lookup"><span data-stu-id="d65bd-207">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span></span>|
|<span data-ttu-id="d65bd-208">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="d65bd-208">intendedPurpose</span></span>|[<span data-ttu-id="d65bd-209">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="d65bd-209">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="d65bd-210">Finalidade pretendido do Perfil de Certificado - que pode ser Unassigned, SmimeEncryption, SmimeSigning etc. Os valores possíveis são: `unassigned` , , , , `smimeEncryption` `smimeSigning` `vpn` `wifi` .</span><span class="sxs-lookup"><span data-stu-id="d65bd-210">Intended Purpose of the Certificate Profile - which could be Unassigned, SmimeEncryption, SmimeSigning etc. Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="d65bd-211">Resposta</span><span class="sxs-lookup"><span data-stu-id="d65bd-211">Response</span></span>
<span data-ttu-id="d65bd-212">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto androidDeviceOwnerImportedPFXCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerimportedpfxcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d65bd-212">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerImportedPFXCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d65bd-213">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d65bd-213">Example</span></span>

### <a name="request"></a><span data-ttu-id="d65bd-214">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d65bd-214">Request</span></span>
<span data-ttu-id="d65bd-215">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d65bd-215">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1503

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerImportedPFXCertificateProfile",
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
  "intendedPurpose": "smimeEncryption"
}
```

### <a name="response"></a><span data-ttu-id="d65bd-216">Resposta</span><span class="sxs-lookup"><span data-stu-id="d65bd-216">Response</span></span>
<span data-ttu-id="d65bd-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d65bd-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1675

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerImportedPFXCertificateProfile",
  "id": "8d46d3c7-d3c7-8d46-c7d3-468dc7d3468d",
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
  "intendedPurpose": "smimeEncryption"
}
```




