---
title: Atualizar macOSImportedPFXCertificateProfile
description: Atualiza as propriedades de um objeto macOSImportedPFXCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9e673ade636b50476fdfc6c0da3a97795dfccc75
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47974608"
---
# <a name="update-macosimportedpfxcertificateprofile"></a><span data-ttu-id="76666-103">Atualizar macOSImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="76666-103">Update macOSImportedPFXCertificateProfile</span></span>

<span data-ttu-id="76666-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76666-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="76666-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="76666-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="76666-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="76666-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76666-107">Atualiza as propriedades de um objeto [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="76666-107">Update the properties of a [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="76666-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="76666-108">Prerequisites</span></span>
<span data-ttu-id="76666-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76666-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76666-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="76666-111">Permission type</span></span>|<span data-ttu-id="76666-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="76666-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="76666-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="76666-113">Delegated (work or school account)</span></span>|<span data-ttu-id="76666-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76666-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="76666-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="76666-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="76666-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="76666-116">Not supported.</span></span>|
|<span data-ttu-id="76666-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="76666-117">Application</span></span>|<span data-ttu-id="76666-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76666-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="76666-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="76666-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="76666-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="76666-120">Request headers</span></span>
|<span data-ttu-id="76666-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="76666-121">Header</span></span>|<span data-ttu-id="76666-122">Valor</span><span class="sxs-lookup"><span data-stu-id="76666-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="76666-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="76666-123">Authorization</span></span>|<span data-ttu-id="76666-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="76666-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="76666-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="76666-125">Accept</span></span>|<span data-ttu-id="76666-126">application/json</span><span class="sxs-lookup"><span data-stu-id="76666-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="76666-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="76666-127">Request body</span></span>
<span data-ttu-id="76666-128">No corpo da solicitação, forneça uma representação JSON do objeto [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="76666-128">In the request body, supply a JSON representation for the [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) object.</span></span>

<span data-ttu-id="76666-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="76666-129">The following table shows the properties that are required when you create the [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md).</span></span>

|<span data-ttu-id="76666-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="76666-130">Property</span></span>|<span data-ttu-id="76666-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="76666-131">Type</span></span>|<span data-ttu-id="76666-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="76666-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76666-133">id</span><span class="sxs-lookup"><span data-stu-id="76666-133">id</span></span>|<span data-ttu-id="76666-134">String</span><span class="sxs-lookup"><span data-stu-id="76666-134">String</span></span>|<span data-ttu-id="76666-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="76666-135">Key of the entity.</span></span> <span data-ttu-id="76666-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76666-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76666-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="76666-137">lastModifiedDateTime</span></span>|<span data-ttu-id="76666-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76666-138">DateTimeOffset</span></span>|<span data-ttu-id="76666-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="76666-139">DateTime the object was last modified.</span></span> <span data-ttu-id="76666-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76666-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76666-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="76666-141">roleScopeTagIds</span></span>|<span data-ttu-id="76666-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="76666-142">String collection</span></span>|<span data-ttu-id="76666-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="76666-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="76666-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76666-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76666-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="76666-145">supportsScopeTags</span></span>|<span data-ttu-id="76666-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="76666-146">Boolean</span></span>|<span data-ttu-id="76666-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="76666-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="76666-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="76666-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="76666-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="76666-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="76666-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="76666-150">This property is read-only.</span></span> <span data-ttu-id="76666-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76666-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76666-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="76666-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="76666-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="76666-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="76666-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="76666-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="76666-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76666-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76666-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="76666-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="76666-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="76666-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="76666-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="76666-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="76666-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76666-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76666-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="76666-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="76666-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="76666-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="76666-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="76666-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="76666-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76666-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76666-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="76666-164">createdDateTime</span></span>|<span data-ttu-id="76666-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76666-165">DateTimeOffset</span></span>|<span data-ttu-id="76666-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="76666-166">DateTime the object was created.</span></span> <span data-ttu-id="76666-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76666-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76666-168">description</span><span class="sxs-lookup"><span data-stu-id="76666-168">description</span></span>|<span data-ttu-id="76666-169">String</span><span class="sxs-lookup"><span data-stu-id="76666-169">String</span></span>|<span data-ttu-id="76666-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="76666-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="76666-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76666-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76666-172">displayName</span><span class="sxs-lookup"><span data-stu-id="76666-172">displayName</span></span>|<span data-ttu-id="76666-173">String</span><span class="sxs-lookup"><span data-stu-id="76666-173">String</span></span>|<span data-ttu-id="76666-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="76666-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="76666-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76666-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76666-176">versão</span><span class="sxs-lookup"><span data-stu-id="76666-176">version</span></span>|<span data-ttu-id="76666-177">Int32</span><span class="sxs-lookup"><span data-stu-id="76666-177">Int32</span></span>|<span data-ttu-id="76666-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="76666-178">Version of the device configuration.</span></span> <span data-ttu-id="76666-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76666-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76666-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="76666-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="76666-181">Int32</span><span class="sxs-lookup"><span data-stu-id="76666-181">Int32</span></span>|<span data-ttu-id="76666-182">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="76666-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="76666-183">Herdado de [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="76666-183">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="76666-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="76666-184">subjectNameFormat</span></span>|[<span data-ttu-id="76666-185">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="76666-185">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="76666-186">Formato do nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="76666-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="76666-187">Herdado de [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="76666-187">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="76666-188">Os possíveis valores são: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="76666-188">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="76666-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="76666-189">subjectAlternativeNameType</span></span>|[<span data-ttu-id="76666-190">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="76666-190">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="76666-191">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="76666-191">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="76666-192">Herdado de [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="76666-192">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="76666-193">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="76666-193">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="76666-194">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="76666-194">certificateValidityPeriodValue</span></span>|<span data-ttu-id="76666-195">Int32</span><span class="sxs-lookup"><span data-stu-id="76666-195">Int32</span></span>|<span data-ttu-id="76666-196">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="76666-196">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="76666-197">Herdado de [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="76666-197">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="76666-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="76666-198">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="76666-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="76666-199">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="76666-200">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="76666-200">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="76666-201">Herdado de [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="76666-201">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="76666-202">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="76666-202">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="76666-203">Da intendedpurpose</span><span class="sxs-lookup"><span data-stu-id="76666-203">intendedPurpose</span></span>|[<span data-ttu-id="76666-204">Da intendedpurpose</span><span class="sxs-lookup"><span data-stu-id="76666-204">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="76666-205">Finalidade do perfil do certificado, que pode ser não atribuído, SmimeEncryption, SmimeSigning, etc. Os valores possíveis são: `unassigned` , `smimeEncryption` , `smimeSigning` , `vpn` , `wifi` .</span><span class="sxs-lookup"><span data-stu-id="76666-205">Intended Purpose of the Certificate Profile - which could be Unassigned, SmimeEncryption, SmimeSigning etc. Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="76666-206">Resposta</span><span class="sxs-lookup"><span data-stu-id="76666-206">Response</span></span>
<span data-ttu-id="76666-207">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="76666-207">If successful, this method returns a `200 OK` response code and an updated [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76666-208">Exemplo</span><span class="sxs-lookup"><span data-stu-id="76666-208">Example</span></span>

### <a name="request"></a><span data-ttu-id="76666-209">Solicitação</span><span class="sxs-lookup"><span data-stu-id="76666-209">Request</span></span>
<span data-ttu-id="76666-210">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="76666-210">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1297

{
  "@odata.type": "#microsoft.graph.macOSImportedPFXCertificateProfile",
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
  "intendedPurpose": "smimeEncryption"
}
```

### <a name="response"></a><span data-ttu-id="76666-211">Resposta</span><span class="sxs-lookup"><span data-stu-id="76666-211">Response</span></span>
<span data-ttu-id="76666-p118">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="76666-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1469

{
  "@odata.type": "#microsoft.graph.macOSImportedPFXCertificateProfile",
  "id": "4175bd8c-bd8c-4175-8cbd-75418cbd7541",
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
  "intendedPurpose": "smimeEncryption"
}
```






