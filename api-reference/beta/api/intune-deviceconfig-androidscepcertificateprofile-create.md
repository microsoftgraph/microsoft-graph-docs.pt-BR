---
title: Criar androidScepCertificateProfile
description: Criar um novo objeto androidScepCertificateProfile.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7a4909201acb82309b47a407db0fd1a9cbf29195
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42758823"
---
# <a name="create-androidscepcertificateprofile"></a><span data-ttu-id="a2907-103">Criar androidScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="a2907-103">Create androidScepCertificateProfile</span></span>

> <span data-ttu-id="a2907-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a2907-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a2907-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a2907-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2907-106">Criar um novo objeto [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="a2907-106">Create a new [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a2907-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a2907-107">Prerequisites</span></span>
<span data-ttu-id="a2907-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2907-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2907-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a2907-110">Permission type</span></span>|<span data-ttu-id="a2907-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a2907-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2907-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a2907-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a2907-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2907-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a2907-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a2907-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2907-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a2907-115">Not supported.</span></span>|
|<span data-ttu-id="a2907-116">Application</span><span class="sxs-lookup"><span data-stu-id="a2907-116">Application</span></span>|<span data-ttu-id="a2907-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2907-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2907-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a2907-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a2907-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a2907-119">Request headers</span></span>
|<span data-ttu-id="a2907-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a2907-120">Header</span></span>|<span data-ttu-id="a2907-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a2907-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a2907-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a2907-122">Authorization</span></span>|<span data-ttu-id="a2907-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a2907-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a2907-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a2907-124">Accept</span></span>|<span data-ttu-id="a2907-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a2907-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2907-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a2907-126">Request body</span></span>
<span data-ttu-id="a2907-127">No corpo da solicitação, forneça uma representação JSON do objeto androidScepCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="a2907-127">In the request body, supply a JSON representation for the androidScepCertificateProfile object.</span></span>

<span data-ttu-id="a2907-128">A tabela a seguir mostra as propriedades que são necessárias ao criar androidScepCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="a2907-128">The following table shows the properties that are required when you create the androidScepCertificateProfile.</span></span>

|<span data-ttu-id="a2907-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a2907-129">Property</span></span>|<span data-ttu-id="a2907-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a2907-130">Type</span></span>|<span data-ttu-id="a2907-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2907-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2907-132">id</span><span class="sxs-lookup"><span data-stu-id="a2907-132">id</span></span>|<span data-ttu-id="a2907-133">String</span><span class="sxs-lookup"><span data-stu-id="a2907-133">String</span></span>|<span data-ttu-id="a2907-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a2907-134">Key of the entity.</span></span> <span data-ttu-id="a2907-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a2907-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a2907-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a2907-136">lastModifiedDateTime</span></span>|<span data-ttu-id="a2907-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2907-137">DateTimeOffset</span></span>|<span data-ttu-id="a2907-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="a2907-138">DateTime the object was last modified.</span></span> <span data-ttu-id="a2907-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a2907-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a2907-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a2907-140">roleScopeTagIds</span></span>|<span data-ttu-id="a2907-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a2907-141">String collection</span></span>|<span data-ttu-id="a2907-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="a2907-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a2907-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a2907-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a2907-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a2907-144">supportsScopeTags</span></span>|<span data-ttu-id="a2907-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2907-145">Boolean</span></span>|<span data-ttu-id="a2907-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="a2907-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a2907-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="a2907-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a2907-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="a2907-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a2907-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a2907-149">This property is read-only.</span></span> <span data-ttu-id="a2907-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a2907-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a2907-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a2907-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="a2907-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a2907-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="a2907-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="a2907-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="a2907-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a2907-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a2907-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a2907-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="a2907-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a2907-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="a2907-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="a2907-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="a2907-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a2907-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a2907-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a2907-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="a2907-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a2907-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="a2907-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="a2907-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="a2907-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a2907-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a2907-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a2907-163">createdDateTime</span></span>|<span data-ttu-id="a2907-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2907-164">DateTimeOffset</span></span>|<span data-ttu-id="a2907-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="a2907-165">DateTime the object was created.</span></span> <span data-ttu-id="a2907-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a2907-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a2907-167">description</span><span class="sxs-lookup"><span data-stu-id="a2907-167">description</span></span>|<span data-ttu-id="a2907-168">String</span><span class="sxs-lookup"><span data-stu-id="a2907-168">String</span></span>|<span data-ttu-id="a2907-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a2907-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a2907-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a2907-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a2907-171">displayName</span><span class="sxs-lookup"><span data-stu-id="a2907-171">displayName</span></span>|<span data-ttu-id="a2907-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a2907-172">String</span></span>|<span data-ttu-id="a2907-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a2907-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a2907-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a2907-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a2907-175">versão</span><span class="sxs-lookup"><span data-stu-id="a2907-175">version</span></span>|<span data-ttu-id="a2907-176">Int32</span><span class="sxs-lookup"><span data-stu-id="a2907-176">Int32</span></span>|<span data-ttu-id="a2907-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a2907-177">Version of the device configuration.</span></span> <span data-ttu-id="a2907-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a2907-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a2907-179">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="a2907-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="a2907-180">Int32</span><span class="sxs-lookup"><span data-stu-id="a2907-180">Int32</span></span>|<span data-ttu-id="a2907-181">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="a2907-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="a2907-182">Valores válidos de 1 a 99 herdados de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="a2907-182">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="a2907-183">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="a2907-183">subjectNameFormat</span></span>|[<span data-ttu-id="a2907-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="a2907-184">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="a2907-185">Formato do nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="a2907-185">Certificate Subject Name Format.</span></span> <span data-ttu-id="a2907-186">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="a2907-186">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="a2907-187">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="a2907-187">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="a2907-188">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="a2907-188">subjectAlternativeNameType</span></span>|[<span data-ttu-id="a2907-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="a2907-189">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="a2907-190">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="a2907-190">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="a2907-191">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="a2907-191">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="a2907-192">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="a2907-192">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="a2907-193">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="a2907-193">certificateValidityPeriodValue</span></span>|<span data-ttu-id="a2907-194">Int32</span><span class="sxs-lookup"><span data-stu-id="a2907-194">Int32</span></span>|<span data-ttu-id="a2907-195">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="a2907-195">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="a2907-196">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="a2907-196">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="a2907-197">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="a2907-197">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="a2907-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="a2907-198">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="a2907-199">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="a2907-199">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="a2907-200">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="a2907-200">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="a2907-201">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="a2907-201">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="a2907-202">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="a2907-202">extendedKeyUsages</span></span>|<span data-ttu-id="a2907-203">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="a2907-203">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="a2907-204">Configurações de EKU (uso estendido de chave).</span><span class="sxs-lookup"><span data-stu-id="a2907-204">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="a2907-205">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="a2907-205">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="a2907-206">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="a2907-206">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="a2907-207">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="a2907-207">scepServerUrls</span></span>|<span data-ttu-id="a2907-208">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a2907-208">String collection</span></span>|<span data-ttu-id="a2907-209">URL (s) do servidor de SCEP</span><span class="sxs-lookup"><span data-stu-id="a2907-209">SCEP Server Url(s)</span></span>|
|<span data-ttu-id="a2907-210">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="a2907-210">subjectNameFormatString</span></span>|<span data-ttu-id="a2907-211">String</span><span class="sxs-lookup"><span data-stu-id="a2907-211">String</span></span>|<span data-ttu-id="a2907-212">Formato personalizado a ser usado com SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="a2907-212">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="a2907-213">Exemplo: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = usuários corporativos, O = Contoso Corporation, L = Redmond, ST = WA, C = br</span><span class="sxs-lookup"><span data-stu-id="a2907-213">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="a2907-214">uso de</span><span class="sxs-lookup"><span data-stu-id="a2907-214">keyUsage</span></span>|[<span data-ttu-id="a2907-215">usos de</span><span class="sxs-lookup"><span data-stu-id="a2907-215">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="a2907-216">Uso da chave do SCEP.</span><span class="sxs-lookup"><span data-stu-id="a2907-216">SCEP Key Usage.</span></span> <span data-ttu-id="a2907-217">Os valores possíveis são: `keyEncipherment` e `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="a2907-217">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="a2907-218">keySize</span><span class="sxs-lookup"><span data-stu-id="a2907-218">keySize</span></span>|[<span data-ttu-id="a2907-219">keySize</span><span class="sxs-lookup"><span data-stu-id="a2907-219">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="a2907-220">Tamanho da chave SCEP.</span><span class="sxs-lookup"><span data-stu-id="a2907-220">SCEP Key Size.</span></span> <span data-ttu-id="a2907-221">Os valores possíveis são: `size1024` e `size2048`.</span><span class="sxs-lookup"><span data-stu-id="a2907-221">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="a2907-222">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="a2907-222">hashAlgorithm</span></span>|[<span data-ttu-id="a2907-223">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="a2907-223">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="a2907-224">Algoritmo de hash do SCEP.</span><span class="sxs-lookup"><span data-stu-id="a2907-224">SCEP Hash Algorithm.</span></span> <span data-ttu-id="a2907-225">Os valores possíveis são: `sha1` e `sha2`.</span><span class="sxs-lookup"><span data-stu-id="a2907-225">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="a2907-226">Subjectalternativenameformatstring foi</span><span class="sxs-lookup"><span data-stu-id="a2907-226">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="a2907-227">String</span><span class="sxs-lookup"><span data-stu-id="a2907-227">String</span></span>|<span data-ttu-id="a2907-228">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="a2907-228">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="a2907-229">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2907-229">Response</span></span>
<span data-ttu-id="a2907-230">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a2907-230">If successful, this method returns a `201 Created` response code and a [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2907-231">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a2907-231">Example</span></span>

### <a name="request"></a><span data-ttu-id="a2907-232">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a2907-232">Request</span></span>
<span data-ttu-id="a2907-233">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a2907-233">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a2907-234">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2907-234">Response</span></span>
<span data-ttu-id="a2907-p123">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a2907-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




