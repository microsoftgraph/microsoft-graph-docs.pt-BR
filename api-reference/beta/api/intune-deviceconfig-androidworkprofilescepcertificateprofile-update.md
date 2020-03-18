---
title: Atualizar Entidadeandroidworkprofilescepcertificateprofile
description: Atualiza as propriedades de um objeto Entidadeandroidworkprofilescepcertificateprofile.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bf94c3f04e42945ffd783f58d5f287695fd4d6c6
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42757967"
---
# <a name="update-androidworkprofilescepcertificateprofile"></a><span data-ttu-id="df648-103">Atualizar Entidadeandroidworkprofilescepcertificateprofile</span><span class="sxs-lookup"><span data-stu-id="df648-103">Update androidWorkProfileScepCertificateProfile</span></span>

> <span data-ttu-id="df648-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="df648-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="df648-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="df648-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df648-106">Atualiza as propriedades de um objeto [entidadeandroidworkprofilescepcertificateprofile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="df648-106">Update the properties of a [androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="df648-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="df648-107">Prerequisites</span></span>
<span data-ttu-id="df648-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df648-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df648-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="df648-110">Permission type</span></span>|<span data-ttu-id="df648-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="df648-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="df648-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="df648-112">Delegated (work or school account)</span></span>|<span data-ttu-id="df648-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df648-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="df648-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="df648-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="df648-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="df648-115">Not supported.</span></span>|
|<span data-ttu-id="df648-116">Application</span><span class="sxs-lookup"><span data-stu-id="df648-116">Application</span></span>|<span data-ttu-id="df648-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df648-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="df648-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="df648-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="df648-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="df648-119">Request headers</span></span>
|<span data-ttu-id="df648-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="df648-120">Header</span></span>|<span data-ttu-id="df648-121">Valor</span><span class="sxs-lookup"><span data-stu-id="df648-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="df648-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="df648-122">Authorization</span></span>|<span data-ttu-id="df648-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="df648-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="df648-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="df648-124">Accept</span></span>|<span data-ttu-id="df648-125">application/json</span><span class="sxs-lookup"><span data-stu-id="df648-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="df648-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="df648-126">Request body</span></span>
<span data-ttu-id="df648-127">No corpo da solicitação, forneça uma representação JSON do objeto [entidadeandroidworkprofilescepcertificateprofile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="df648-127">In the request body, supply a JSON representation for the [androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) object.</span></span>

<span data-ttu-id="df648-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [entidadeandroidworkprofilescepcertificateprofile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="df648-128">The following table shows the properties that are required when you create the [androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md).</span></span>

|<span data-ttu-id="df648-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="df648-129">Property</span></span>|<span data-ttu-id="df648-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="df648-130">Type</span></span>|<span data-ttu-id="df648-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="df648-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df648-132">id</span><span class="sxs-lookup"><span data-stu-id="df648-132">id</span></span>|<span data-ttu-id="df648-133">String</span><span class="sxs-lookup"><span data-stu-id="df648-133">String</span></span>|<span data-ttu-id="df648-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="df648-134">Key of the entity.</span></span> <span data-ttu-id="df648-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="df648-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="df648-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="df648-136">lastModifiedDateTime</span></span>|<span data-ttu-id="df648-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="df648-137">DateTimeOffset</span></span>|<span data-ttu-id="df648-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="df648-138">DateTime the object was last modified.</span></span> <span data-ttu-id="df648-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="df648-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="df648-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="df648-140">roleScopeTagIds</span></span>|<span data-ttu-id="df648-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="df648-141">String collection</span></span>|<span data-ttu-id="df648-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="df648-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="df648-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="df648-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="df648-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="df648-144">supportsScopeTags</span></span>|<span data-ttu-id="df648-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="df648-145">Boolean</span></span>|<span data-ttu-id="df648-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="df648-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="df648-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="df648-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="df648-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="df648-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="df648-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="df648-149">This property is read-only.</span></span> <span data-ttu-id="df648-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="df648-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="df648-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="df648-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="df648-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="df648-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="df648-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="df648-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="df648-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="df648-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="df648-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="df648-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="df648-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="df648-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="df648-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="df648-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="df648-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="df648-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="df648-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="df648-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="df648-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="df648-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="df648-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="df648-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="df648-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="df648-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="df648-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="df648-163">createdDateTime</span></span>|<span data-ttu-id="df648-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="df648-164">DateTimeOffset</span></span>|<span data-ttu-id="df648-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="df648-165">DateTime the object was created.</span></span> <span data-ttu-id="df648-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="df648-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="df648-167">description</span><span class="sxs-lookup"><span data-stu-id="df648-167">description</span></span>|<span data-ttu-id="df648-168">String</span><span class="sxs-lookup"><span data-stu-id="df648-168">String</span></span>|<span data-ttu-id="df648-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="df648-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="df648-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="df648-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="df648-171">displayName</span><span class="sxs-lookup"><span data-stu-id="df648-171">displayName</span></span>|<span data-ttu-id="df648-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df648-172">String</span></span>|<span data-ttu-id="df648-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="df648-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="df648-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="df648-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="df648-175">versão</span><span class="sxs-lookup"><span data-stu-id="df648-175">version</span></span>|<span data-ttu-id="df648-176">Int32</span><span class="sxs-lookup"><span data-stu-id="df648-176">Int32</span></span>|<span data-ttu-id="df648-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="df648-177">Version of the device configuration.</span></span> <span data-ttu-id="df648-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="df648-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="df648-179">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="df648-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="df648-180">Int32</span><span class="sxs-lookup"><span data-stu-id="df648-180">Int32</span></span>|<span data-ttu-id="df648-181">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="df648-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="df648-182">Valores válidos de 1 a 99 herdados de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="df648-182">Valid values 1 to 99 Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="df648-183">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="df648-183">subjectNameFormat</span></span>|[<span data-ttu-id="df648-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="df648-184">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="df648-185">Formato do nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="df648-185">Certificate Subject Name Format.</span></span> <span data-ttu-id="df648-186">Herdado de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="df648-186">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="df648-187">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="df648-187">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="df648-188">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="df648-188">certificateValidityPeriodValue</span></span>|<span data-ttu-id="df648-189">Int32</span><span class="sxs-lookup"><span data-stu-id="df648-189">Int32</span></span>|<span data-ttu-id="df648-190">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="df648-190">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="df648-191">Herdado de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="df648-191">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="df648-192">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="df648-192">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="df648-193">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="df648-193">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="df648-194">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="df648-194">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="df648-195">Herdado de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="df648-195">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="df648-196">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="df648-196">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="df648-197">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="df648-197">extendedKeyUsages</span></span>|<span data-ttu-id="df648-198">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="df648-198">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="df648-199">Configurações de EKU (uso estendido de chave).</span><span class="sxs-lookup"><span data-stu-id="df648-199">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="df648-200">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="df648-200">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="df648-201">Herdado de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="df648-201">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="df648-202">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="df648-202">subjectAlternativeNameType</span></span>|[<span data-ttu-id="df648-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="df648-203">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="df648-204">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="df648-204">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="df648-205">Herdado de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="df648-205">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="df648-206">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="df648-206">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="df648-207">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="df648-207">scepServerUrls</span></span>|<span data-ttu-id="df648-208">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="df648-208">String collection</span></span>|<span data-ttu-id="df648-209">URL (s) do servidor de SCEP</span><span class="sxs-lookup"><span data-stu-id="df648-209">SCEP Server Url(s)</span></span>|
|<span data-ttu-id="df648-210">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="df648-210">subjectNameFormatString</span></span>|<span data-ttu-id="df648-211">String</span><span class="sxs-lookup"><span data-stu-id="df648-211">String</span></span>|<span data-ttu-id="df648-212">Formato personalizado a ser usado com SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="df648-212">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="df648-213">Exemplo: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = usuários corporativos, O = Contoso Corporation, L = Redmond, ST = WA, C = br</span><span class="sxs-lookup"><span data-stu-id="df648-213">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="df648-214">uso de</span><span class="sxs-lookup"><span data-stu-id="df648-214">keyUsage</span></span>|[<span data-ttu-id="df648-215">usos de</span><span class="sxs-lookup"><span data-stu-id="df648-215">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="df648-216">Uso da chave do SCEP.</span><span class="sxs-lookup"><span data-stu-id="df648-216">SCEP Key Usage.</span></span> <span data-ttu-id="df648-217">Os valores possíveis são: `keyEncipherment` e `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="df648-217">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="df648-218">keySize</span><span class="sxs-lookup"><span data-stu-id="df648-218">keySize</span></span>|[<span data-ttu-id="df648-219">keySize</span><span class="sxs-lookup"><span data-stu-id="df648-219">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="df648-220">Tamanho da chave SCEP.</span><span class="sxs-lookup"><span data-stu-id="df648-220">SCEP Key Size.</span></span> <span data-ttu-id="df648-221">Os valores possíveis são: `size1024` e `size2048`.</span><span class="sxs-lookup"><span data-stu-id="df648-221">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="df648-222">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="df648-222">hashAlgorithm</span></span>|[<span data-ttu-id="df648-223">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="df648-223">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="df648-224">Algoritmo de hash do SCEP.</span><span class="sxs-lookup"><span data-stu-id="df648-224">SCEP Hash Algorithm.</span></span> <span data-ttu-id="df648-225">Os valores possíveis são: `sha1` e `sha2`.</span><span class="sxs-lookup"><span data-stu-id="df648-225">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="df648-226">Subjectalternativenameformatstring foi</span><span class="sxs-lookup"><span data-stu-id="df648-226">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="df648-227">String</span><span class="sxs-lookup"><span data-stu-id="df648-227">String</span></span>|<span data-ttu-id="df648-228">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="df648-228">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="df648-229">certificateStore</span><span class="sxs-lookup"><span data-stu-id="df648-229">certificateStore</span></span>|[<span data-ttu-id="df648-230">certificateStore</span><span class="sxs-lookup"><span data-stu-id="df648-230">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="df648-231">Certificado de repositório de destino.</span><span class="sxs-lookup"><span data-stu-id="df648-231">Target store certificate.</span></span> <span data-ttu-id="df648-232">Os valores possíveis são: `user` e `machine`.</span><span class="sxs-lookup"><span data-stu-id="df648-232">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="df648-233">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="df648-233">customSubjectAlternativeNames</span></span>|<span data-ttu-id="df648-234">coleção [customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="df648-234">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="df648-235">Configurações de nome alternativo de entidade personalizada.</span><span class="sxs-lookup"><span data-stu-id="df648-235">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="df648-236">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="df648-236">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="df648-237">Resposta</span><span class="sxs-lookup"><span data-stu-id="df648-237">Response</span></span>
<span data-ttu-id="df648-238">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [entidadeandroidworkprofilescepcertificateprofile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="df648-238">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df648-239">Exemplo</span><span class="sxs-lookup"><span data-stu-id="df648-239">Example</span></span>

### <a name="request"></a><span data-ttu-id="df648-240">Solicitação</span><span class="sxs-lookup"><span data-stu-id="df648-240">Request</span></span>
<span data-ttu-id="df648-241">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="df648-241">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="df648-242">Resposta</span><span class="sxs-lookup"><span data-stu-id="df648-242">Response</span></span>
<span data-ttu-id="df648-p125">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="df648-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




