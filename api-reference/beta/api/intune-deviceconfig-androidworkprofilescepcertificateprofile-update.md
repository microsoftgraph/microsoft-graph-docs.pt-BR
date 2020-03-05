---
title: Atualizar Entidadeandroidworkprofilescepcertificateprofile
description: Atualiza as propriedades de um objeto Entidadeandroidworkprofilescepcertificateprofile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: eac42f69b2acff1586891cea59e73e57d9449f9a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42449485"
---
# <a name="update-androidworkprofilescepcertificateprofile"></a><span data-ttu-id="5a453-103">Atualizar Entidadeandroidworkprofilescepcertificateprofile</span><span class="sxs-lookup"><span data-stu-id="5a453-103">Update androidWorkProfileScepCertificateProfile</span></span>

<span data-ttu-id="5a453-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="5a453-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5a453-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5a453-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5a453-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5a453-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5a453-107">Atualiza as propriedades de um objeto [entidadeandroidworkprofilescepcertificateprofile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="5a453-107">Update the properties of a [androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5a453-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5a453-108">Prerequisites</span></span>
<span data-ttu-id="5a453-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a453-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a453-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5a453-111">Permission type</span></span>|<span data-ttu-id="5a453-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5a453-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5a453-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5a453-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5a453-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a453-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5a453-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5a453-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5a453-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5a453-116">Not supported.</span></span>|
|<span data-ttu-id="5a453-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5a453-117">Application</span></span>|<span data-ttu-id="5a453-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a453-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5a453-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5a453-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="5a453-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5a453-120">Request headers</span></span>
|<span data-ttu-id="5a453-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5a453-121">Header</span></span>|<span data-ttu-id="5a453-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5a453-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5a453-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5a453-123">Authorization</span></span>|<span data-ttu-id="5a453-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5a453-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5a453-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5a453-125">Accept</span></span>|<span data-ttu-id="5a453-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5a453-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5a453-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5a453-127">Request body</span></span>
<span data-ttu-id="5a453-128">No corpo da solicitação, forneça uma representação JSON do objeto [entidadeandroidworkprofilescepcertificateprofile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="5a453-128">In the request body, supply a JSON representation for the [androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) object.</span></span>

<span data-ttu-id="5a453-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [entidadeandroidworkprofilescepcertificateprofile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="5a453-129">The following table shows the properties that are required when you create the [androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md).</span></span>

|<span data-ttu-id="5a453-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5a453-130">Property</span></span>|<span data-ttu-id="5a453-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="5a453-131">Type</span></span>|<span data-ttu-id="5a453-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a453-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a453-133">id</span><span class="sxs-lookup"><span data-stu-id="5a453-133">id</span></span>|<span data-ttu-id="5a453-134">String</span><span class="sxs-lookup"><span data-stu-id="5a453-134">String</span></span>|<span data-ttu-id="5a453-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="5a453-135">Key of the entity.</span></span> <span data-ttu-id="5a453-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5a453-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5a453-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5a453-137">lastModifiedDateTime</span></span>|<span data-ttu-id="5a453-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5a453-138">DateTimeOffset</span></span>|<span data-ttu-id="5a453-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="5a453-139">DateTime the object was last modified.</span></span> <span data-ttu-id="5a453-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5a453-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5a453-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5a453-141">roleScopeTagIds</span></span>|<span data-ttu-id="5a453-142">String collection</span><span class="sxs-lookup"><span data-stu-id="5a453-142">String collection</span></span>|<span data-ttu-id="5a453-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="5a453-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="5a453-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5a453-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5a453-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="5a453-145">supportsScopeTags</span></span>|<span data-ttu-id="5a453-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="5a453-146">Boolean</span></span>|<span data-ttu-id="5a453-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="5a453-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="5a453-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="5a453-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="5a453-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="5a453-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="5a453-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5a453-150">This property is read-only.</span></span> <span data-ttu-id="5a453-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5a453-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5a453-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="5a453-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="5a453-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="5a453-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="5a453-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="5a453-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="5a453-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5a453-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5a453-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="5a453-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="5a453-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="5a453-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="5a453-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="5a453-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="5a453-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5a453-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5a453-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="5a453-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="5a453-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="5a453-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="5a453-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="5a453-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="5a453-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5a453-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5a453-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5a453-164">createdDateTime</span></span>|<span data-ttu-id="5a453-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5a453-165">DateTimeOffset</span></span>|<span data-ttu-id="5a453-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="5a453-166">DateTime the object was created.</span></span> <span data-ttu-id="5a453-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5a453-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5a453-168">description</span><span class="sxs-lookup"><span data-stu-id="5a453-168">description</span></span>|<span data-ttu-id="5a453-169">String</span><span class="sxs-lookup"><span data-stu-id="5a453-169">String</span></span>|<span data-ttu-id="5a453-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5a453-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5a453-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5a453-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5a453-172">displayName</span><span class="sxs-lookup"><span data-stu-id="5a453-172">displayName</span></span>|<span data-ttu-id="5a453-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5a453-173">String</span></span>|<span data-ttu-id="5a453-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5a453-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5a453-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5a453-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5a453-176">versão</span><span class="sxs-lookup"><span data-stu-id="5a453-176">version</span></span>|<span data-ttu-id="5a453-177">Int32</span><span class="sxs-lookup"><span data-stu-id="5a453-177">Int32</span></span>|<span data-ttu-id="5a453-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5a453-178">Version of the device configuration.</span></span> <span data-ttu-id="5a453-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5a453-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5a453-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="5a453-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="5a453-181">Int32</span><span class="sxs-lookup"><span data-stu-id="5a453-181">Int32</span></span>|<span data-ttu-id="5a453-182">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="5a453-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="5a453-183">Valores válidos de 1 a 99 herdados de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="5a453-183">Valid values 1 to 99 Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="5a453-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="5a453-184">subjectNameFormat</span></span>|[<span data-ttu-id="5a453-185">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="5a453-185">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="5a453-186">Formato do nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="5a453-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="5a453-187">Herdado de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="5a453-187">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="5a453-188">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="5a453-188">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="5a453-189">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="5a453-189">certificateValidityPeriodValue</span></span>|<span data-ttu-id="5a453-190">Int32</span><span class="sxs-lookup"><span data-stu-id="5a453-190">Int32</span></span>|<span data-ttu-id="5a453-191">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="5a453-191">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="5a453-192">Herdado de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="5a453-192">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="5a453-193">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="5a453-193">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="5a453-194">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="5a453-194">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="5a453-195">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="5a453-195">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="5a453-196">Herdado de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="5a453-196">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="5a453-197">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="5a453-197">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="5a453-198">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="5a453-198">extendedKeyUsages</span></span>|<span data-ttu-id="5a453-199">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="5a453-199">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="5a453-200">Configurações de EKU (uso estendido de chave).</span><span class="sxs-lookup"><span data-stu-id="5a453-200">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="5a453-201">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="5a453-201">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="5a453-202">Herdado de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="5a453-202">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="5a453-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="5a453-203">subjectAlternativeNameType</span></span>|[<span data-ttu-id="5a453-204">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="5a453-204">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="5a453-205">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="5a453-205">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="5a453-206">Herdado de [entidadeandroidworkprofilecertificateprofilebase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="5a453-206">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="5a453-207">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="5a453-207">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="5a453-208">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="5a453-208">scepServerUrls</span></span>|<span data-ttu-id="5a453-209">String collection</span><span class="sxs-lookup"><span data-stu-id="5a453-209">String collection</span></span>|<span data-ttu-id="5a453-210">URL (s) do servidor de SCEP</span><span class="sxs-lookup"><span data-stu-id="5a453-210">SCEP Server Url(s)</span></span>|
|<span data-ttu-id="5a453-211">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="5a453-211">subjectNameFormatString</span></span>|<span data-ttu-id="5a453-212">String</span><span class="sxs-lookup"><span data-stu-id="5a453-212">String</span></span>|<span data-ttu-id="5a453-213">Formato personalizado a ser usado com SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="5a453-213">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="5a453-214">Exemplo: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = usuários corporativos, O = Contoso Corporation, L = Redmond, ST = WA, C = br</span><span class="sxs-lookup"><span data-stu-id="5a453-214">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="5a453-215">uso de</span><span class="sxs-lookup"><span data-stu-id="5a453-215">keyUsage</span></span>|[<span data-ttu-id="5a453-216">usos de</span><span class="sxs-lookup"><span data-stu-id="5a453-216">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="5a453-217">Uso da chave do SCEP.</span><span class="sxs-lookup"><span data-stu-id="5a453-217">SCEP Key Usage.</span></span> <span data-ttu-id="5a453-218">Os valores possíveis são: `keyEncipherment` e `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="5a453-218">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="5a453-219">keySize</span><span class="sxs-lookup"><span data-stu-id="5a453-219">keySize</span></span>|[<span data-ttu-id="5a453-220">keySize</span><span class="sxs-lookup"><span data-stu-id="5a453-220">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="5a453-221">Tamanho da chave SCEP.</span><span class="sxs-lookup"><span data-stu-id="5a453-221">SCEP Key Size.</span></span> <span data-ttu-id="5a453-222">Os valores possíveis são: `size1024` e `size2048`.</span><span class="sxs-lookup"><span data-stu-id="5a453-222">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="5a453-223">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="5a453-223">hashAlgorithm</span></span>|[<span data-ttu-id="5a453-224">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="5a453-224">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="5a453-225">Algoritmo de hash do SCEP.</span><span class="sxs-lookup"><span data-stu-id="5a453-225">SCEP Hash Algorithm.</span></span> <span data-ttu-id="5a453-226">Os valores possíveis são: `sha1` e `sha2`.</span><span class="sxs-lookup"><span data-stu-id="5a453-226">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="5a453-227">Subjectalternativenameformatstring foi</span><span class="sxs-lookup"><span data-stu-id="5a453-227">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="5a453-228">String</span><span class="sxs-lookup"><span data-stu-id="5a453-228">String</span></span>|<span data-ttu-id="5a453-229">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="5a453-229">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="5a453-230">certificateStore</span><span class="sxs-lookup"><span data-stu-id="5a453-230">certificateStore</span></span>|[<span data-ttu-id="5a453-231">certificateStore</span><span class="sxs-lookup"><span data-stu-id="5a453-231">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="5a453-232">Certificado de repositório de destino.</span><span class="sxs-lookup"><span data-stu-id="5a453-232">Target store certificate.</span></span> <span data-ttu-id="5a453-233">Os valores possíveis são: `user` e `machine`.</span><span class="sxs-lookup"><span data-stu-id="5a453-233">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="5a453-234">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="5a453-234">customSubjectAlternativeNames</span></span>|<span data-ttu-id="5a453-235">coleção [customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="5a453-235">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="5a453-236">Configurações de nome alternativo de entidade personalizada.</span><span class="sxs-lookup"><span data-stu-id="5a453-236">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="5a453-237">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="5a453-237">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="5a453-238">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a453-238">Response</span></span>
<span data-ttu-id="5a453-239">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [entidadeandroidworkprofilescepcertificateprofile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5a453-239">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a453-240">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5a453-240">Example</span></span>

### <a name="request"></a><span data-ttu-id="5a453-241">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5a453-241">Request</span></span>
<span data-ttu-id="5a453-242">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5a453-242">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5a453-243">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a453-243">Response</span></span>
<span data-ttu-id="5a453-p125">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5a453-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





