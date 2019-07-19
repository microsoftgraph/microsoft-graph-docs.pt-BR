---
title: Atualizar androidScepCertificateProfile
description: Atualiza as propriedades de um objeto androidScepCertificateProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d8a1b323b7ad0fbb9dca19313e410ff2f61a62aa
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34969901"
---
# <a name="update-androidscepcertificateprofile"></a><span data-ttu-id="c8627-103">Atualizar androidScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="c8627-103">Update androidScepCertificateProfile</span></span>

> <span data-ttu-id="c8627-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c8627-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c8627-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c8627-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8627-106">Atualiza as propriedades de um objeto [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="c8627-106">Update the properties of a [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c8627-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c8627-107">Prerequisites</span></span>
<span data-ttu-id="c8627-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8627-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8627-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c8627-110">Permission type</span></span>|<span data-ttu-id="c8627-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c8627-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c8627-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c8627-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c8627-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8627-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c8627-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c8627-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8627-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c8627-115">Not supported.</span></span>|
|<span data-ttu-id="c8627-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c8627-116">Application</span></span>|<span data-ttu-id="c8627-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c8627-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c8627-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c8627-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="c8627-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c8627-119">Request headers</span></span>
|<span data-ttu-id="c8627-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c8627-120">Header</span></span>|<span data-ttu-id="c8627-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c8627-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c8627-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c8627-122">Authorization</span></span>|<span data-ttu-id="c8627-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c8627-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c8627-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c8627-124">Accept</span></span>|<span data-ttu-id="c8627-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c8627-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8627-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c8627-126">Request body</span></span>
<span data-ttu-id="c8627-127">No corpo da solicitação, forneça uma representação JSON do objeto [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="c8627-127">In the request body, supply a JSON representation for the [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) object.</span></span>

<span data-ttu-id="c8627-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="c8627-128">The following table shows the properties that are required when you create the [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md).</span></span>

|<span data-ttu-id="c8627-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c8627-129">Property</span></span>|<span data-ttu-id="c8627-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="c8627-130">Type</span></span>|<span data-ttu-id="c8627-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="c8627-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8627-132">id</span><span class="sxs-lookup"><span data-stu-id="c8627-132">id</span></span>|<span data-ttu-id="c8627-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c8627-133">String</span></span>|<span data-ttu-id="c8627-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c8627-134">Key of the entity.</span></span> <span data-ttu-id="c8627-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c8627-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c8627-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c8627-136">lastModifiedDateTime</span></span>|<span data-ttu-id="c8627-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8627-137">DateTimeOffset</span></span>|<span data-ttu-id="c8627-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="c8627-138">DateTime the object was last modified.</span></span> <span data-ttu-id="c8627-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c8627-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c8627-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c8627-140">roleScopeTagIds</span></span>|<span data-ttu-id="c8627-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c8627-141">String collection</span></span>|<span data-ttu-id="c8627-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="c8627-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c8627-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c8627-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c8627-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c8627-144">supportsScopeTags</span></span>|<span data-ttu-id="c8627-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="c8627-145">Boolean</span></span>|<span data-ttu-id="c8627-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="c8627-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c8627-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="c8627-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c8627-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="c8627-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c8627-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c8627-149">This property is read-only.</span></span> <span data-ttu-id="c8627-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c8627-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c8627-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c8627-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="c8627-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c8627-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="c8627-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="c8627-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="c8627-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c8627-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c8627-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c8627-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="c8627-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c8627-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="c8627-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="c8627-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="c8627-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c8627-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c8627-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c8627-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="c8627-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c8627-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="c8627-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="c8627-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="c8627-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c8627-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c8627-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c8627-163">createdDateTime</span></span>|<span data-ttu-id="c8627-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8627-164">DateTimeOffset</span></span>|<span data-ttu-id="c8627-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="c8627-165">DateTime the object was created.</span></span> <span data-ttu-id="c8627-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c8627-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c8627-167">descrição</span><span class="sxs-lookup"><span data-stu-id="c8627-167">description</span></span>|<span data-ttu-id="c8627-168">String</span><span class="sxs-lookup"><span data-stu-id="c8627-168">String</span></span>|<span data-ttu-id="c8627-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c8627-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c8627-170">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c8627-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c8627-171">displayName</span><span class="sxs-lookup"><span data-stu-id="c8627-171">displayName</span></span>|<span data-ttu-id="c8627-172">String</span><span class="sxs-lookup"><span data-stu-id="c8627-172">String</span></span>|<span data-ttu-id="c8627-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c8627-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c8627-174">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c8627-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c8627-175">versão</span><span class="sxs-lookup"><span data-stu-id="c8627-175">version</span></span>|<span data-ttu-id="c8627-176">Int32</span><span class="sxs-lookup"><span data-stu-id="c8627-176">Int32</span></span>|<span data-ttu-id="c8627-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c8627-177">Version of the device configuration.</span></span> <span data-ttu-id="c8627-178">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c8627-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c8627-179">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="c8627-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="c8627-180">Int32</span><span class="sxs-lookup"><span data-stu-id="c8627-180">Int32</span></span>|<span data-ttu-id="c8627-181">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="c8627-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="c8627-182">Valores válidos de 1 a 99 herdados de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="c8627-182">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="c8627-183">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="c8627-183">subjectNameFormat</span></span>|[<span data-ttu-id="c8627-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="c8627-184">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="c8627-185">Formato do nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="c8627-185">Certificate Subject Name Format.</span></span> <span data-ttu-id="c8627-186">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="c8627-186">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="c8627-187">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="c8627-187">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="c8627-188">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="c8627-188">subjectAlternativeNameType</span></span>|[<span data-ttu-id="c8627-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="c8627-189">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="c8627-190">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="c8627-190">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="c8627-191">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="c8627-191">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="c8627-192">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="c8627-192">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="c8627-193">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="c8627-193">certificateValidityPeriodValue</span></span>|<span data-ttu-id="c8627-194">Int32</span><span class="sxs-lookup"><span data-stu-id="c8627-194">Int32</span></span>|<span data-ttu-id="c8627-195">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="c8627-195">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="c8627-196">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="c8627-196">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="c8627-197">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="c8627-197">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="c8627-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="c8627-198">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="c8627-199">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="c8627-199">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="c8627-200">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="c8627-200">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="c8627-201">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="c8627-201">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="c8627-202">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="c8627-202">extendedKeyUsages</span></span>|<span data-ttu-id="c8627-203">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="c8627-203">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="c8627-204">Configurações de EKU (uso estendido de chave).</span><span class="sxs-lookup"><span data-stu-id="c8627-204">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="c8627-205">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="c8627-205">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="c8627-206">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="c8627-206">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="c8627-207">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="c8627-207">scepServerUrls</span></span>|<span data-ttu-id="c8627-208">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c8627-208">String collection</span></span>|<span data-ttu-id="c8627-209">URL (s) do servidor de SCEP</span><span class="sxs-lookup"><span data-stu-id="c8627-209">SCEP Server Url(s)</span></span>|
|<span data-ttu-id="c8627-210">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="c8627-210">subjectNameFormatString</span></span>|<span data-ttu-id="c8627-211">String</span><span class="sxs-lookup"><span data-stu-id="c8627-211">String</span></span>|<span data-ttu-id="c8627-212">Formato personalizado a ser usado com SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="c8627-212">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="c8627-213">Exemplo: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = usuários corporativos, O = Contoso Corporation, L = Redmond, ST = WA, C = br</span><span class="sxs-lookup"><span data-stu-id="c8627-213">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="c8627-214">uso de</span><span class="sxs-lookup"><span data-stu-id="c8627-214">keyUsage</span></span>|[<span data-ttu-id="c8627-215">usos de</span><span class="sxs-lookup"><span data-stu-id="c8627-215">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="c8627-216">Uso da chave do SCEP.</span><span class="sxs-lookup"><span data-stu-id="c8627-216">SCEP Key Usage.</span></span> <span data-ttu-id="c8627-217">Os valores possíveis são: `keyEncipherment` e `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="c8627-217">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="c8627-218">keySize</span><span class="sxs-lookup"><span data-stu-id="c8627-218">keySize</span></span>|[<span data-ttu-id="c8627-219">keySize</span><span class="sxs-lookup"><span data-stu-id="c8627-219">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="c8627-220">Tamanho da chave SCEP.</span><span class="sxs-lookup"><span data-stu-id="c8627-220">SCEP Key Size.</span></span> <span data-ttu-id="c8627-221">Os valores possíveis são: `size1024` e `size2048`.</span><span class="sxs-lookup"><span data-stu-id="c8627-221">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="c8627-222">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="c8627-222">hashAlgorithm</span></span>|[<span data-ttu-id="c8627-223">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="c8627-223">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="c8627-224">Algoritmo de hash do SCEP.</span><span class="sxs-lookup"><span data-stu-id="c8627-224">SCEP Hash Algorithm.</span></span> <span data-ttu-id="c8627-225">Os valores possíveis são: `sha1` e `sha2`.</span><span class="sxs-lookup"><span data-stu-id="c8627-225">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="c8627-226">Subjectalternativenameformatstring foi</span><span class="sxs-lookup"><span data-stu-id="c8627-226">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="c8627-227">String</span><span class="sxs-lookup"><span data-stu-id="c8627-227">String</span></span>|<span data-ttu-id="c8627-228">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="c8627-228">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="c8627-229">Resposta</span><span class="sxs-lookup"><span data-stu-id="c8627-229">Response</span></span>
<span data-ttu-id="c8627-230">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c8627-230">If successful, this method returns a `200 OK` response code and an updated [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8627-231">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c8627-231">Example</span></span>

### <a name="request"></a><span data-ttu-id="c8627-232">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c8627-232">Request</span></span>
<span data-ttu-id="c8627-233">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c8627-233">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1747

{
  "@odata.type": "#microsoft.graph.androidScepCertificateProfile",
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
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```

### <a name="response"></a><span data-ttu-id="c8627-234">Resposta</span><span class="sxs-lookup"><span data-stu-id="c8627-234">Response</span></span>
<span data-ttu-id="c8627-p123">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c8627-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1919

{
  "@odata.type": "#microsoft.graph.androidScepCertificateProfile",
  "id": "e9a0dbbd-dbbd-e9a0-bddb-a0e9bddba0e9",
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
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```





