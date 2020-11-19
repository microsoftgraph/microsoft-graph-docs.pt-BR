---
title: Atualizar Entidadeandroidworkprofilescepcertificateprofile
description: Atualiza as propriedades de um objeto Entidadeandroidworkprofilescepcertificateprofile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9102001c9de9fbfea0ded7edad9c95a699b13baf
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49206879"
---
# <a name="update-androidworkprofilescepcertificateprofile"></a><span data-ttu-id="246f6-103">Atualizar Entidadeandroidworkprofilescepcertificateprofile</span><span class="sxs-lookup"><span data-stu-id="246f6-103">Update androidWorkProfileScepCertificateProfile</span></span>

<span data-ttu-id="246f6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="246f6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="246f6-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="246f6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="246f6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="246f6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="246f6-107">Atualiza as propriedades de um objeto [entidadeandroidworkprofilescepcertificateprofile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="246f6-107">Update the properties of a [androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="246f6-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="246f6-108">Prerequisites</span></span>
<span data-ttu-id="246f6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="246f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="246f6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="246f6-111">Permission type</span></span>|<span data-ttu-id="246f6-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="246f6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="246f6-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="246f6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="246f6-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="246f6-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="246f6-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="246f6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="246f6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="246f6-116">Not supported.</span></span>|
|<span data-ttu-id="246f6-117">Application</span><span class="sxs-lookup"><span data-stu-id="246f6-117">Application</span></span>|<span data-ttu-id="246f6-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="246f6-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="246f6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="246f6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="246f6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="246f6-120">Request headers</span></span>
|<span data-ttu-id="246f6-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="246f6-121">Header</span></span>|<span data-ttu-id="246f6-122">Valor</span><span class="sxs-lookup"><span data-stu-id="246f6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="246f6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="246f6-123">Authorization</span></span>|<span data-ttu-id="246f6-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="246f6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="246f6-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="246f6-125">Accept</span></span>|<span data-ttu-id="246f6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="246f6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="246f6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="246f6-127">Request body</span></span>
<span data-ttu-id="246f6-128">No corpo da solicitação, forneça uma representação JSON do objeto [entidadeandroidworkprofilescepcertificateprofile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="246f6-128">In the request body, supply a JSON representation for the [androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) object.</span></span>

<span data-ttu-id="246f6-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [entidadeandroidworkprofilescepcertificateprofile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="246f6-129">The following table shows the properties that are required when you create the [androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md).</span></span>

|<span data-ttu-id="246f6-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="246f6-130">Property</span></span>|<span data-ttu-id="246f6-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="246f6-131">Type</span></span>|<span data-ttu-id="246f6-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="246f6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="246f6-133">id</span><span class="sxs-lookup"><span data-stu-id="246f6-133">id</span></span>|<span data-ttu-id="246f6-134">String</span><span class="sxs-lookup"><span data-stu-id="246f6-134">String</span></span>|<span data-ttu-id="246f6-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="246f6-135">Key of the entity.</span></span> <span data-ttu-id="246f6-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="246f6-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="246f6-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="246f6-137">lastModifiedDateTime</span></span>|<span data-ttu-id="246f6-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="246f6-138">DateTimeOffset</span></span>|<span data-ttu-id="246f6-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="246f6-139">DateTime the object was last modified.</span></span> <span data-ttu-id="246f6-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="246f6-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="246f6-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="246f6-141">roleScopeTagIds</span></span>|<span data-ttu-id="246f6-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="246f6-142">String collection</span></span>|<span data-ttu-id="246f6-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="246f6-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="246f6-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="246f6-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="246f6-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="246f6-145">supportsScopeTags</span></span>|<span data-ttu-id="246f6-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="246f6-146">Boolean</span></span>|<span data-ttu-id="246f6-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="246f6-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="246f6-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="246f6-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="246f6-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="246f6-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="246f6-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="246f6-150">This property is read-only.</span></span> <span data-ttu-id="246f6-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="246f6-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="246f6-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="246f6-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="246f6-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="246f6-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="246f6-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="246f6-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="246f6-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="246f6-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="246f6-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="246f6-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="246f6-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="246f6-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="246f6-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="246f6-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="246f6-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="246f6-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="246f6-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="246f6-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="246f6-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="246f6-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="246f6-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="246f6-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="246f6-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="246f6-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="246f6-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="246f6-164">createdDateTime</span></span>|<span data-ttu-id="246f6-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="246f6-165">DateTimeOffset</span></span>|<span data-ttu-id="246f6-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="246f6-166">DateTime the object was created.</span></span> <span data-ttu-id="246f6-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="246f6-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="246f6-168">description</span><span class="sxs-lookup"><span data-stu-id="246f6-168">description</span></span>|<span data-ttu-id="246f6-169">String</span><span class="sxs-lookup"><span data-stu-id="246f6-169">String</span></span>|<span data-ttu-id="246f6-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="246f6-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="246f6-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="246f6-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="246f6-172">displayName</span><span class="sxs-lookup"><span data-stu-id="246f6-172">displayName</span></span>|<span data-ttu-id="246f6-173">String</span><span class="sxs-lookup"><span data-stu-id="246f6-173">String</span></span>|<span data-ttu-id="246f6-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="246f6-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="246f6-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="246f6-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="246f6-176">versão</span><span class="sxs-lookup"><span data-stu-id="246f6-176">version</span></span>|<span data-ttu-id="246f6-177">Int32</span><span class="sxs-lookup"><span data-stu-id="246f6-177">Int32</span></span>|<span data-ttu-id="246f6-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="246f6-178">Version of the device configuration.</span></span> <span data-ttu-id="246f6-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="246f6-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="246f6-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="246f6-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="246f6-181">Int32</span><span class="sxs-lookup"><span data-stu-id="246f6-181">Int32</span></span>|<span data-ttu-id="246f6-182">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="246f6-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="246f6-183">Valores válidos de 1 a 99 herdados de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="246f6-183">Valid values 1 to 99 Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="246f6-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="246f6-184">subjectNameFormat</span></span>|[<span data-ttu-id="246f6-185">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="246f6-185">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="246f6-186">Formato do nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="246f6-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="246f6-187">Herdado de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="246f6-187">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="246f6-188">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="246f6-188">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="246f6-189">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="246f6-189">certificateValidityPeriodValue</span></span>|<span data-ttu-id="246f6-190">Int32</span><span class="sxs-lookup"><span data-stu-id="246f6-190">Int32</span></span>|<span data-ttu-id="246f6-191">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="246f6-191">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="246f6-192">Herdado de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="246f6-192">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="246f6-193">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="246f6-193">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="246f6-194">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="246f6-194">certificateValidityPeriodScale</span></span>](../resources/intune-shared-certificatevalidityperiodscale.md)|<span data-ttu-id="246f6-195">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="246f6-195">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="246f6-196">Herdado de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="246f6-196">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="246f6-197">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="246f6-197">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="246f6-198">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="246f6-198">extendedKeyUsages</span></span>|<span data-ttu-id="246f6-199">coleção [extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="246f6-199">[extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="246f6-200">Configurações de EKU (uso estendido de chave).</span><span class="sxs-lookup"><span data-stu-id="246f6-200">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="246f6-201">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="246f6-201">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="246f6-202">Herdado de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="246f6-202">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="246f6-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="246f6-203">subjectAlternativeNameType</span></span>|[<span data-ttu-id="246f6-204">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="246f6-204">subjectAlternativeNameType</span></span>](../resources/intune-shared-subjectalternativenametype.md)|<span data-ttu-id="246f6-205">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="246f6-205">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="246f6-206">Herdado de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="246f6-206">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="246f6-207">Os possíveis valores são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span><span class="sxs-lookup"><span data-stu-id="246f6-207">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span></span>|
|<span data-ttu-id="246f6-208">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="246f6-208">scepServerUrls</span></span>|<span data-ttu-id="246f6-209">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="246f6-209">String collection</span></span>|<span data-ttu-id="246f6-210">URL (s) do servidor de SCEP</span><span class="sxs-lookup"><span data-stu-id="246f6-210">SCEP Server Url(s)</span></span>|
|<span data-ttu-id="246f6-211">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="246f6-211">subjectNameFormatString</span></span>|<span data-ttu-id="246f6-212">String</span><span class="sxs-lookup"><span data-stu-id="246f6-212">String</span></span>|<span data-ttu-id="246f6-213">Formato personalizado a ser usado com SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="246f6-213">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="246f6-214">Exemplo: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = usuários corporativos, O = Contoso Corporation, L = Redmond, ST = WA, C = br</span><span class="sxs-lookup"><span data-stu-id="246f6-214">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="246f6-215">uso de</span><span class="sxs-lookup"><span data-stu-id="246f6-215">keyUsage</span></span>|[<span data-ttu-id="246f6-216">usos de</span><span class="sxs-lookup"><span data-stu-id="246f6-216">keyUsages</span></span>](../resources/intune-shared-keyusages.md)|<span data-ttu-id="246f6-217">Uso da chave do SCEP.</span><span class="sxs-lookup"><span data-stu-id="246f6-217">SCEP Key Usage.</span></span> <span data-ttu-id="246f6-218">Os valores possíveis são: `keyEncipherment` e `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="246f6-218">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="246f6-219">keySize</span><span class="sxs-lookup"><span data-stu-id="246f6-219">keySize</span></span>|[<span data-ttu-id="246f6-220">keySize</span><span class="sxs-lookup"><span data-stu-id="246f6-220">keySize</span></span>](../resources/intune-shared-keysize.md)|<span data-ttu-id="246f6-221">Tamanho da chave SCEP.</span><span class="sxs-lookup"><span data-stu-id="246f6-221">SCEP Key Size.</span></span> <span data-ttu-id="246f6-222">Os valores possíveis são: `size1024`, `size2048`, `size4096`.</span><span class="sxs-lookup"><span data-stu-id="246f6-222">Possible values are: `size1024`, `size2048`, `size4096`.</span></span>|
|<span data-ttu-id="246f6-223">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="246f6-223">hashAlgorithm</span></span>|[<span data-ttu-id="246f6-224">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="246f6-224">hashAlgorithms</span></span>](../resources/intune-shared-hashalgorithms.md)|<span data-ttu-id="246f6-225">Algoritmo de hash do SCEP.</span><span class="sxs-lookup"><span data-stu-id="246f6-225">SCEP Hash Algorithm.</span></span> <span data-ttu-id="246f6-226">Os valores possíveis são: `sha1` e `sha2`.</span><span class="sxs-lookup"><span data-stu-id="246f6-226">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="246f6-227">Subjectalternativenameformatstring foi</span><span class="sxs-lookup"><span data-stu-id="246f6-227">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="246f6-228">String</span><span class="sxs-lookup"><span data-stu-id="246f6-228">String</span></span>|<span data-ttu-id="246f6-229">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="246f6-229">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="246f6-230">certificateStore</span><span class="sxs-lookup"><span data-stu-id="246f6-230">certificateStore</span></span>|[<span data-ttu-id="246f6-231">certificateStore</span><span class="sxs-lookup"><span data-stu-id="246f6-231">certificateStore</span></span>](../resources/intune-shared-certificatestore.md)|<span data-ttu-id="246f6-232">Certificado de repositório de destino.</span><span class="sxs-lookup"><span data-stu-id="246f6-232">Target store certificate.</span></span> <span data-ttu-id="246f6-233">Os valores possíveis são: `user` e `machine`.</span><span class="sxs-lookup"><span data-stu-id="246f6-233">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="246f6-234">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="246f6-234">customSubjectAlternativeNames</span></span>|<span data-ttu-id="246f6-235">coleção [customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="246f6-235">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="246f6-236">Configurações de nome alternativo de entidade personalizada.</span><span class="sxs-lookup"><span data-stu-id="246f6-236">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="246f6-237">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="246f6-237">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="246f6-238">Resposta</span><span class="sxs-lookup"><span data-stu-id="246f6-238">Response</span></span>
<span data-ttu-id="246f6-239">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [entidadeandroidworkprofilescepcertificateprofile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="246f6-239">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="246f6-240">Exemplo</span><span class="sxs-lookup"><span data-stu-id="246f6-240">Example</span></span>

### <a name="request"></a><span data-ttu-id="246f6-241">Solicitação</span><span class="sxs-lookup"><span data-stu-id="246f6-241">Request</span></span>
<span data-ttu-id="246f6-242">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="246f6-242">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="246f6-243">Resposta</span><span class="sxs-lookup"><span data-stu-id="246f6-243">Response</span></span>
<span data-ttu-id="246f6-p125">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="246f6-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




