---
title: Criar androidScepCertificateProfile
description: Criar um novo objeto androidScepCertificateProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 726299480430704fd7706bdc38b6912199090785
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37176132"
---
# <a name="create-androidscepcertificateprofile"></a><span data-ttu-id="c0472-103">Criar androidScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="c0472-103">Create androidScepCertificateProfile</span></span>

> <span data-ttu-id="c0472-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c0472-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c0472-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c0472-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0472-106">Criar um novo objeto [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="c0472-106">Create a new [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c0472-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c0472-107">Prerequisites</span></span>
<span data-ttu-id="c0472-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0472-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0472-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c0472-110">Permission type</span></span>|<span data-ttu-id="c0472-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c0472-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0472-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c0472-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c0472-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0472-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c0472-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c0472-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0472-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0472-115">Not supported.</span></span>|
|<span data-ttu-id="c0472-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c0472-116">Application</span></span>|<span data-ttu-id="c0472-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0472-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0472-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c0472-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c0472-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c0472-119">Request headers</span></span>
|<span data-ttu-id="c0472-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c0472-120">Header</span></span>|<span data-ttu-id="c0472-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c0472-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c0472-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c0472-122">Authorization</span></span>|<span data-ttu-id="c0472-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c0472-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c0472-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c0472-124">Accept</span></span>|<span data-ttu-id="c0472-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c0472-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0472-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c0472-126">Request body</span></span>
<span data-ttu-id="c0472-127">No corpo da solicitação, forneça uma representação JSON do objeto androidScepCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="c0472-127">In the request body, supply a JSON representation for the androidScepCertificateProfile object.</span></span>

<span data-ttu-id="c0472-128">A tabela a seguir mostra as propriedades que são necessárias ao criar androidScepCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="c0472-128">The following table shows the properties that are required when you create the androidScepCertificateProfile.</span></span>

|<span data-ttu-id="c0472-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c0472-129">Property</span></span>|<span data-ttu-id="c0472-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="c0472-130">Type</span></span>|<span data-ttu-id="c0472-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0472-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0472-132">id</span><span class="sxs-lookup"><span data-stu-id="c0472-132">id</span></span>|<span data-ttu-id="c0472-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c0472-133">String</span></span>|<span data-ttu-id="c0472-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c0472-134">Key of the entity.</span></span> <span data-ttu-id="c0472-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c0472-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c0472-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c0472-136">lastModifiedDateTime</span></span>|<span data-ttu-id="c0472-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c0472-137">DateTimeOffset</span></span>|<span data-ttu-id="c0472-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="c0472-138">DateTime the object was last modified.</span></span> <span data-ttu-id="c0472-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c0472-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c0472-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c0472-140">roleScopeTagIds</span></span>|<span data-ttu-id="c0472-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c0472-141">String collection</span></span>|<span data-ttu-id="c0472-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="c0472-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c0472-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c0472-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c0472-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c0472-144">supportsScopeTags</span></span>|<span data-ttu-id="c0472-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="c0472-145">Boolean</span></span>|<span data-ttu-id="c0472-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="c0472-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c0472-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="c0472-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c0472-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="c0472-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c0472-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c0472-149">This property is read-only.</span></span> <span data-ttu-id="c0472-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c0472-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c0472-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c0472-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="c0472-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c0472-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="c0472-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="c0472-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="c0472-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c0472-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c0472-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c0472-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="c0472-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c0472-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="c0472-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="c0472-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="c0472-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c0472-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c0472-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c0472-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="c0472-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c0472-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="c0472-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="c0472-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="c0472-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c0472-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c0472-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c0472-163">createdDateTime</span></span>|<span data-ttu-id="c0472-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c0472-164">DateTimeOffset</span></span>|<span data-ttu-id="c0472-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="c0472-165">DateTime the object was created.</span></span> <span data-ttu-id="c0472-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c0472-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c0472-167">descrição</span><span class="sxs-lookup"><span data-stu-id="c0472-167">description</span></span>|<span data-ttu-id="c0472-168">String</span><span class="sxs-lookup"><span data-stu-id="c0472-168">String</span></span>|<span data-ttu-id="c0472-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c0472-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c0472-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c0472-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c0472-171">displayName</span><span class="sxs-lookup"><span data-stu-id="c0472-171">displayName</span></span>|<span data-ttu-id="c0472-172">String</span><span class="sxs-lookup"><span data-stu-id="c0472-172">String</span></span>|<span data-ttu-id="c0472-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c0472-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c0472-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c0472-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c0472-175">versão</span><span class="sxs-lookup"><span data-stu-id="c0472-175">version</span></span>|<span data-ttu-id="c0472-176">Int32</span><span class="sxs-lookup"><span data-stu-id="c0472-176">Int32</span></span>|<span data-ttu-id="c0472-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c0472-177">Version of the device configuration.</span></span> <span data-ttu-id="c0472-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c0472-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c0472-179">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="c0472-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="c0472-180">Int32</span><span class="sxs-lookup"><span data-stu-id="c0472-180">Int32</span></span>|<span data-ttu-id="c0472-181">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="c0472-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="c0472-182">Valores válidos de 1 a 99 herdados de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="c0472-182">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="c0472-183">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="c0472-183">subjectNameFormat</span></span>|[<span data-ttu-id="c0472-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="c0472-184">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="c0472-185">Formato do nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="c0472-185">Certificate Subject Name Format.</span></span> <span data-ttu-id="c0472-186">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="c0472-186">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="c0472-187">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="c0472-187">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="c0472-188">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="c0472-188">subjectAlternativeNameType</span></span>|[<span data-ttu-id="c0472-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="c0472-189">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="c0472-190">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="c0472-190">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="c0472-191">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="c0472-191">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="c0472-192">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="c0472-192">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="c0472-193">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="c0472-193">certificateValidityPeriodValue</span></span>|<span data-ttu-id="c0472-194">Int32</span><span class="sxs-lookup"><span data-stu-id="c0472-194">Int32</span></span>|<span data-ttu-id="c0472-195">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="c0472-195">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="c0472-196">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="c0472-196">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="c0472-197">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="c0472-197">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="c0472-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="c0472-198">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="c0472-199">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="c0472-199">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="c0472-200">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="c0472-200">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="c0472-201">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="c0472-201">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="c0472-202">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="c0472-202">extendedKeyUsages</span></span>|<span data-ttu-id="c0472-203">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="c0472-203">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="c0472-204">Configurações de EKU (uso estendido de chave).</span><span class="sxs-lookup"><span data-stu-id="c0472-204">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="c0472-205">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="c0472-205">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="c0472-206">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="c0472-206">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="c0472-207">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="c0472-207">scepServerUrls</span></span>|<span data-ttu-id="c0472-208">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c0472-208">String collection</span></span>|<span data-ttu-id="c0472-209">URL (s) do servidor de SCEP</span><span class="sxs-lookup"><span data-stu-id="c0472-209">SCEP Server Url(s)</span></span>|
|<span data-ttu-id="c0472-210">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="c0472-210">subjectNameFormatString</span></span>|<span data-ttu-id="c0472-211">String</span><span class="sxs-lookup"><span data-stu-id="c0472-211">String</span></span>|<span data-ttu-id="c0472-212">Formato personalizado a ser usado com SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="c0472-212">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="c0472-213">Exemplo: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = usuários corporativos, O = Contoso Corporation, L = Redmond, ST = WA, C = br</span><span class="sxs-lookup"><span data-stu-id="c0472-213">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="c0472-214">uso de</span><span class="sxs-lookup"><span data-stu-id="c0472-214">keyUsage</span></span>|[<span data-ttu-id="c0472-215">usos de</span><span class="sxs-lookup"><span data-stu-id="c0472-215">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="c0472-216">Uso da chave do SCEP.</span><span class="sxs-lookup"><span data-stu-id="c0472-216">SCEP Key Usage.</span></span> <span data-ttu-id="c0472-217">Os valores possíveis são: `keyEncipherment` e `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="c0472-217">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="c0472-218">keySize</span><span class="sxs-lookup"><span data-stu-id="c0472-218">keySize</span></span>|[<span data-ttu-id="c0472-219">keySize</span><span class="sxs-lookup"><span data-stu-id="c0472-219">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="c0472-220">Tamanho da chave SCEP.</span><span class="sxs-lookup"><span data-stu-id="c0472-220">SCEP Key Size.</span></span> <span data-ttu-id="c0472-221">Os valores possíveis são: `size1024` e `size2048`.</span><span class="sxs-lookup"><span data-stu-id="c0472-221">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="c0472-222">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="c0472-222">hashAlgorithm</span></span>|[<span data-ttu-id="c0472-223">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="c0472-223">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="c0472-224">Algoritmo de hash do SCEP.</span><span class="sxs-lookup"><span data-stu-id="c0472-224">SCEP Hash Algorithm.</span></span> <span data-ttu-id="c0472-225">Os valores possíveis são: `sha1` e `sha2`.</span><span class="sxs-lookup"><span data-stu-id="c0472-225">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="c0472-226">Subjectalternativenameformatstring foi</span><span class="sxs-lookup"><span data-stu-id="c0472-226">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="c0472-227">String</span><span class="sxs-lookup"><span data-stu-id="c0472-227">String</span></span>|<span data-ttu-id="c0472-228">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="c0472-228">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="c0472-229">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0472-229">Response</span></span>
<span data-ttu-id="c0472-230">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c0472-230">If successful, this method returns a `201 Created` response code and a [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0472-231">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c0472-231">Example</span></span>

### <a name="request"></a><span data-ttu-id="c0472-232">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c0472-232">Request</span></span>
<span data-ttu-id="c0472-233">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c0472-233">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="c0472-234">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0472-234">Response</span></span>
<span data-ttu-id="c0472-p123">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c0472-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




