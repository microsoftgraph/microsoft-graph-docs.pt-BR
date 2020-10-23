---
title: Atualizar androidForWorkScepCertificateProfile
description: Atualiza as propriedades de um objeto androidForWorkScepCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bfb5561fee9263b55975425f07594199be2608ae
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48730047"
---
# <a name="update-androidforworkscepcertificateprofile"></a><span data-ttu-id="f9870-103">Atualizar androidForWorkScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="f9870-103">Update androidForWorkScepCertificateProfile</span></span>

<span data-ttu-id="f9870-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f9870-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f9870-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f9870-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f9870-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f9870-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9870-107">Atualiza as propriedades de um objeto [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="f9870-107">Update the properties of a [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f9870-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f9870-108">Prerequisites</span></span>
<span data-ttu-id="f9870-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9870-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9870-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f9870-111">Permission type</span></span>|<span data-ttu-id="f9870-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f9870-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f9870-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f9870-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f9870-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9870-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f9870-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f9870-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f9870-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f9870-116">Not supported.</span></span>|
|<span data-ttu-id="f9870-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f9870-117">Application</span></span>|<span data-ttu-id="f9870-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9870-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f9870-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f9870-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f9870-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f9870-120">Request headers</span></span>
|<span data-ttu-id="f9870-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f9870-121">Header</span></span>|<span data-ttu-id="f9870-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f9870-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f9870-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f9870-123">Authorization</span></span>|<span data-ttu-id="f9870-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f9870-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f9870-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f9870-125">Accept</span></span>|<span data-ttu-id="f9870-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f9870-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9870-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f9870-127">Request body</span></span>
<span data-ttu-id="f9870-128">No corpo da solicitação, forneça uma representação JSON do objeto [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="f9870-128">In the request body, supply a JSON representation for the [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) object.</span></span>

<span data-ttu-id="f9870-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="f9870-129">The following table shows the properties that are required when you create the [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md).</span></span>

|<span data-ttu-id="f9870-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f9870-130">Property</span></span>|<span data-ttu-id="f9870-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f9870-131">Type</span></span>|<span data-ttu-id="f9870-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9870-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9870-133">id</span><span class="sxs-lookup"><span data-stu-id="f9870-133">id</span></span>|<span data-ttu-id="f9870-134">String</span><span class="sxs-lookup"><span data-stu-id="f9870-134">String</span></span>|<span data-ttu-id="f9870-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f9870-135">Key of the entity.</span></span> <span data-ttu-id="f9870-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f9870-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f9870-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f9870-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f9870-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9870-138">DateTimeOffset</span></span>|<span data-ttu-id="f9870-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="f9870-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f9870-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f9870-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f9870-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f9870-141">roleScopeTagIds</span></span>|<span data-ttu-id="f9870-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f9870-142">String collection</span></span>|<span data-ttu-id="f9870-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="f9870-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f9870-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f9870-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f9870-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f9870-145">supportsScopeTags</span></span>|<span data-ttu-id="f9870-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="f9870-146">Boolean</span></span>|<span data-ttu-id="f9870-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="f9870-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f9870-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="f9870-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f9870-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="f9870-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f9870-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9870-150">This property is read-only.</span></span> <span data-ttu-id="f9870-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f9870-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f9870-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f9870-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="f9870-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f9870-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="f9870-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="f9870-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="f9870-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f9870-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f9870-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f9870-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="f9870-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f9870-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="f9870-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="f9870-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="f9870-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f9870-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f9870-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f9870-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="f9870-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f9870-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="f9870-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="f9870-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="f9870-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f9870-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f9870-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f9870-164">createdDateTime</span></span>|<span data-ttu-id="f9870-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9870-165">DateTimeOffset</span></span>|<span data-ttu-id="f9870-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="f9870-166">DateTime the object was created.</span></span> <span data-ttu-id="f9870-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f9870-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f9870-168">description</span><span class="sxs-lookup"><span data-stu-id="f9870-168">description</span></span>|<span data-ttu-id="f9870-169">String</span><span class="sxs-lookup"><span data-stu-id="f9870-169">String</span></span>|<span data-ttu-id="f9870-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9870-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f9870-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f9870-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f9870-172">displayName</span><span class="sxs-lookup"><span data-stu-id="f9870-172">displayName</span></span>|<span data-ttu-id="f9870-173">String</span><span class="sxs-lookup"><span data-stu-id="f9870-173">String</span></span>|<span data-ttu-id="f9870-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9870-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f9870-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f9870-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f9870-176">versão</span><span class="sxs-lookup"><span data-stu-id="f9870-176">version</span></span>|<span data-ttu-id="f9870-177">Int32</span><span class="sxs-lookup"><span data-stu-id="f9870-177">Int32</span></span>|<span data-ttu-id="f9870-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9870-178">Version of the device configuration.</span></span> <span data-ttu-id="f9870-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f9870-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f9870-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="f9870-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="f9870-181">Int32</span><span class="sxs-lookup"><span data-stu-id="f9870-181">Int32</span></span>|<span data-ttu-id="f9870-182">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="f9870-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="f9870-183">Valores válidos de 1 a 99 herdados de [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="f9870-183">Valid values 1 to 99 Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="f9870-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="f9870-184">subjectNameFormat</span></span>|[<span data-ttu-id="f9870-185">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="f9870-185">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="f9870-186">Formato do nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="f9870-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="f9870-187">Herdado de [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="f9870-187">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="f9870-188">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="f9870-188">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="f9870-189">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="f9870-189">certificateValidityPeriodValue</span></span>|<span data-ttu-id="f9870-190">Int32</span><span class="sxs-lookup"><span data-stu-id="f9870-190">Int32</span></span>|<span data-ttu-id="f9870-191">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="f9870-191">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="f9870-192">Herdado de [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="f9870-192">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="f9870-193">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="f9870-193">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="f9870-194">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="f9870-194">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="f9870-195">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="f9870-195">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="f9870-196">Herdado de [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="f9870-196">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="f9870-197">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="f9870-197">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="f9870-198">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="f9870-198">extendedKeyUsages</span></span>|<span data-ttu-id="f9870-199">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="f9870-199">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="f9870-200">Configurações de EKU (uso estendido de chave).</span><span class="sxs-lookup"><span data-stu-id="f9870-200">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="f9870-201">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="f9870-201">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="f9870-202">Herdado de [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="f9870-202">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="f9870-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="f9870-203">subjectAlternativeNameType</span></span>|[<span data-ttu-id="f9870-204">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="f9870-204">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="f9870-205">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="f9870-205">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="f9870-206">Herdado de [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="f9870-206">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="f9870-207">Os possíveis valores são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span><span class="sxs-lookup"><span data-stu-id="f9870-207">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span></span>|
|<span data-ttu-id="f9870-208">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="f9870-208">scepServerUrls</span></span>|<span data-ttu-id="f9870-209">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f9870-209">String collection</span></span>|<span data-ttu-id="f9870-210">URL (s) do servidor de SCEP</span><span class="sxs-lookup"><span data-stu-id="f9870-210">SCEP Server Url(s)</span></span>|
|<span data-ttu-id="f9870-211">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="f9870-211">subjectNameFormatString</span></span>|<span data-ttu-id="f9870-212">String</span><span class="sxs-lookup"><span data-stu-id="f9870-212">String</span></span>|<span data-ttu-id="f9870-213">Formato personalizado a ser usado com SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="f9870-213">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="f9870-214">Exemplo: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = usuários corporativos, O = Contoso Corporation, L = Redmond, ST = WA, C = br</span><span class="sxs-lookup"><span data-stu-id="f9870-214">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="f9870-215">uso de</span><span class="sxs-lookup"><span data-stu-id="f9870-215">keyUsage</span></span>|[<span data-ttu-id="f9870-216">usos de</span><span class="sxs-lookup"><span data-stu-id="f9870-216">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="f9870-217">Uso da chave do SCEP.</span><span class="sxs-lookup"><span data-stu-id="f9870-217">SCEP Key Usage.</span></span> <span data-ttu-id="f9870-218">Os valores possíveis são: `keyEncipherment` e `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="f9870-218">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="f9870-219">keySize</span><span class="sxs-lookup"><span data-stu-id="f9870-219">keySize</span></span>|[<span data-ttu-id="f9870-220">keySize</span><span class="sxs-lookup"><span data-stu-id="f9870-220">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="f9870-221">Tamanho da chave SCEP.</span><span class="sxs-lookup"><span data-stu-id="f9870-221">SCEP Key Size.</span></span> <span data-ttu-id="f9870-222">Os valores possíveis são: `size1024`, `size2048`, `size4096`.</span><span class="sxs-lookup"><span data-stu-id="f9870-222">Possible values are: `size1024`, `size2048`, `size4096`.</span></span>|
|<span data-ttu-id="f9870-223">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="f9870-223">hashAlgorithm</span></span>|[<span data-ttu-id="f9870-224">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="f9870-224">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="f9870-225">Algoritmo de hash do SCEP.</span><span class="sxs-lookup"><span data-stu-id="f9870-225">SCEP Hash Algorithm.</span></span> <span data-ttu-id="f9870-226">Os valores possíveis são: `sha1` e `sha2`.</span><span class="sxs-lookup"><span data-stu-id="f9870-226">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="f9870-227">Subjectalternativenameformatstring foi</span><span class="sxs-lookup"><span data-stu-id="f9870-227">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="f9870-228">String</span><span class="sxs-lookup"><span data-stu-id="f9870-228">String</span></span>|<span data-ttu-id="f9870-229">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="f9870-229">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="f9870-230">certificateStore</span><span class="sxs-lookup"><span data-stu-id="f9870-230">certificateStore</span></span>|[<span data-ttu-id="f9870-231">certificateStore</span><span class="sxs-lookup"><span data-stu-id="f9870-231">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="f9870-232">Certificado de repositório de destino.</span><span class="sxs-lookup"><span data-stu-id="f9870-232">Target store certificate.</span></span> <span data-ttu-id="f9870-233">Os valores possíveis são: `user` e `machine`.</span><span class="sxs-lookup"><span data-stu-id="f9870-233">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="f9870-234">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="f9870-234">customSubjectAlternativeNames</span></span>|<span data-ttu-id="f9870-235">coleção [customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="f9870-235">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="f9870-236">Configurações de nome alternativo de entidade personalizada.</span><span class="sxs-lookup"><span data-stu-id="f9870-236">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="f9870-237">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="f9870-237">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="f9870-238">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9870-238">Response</span></span>
<span data-ttu-id="f9870-239">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f9870-239">If successful, this method returns a `200 OK` response code and an updated [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9870-240">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f9870-240">Example</span></span>

### <a name="request"></a><span data-ttu-id="f9870-241">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f9870-241">Request</span></span>
<span data-ttu-id="f9870-242">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f9870-242">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1978

{
  "@odata.type": "#microsoft.graph.androidForWorkScepCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="f9870-243">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9870-243">Response</span></span>
<span data-ttu-id="f9870-p125">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f9870-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2150

{
  "@odata.type": "#microsoft.graph.androidForWorkScepCertificateProfile",
  "id": "09e532af-32af-09e5-af32-e509af32e509",
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





