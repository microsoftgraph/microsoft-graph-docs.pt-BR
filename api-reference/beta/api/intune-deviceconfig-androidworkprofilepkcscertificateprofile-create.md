---
title: Criar androidWorkProfilePkcsCertificateProfile
description: Criar um novo objeto androidWorkProfilePkcsCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 966a4c8d3d9e744867127524680492c8a93d8b15
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48022691"
---
# <a name="create-androidworkprofilepkcscertificateprofile"></a><span data-ttu-id="3f9fb-103">Criar androidWorkProfilePkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="3f9fb-103">Create androidWorkProfilePkcsCertificateProfile</span></span>

<span data-ttu-id="3f9fb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3f9fb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3f9fb-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3f9fb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3f9fb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3f9fb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f9fb-107">Criar um novo objeto [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="3f9fb-107">Create a new [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3f9fb-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3f9fb-108">Prerequisites</span></span>
<span data-ttu-id="3f9fb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3f9fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3f9fb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3f9fb-111">Permission type</span></span>|<span data-ttu-id="3f9fb-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3f9fb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3f9fb-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3f9fb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3f9fb-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f9fb-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3f9fb-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3f9fb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3f9fb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3f9fb-116">Not supported.</span></span>|
|<span data-ttu-id="3f9fb-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3f9fb-117">Application</span></span>|<span data-ttu-id="3f9fb-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f9fb-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3f9fb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3f9fb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3f9fb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3f9fb-120">Request headers</span></span>
|<span data-ttu-id="3f9fb-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3f9fb-121">Header</span></span>|<span data-ttu-id="3f9fb-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3f9fb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3f9fb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3f9fb-123">Authorization</span></span>|<span data-ttu-id="3f9fb-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3f9fb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3f9fb-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3f9fb-125">Accept</span></span>|<span data-ttu-id="3f9fb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3f9fb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3f9fb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3f9fb-127">Request body</span></span>
<span data-ttu-id="3f9fb-128">No corpo da solicitação, forneça uma representação JSON do objeto androidWorkProfilePkcsCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="3f9fb-128">In the request body, supply a JSON representation for the androidWorkProfilePkcsCertificateProfile object.</span></span>

<span data-ttu-id="3f9fb-129">A tabela a seguir mostra as propriedades que são necessárias ao criar androidWorkProfilePkcsCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="3f9fb-129">The following table shows the properties that are required when you create the androidWorkProfilePkcsCertificateProfile.</span></span>

|<span data-ttu-id="3f9fb-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3f9fb-130">Property</span></span>|<span data-ttu-id="3f9fb-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="3f9fb-131">Type</span></span>|<span data-ttu-id="3f9fb-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3f9fb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f9fb-133">id</span><span class="sxs-lookup"><span data-stu-id="3f9fb-133">id</span></span>|<span data-ttu-id="3f9fb-134">String</span><span class="sxs-lookup"><span data-stu-id="3f9fb-134">String</span></span>|<span data-ttu-id="3f9fb-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="3f9fb-135">Key of the entity.</span></span> <span data-ttu-id="3f9fb-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3f9fb-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f9fb-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3f9fb-137">lastModifiedDateTime</span></span>|<span data-ttu-id="3f9fb-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f9fb-138">DateTimeOffset</span></span>|<span data-ttu-id="3f9fb-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="3f9fb-139">DateTime the object was last modified.</span></span> <span data-ttu-id="3f9fb-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3f9fb-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f9fb-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3f9fb-141">roleScopeTagIds</span></span>|<span data-ttu-id="3f9fb-142">Coleção String</span><span class="sxs-lookup"><span data-stu-id="3f9fb-142">String collection</span></span>|<span data-ttu-id="3f9fb-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="3f9fb-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3f9fb-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3f9fb-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f9fb-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="3f9fb-145">supportsScopeTags</span></span>|<span data-ttu-id="3f9fb-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="3f9fb-146">Boolean</span></span>|<span data-ttu-id="3f9fb-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="3f9fb-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="3f9fb-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="3f9fb-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="3f9fb-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="3f9fb-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="3f9fb-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3f9fb-150">This property is read-only.</span></span> <span data-ttu-id="3f9fb-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3f9fb-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f9fb-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="3f9fb-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="3f9fb-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="3f9fb-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="3f9fb-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="3f9fb-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="3f9fb-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3f9fb-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f9fb-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="3f9fb-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="3f9fb-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="3f9fb-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="3f9fb-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="3f9fb-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="3f9fb-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3f9fb-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f9fb-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="3f9fb-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="3f9fb-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="3f9fb-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="3f9fb-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="3f9fb-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="3f9fb-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3f9fb-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f9fb-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3f9fb-164">createdDateTime</span></span>|<span data-ttu-id="3f9fb-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f9fb-165">DateTimeOffset</span></span>|<span data-ttu-id="3f9fb-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="3f9fb-166">DateTime the object was created.</span></span> <span data-ttu-id="3f9fb-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3f9fb-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f9fb-168">description</span><span class="sxs-lookup"><span data-stu-id="3f9fb-168">description</span></span>|<span data-ttu-id="3f9fb-169">String</span><span class="sxs-lookup"><span data-stu-id="3f9fb-169">String</span></span>|<span data-ttu-id="3f9fb-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3f9fb-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3f9fb-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3f9fb-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f9fb-172">displayName</span><span class="sxs-lookup"><span data-stu-id="3f9fb-172">displayName</span></span>|<span data-ttu-id="3f9fb-173">String</span><span class="sxs-lookup"><span data-stu-id="3f9fb-173">String</span></span>|<span data-ttu-id="3f9fb-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3f9fb-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3f9fb-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3f9fb-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f9fb-176">versão</span><span class="sxs-lookup"><span data-stu-id="3f9fb-176">version</span></span>|<span data-ttu-id="3f9fb-177">Int32</span><span class="sxs-lookup"><span data-stu-id="3f9fb-177">Int32</span></span>|<span data-ttu-id="3f9fb-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3f9fb-178">Version of the device configuration.</span></span> <span data-ttu-id="3f9fb-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3f9fb-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f9fb-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="3f9fb-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="3f9fb-181">Int32</span><span class="sxs-lookup"><span data-stu-id="3f9fb-181">Int32</span></span>|<span data-ttu-id="3f9fb-182">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="3f9fb-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="3f9fb-183">Valores válidos de 1 a 99 herdados de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="3f9fb-183">Valid values 1 to 99 Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="3f9fb-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="3f9fb-184">subjectNameFormat</span></span>|[<span data-ttu-id="3f9fb-185">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="3f9fb-185">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="3f9fb-186">Formato do nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="3f9fb-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="3f9fb-187">Herdado de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="3f9fb-187">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="3f9fb-188">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="3f9fb-188">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="3f9fb-189">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="3f9fb-189">certificateValidityPeriodValue</span></span>|<span data-ttu-id="3f9fb-190">Int32</span><span class="sxs-lookup"><span data-stu-id="3f9fb-190">Int32</span></span>|<span data-ttu-id="3f9fb-191">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="3f9fb-191">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="3f9fb-192">Herdado de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="3f9fb-192">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="3f9fb-193">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="3f9fb-193">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="3f9fb-194">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="3f9fb-194">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="3f9fb-195">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="3f9fb-195">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="3f9fb-196">Herdado de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="3f9fb-196">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="3f9fb-197">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="3f9fb-197">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="3f9fb-198">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="3f9fb-198">extendedKeyUsages</span></span>|<span data-ttu-id="3f9fb-199">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="3f9fb-199">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="3f9fb-200">Configurações de EKU (uso estendido de chave).</span><span class="sxs-lookup"><span data-stu-id="3f9fb-200">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="3f9fb-201">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="3f9fb-201">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="3f9fb-202">Herdado de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="3f9fb-202">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="3f9fb-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="3f9fb-203">subjectAlternativeNameType</span></span>|[<span data-ttu-id="3f9fb-204">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="3f9fb-204">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="3f9fb-205">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="3f9fb-205">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="3f9fb-206">Herdado de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="3f9fb-206">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="3f9fb-207">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="3f9fb-207">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="3f9fb-208">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="3f9fb-208">certificationAuthority</span></span>|<span data-ttu-id="3f9fb-209">String</span><span class="sxs-lookup"><span data-stu-id="3f9fb-209">String</span></span>|<span data-ttu-id="3f9fb-210">Autoridade de certificação PKCS</span><span class="sxs-lookup"><span data-stu-id="3f9fb-210">PKCS Certification Authority</span></span>|
|<span data-ttu-id="3f9fb-211">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="3f9fb-211">certificationAuthorityName</span></span>|<span data-ttu-id="3f9fb-212">String</span><span class="sxs-lookup"><span data-stu-id="3f9fb-212">String</span></span>|<span data-ttu-id="3f9fb-213">Nome da autoridade de certificação PKCS</span><span class="sxs-lookup"><span data-stu-id="3f9fb-213">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="3f9fb-214">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="3f9fb-214">certificateTemplateName</span></span>|<span data-ttu-id="3f9fb-215">String</span><span class="sxs-lookup"><span data-stu-id="3f9fb-215">String</span></span>|<span data-ttu-id="3f9fb-216">Nome do modelo de certificado PKCS</span><span class="sxs-lookup"><span data-stu-id="3f9fb-216">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="3f9fb-217">Subjectalternativenameformatstring foi</span><span class="sxs-lookup"><span data-stu-id="3f9fb-217">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="3f9fb-218">String</span><span class="sxs-lookup"><span data-stu-id="3f9fb-218">String</span></span>|<span data-ttu-id="3f9fb-219">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="3f9fb-219">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="3f9fb-220">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="3f9fb-220">subjectNameFormatString</span></span>|<span data-ttu-id="3f9fb-221">String</span><span class="sxs-lookup"><span data-stu-id="3f9fb-221">String</span></span>|<span data-ttu-id="3f9fb-222">Formato personalizado a ser usado com SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="3f9fb-222">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="3f9fb-223">Exemplo: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = usuários corporativos, O = Contoso Corporation, L = Redmond, ST = WA, C = br</span><span class="sxs-lookup"><span data-stu-id="3f9fb-223">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="3f9fb-224">certificateStore</span><span class="sxs-lookup"><span data-stu-id="3f9fb-224">certificateStore</span></span>|[<span data-ttu-id="3f9fb-225">certificateStore</span><span class="sxs-lookup"><span data-stu-id="3f9fb-225">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="3f9fb-226">Certificado de repositório de destino.</span><span class="sxs-lookup"><span data-stu-id="3f9fb-226">Target store certificate.</span></span> <span data-ttu-id="3f9fb-227">Os valores possíveis são: `user` e `machine`.</span><span class="sxs-lookup"><span data-stu-id="3f9fb-227">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="3f9fb-228">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="3f9fb-228">customSubjectAlternativeNames</span></span>|<span data-ttu-id="3f9fb-229">coleção [customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="3f9fb-229">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="3f9fb-230">Configurações de nome alternativo de entidade personalizada.</span><span class="sxs-lookup"><span data-stu-id="3f9fb-230">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="3f9fb-231">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="3f9fb-231">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="3f9fb-232">Resposta</span><span class="sxs-lookup"><span data-stu-id="3f9fb-232">Response</span></span>
<span data-ttu-id="3f9fb-233">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3f9fb-233">If successful, this method returns a `201 Created` response code and a [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3f9fb-234">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3f9fb-234">Example</span></span>

### <a name="request"></a><span data-ttu-id="3f9fb-235">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3f9fb-235">Request</span></span>
<span data-ttu-id="3f9fb-236">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3f9fb-236">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="3f9fb-237">Resposta</span><span class="sxs-lookup"><span data-stu-id="3f9fb-237">Response</span></span>
<span data-ttu-id="3f9fb-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3f9fb-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






