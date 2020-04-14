---
title: Atualizar androidDeviceOwnerScepCertificateProfile
description: Atualiza as propriedades de um objeto androidDeviceOwnerScepCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7572b205dc6e14a3269e5665fb2ba1adc0a133b5
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43350529"
---
# <a name="update-androiddeviceownerscepcertificateprofile"></a><span data-ttu-id="f8c81-103">Atualizar androidDeviceOwnerScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="f8c81-103">Update androidDeviceOwnerScepCertificateProfile</span></span>

<span data-ttu-id="f8c81-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f8c81-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f8c81-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f8c81-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f8c81-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f8c81-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f8c81-107">Atualiza as propriedades de um objeto [androidDeviceOwnerScepCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="f8c81-107">Update the properties of a [androidDeviceOwnerScepCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f8c81-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f8c81-108">Prerequisites</span></span>
<span data-ttu-id="f8c81-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8c81-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8c81-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f8c81-111">Permission type</span></span>|<span data-ttu-id="f8c81-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f8c81-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f8c81-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f8c81-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f8c81-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8c81-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f8c81-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f8c81-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f8c81-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f8c81-116">Not supported.</span></span>|
|<span data-ttu-id="f8c81-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f8c81-117">Application</span></span>|<span data-ttu-id="f8c81-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8c81-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f8c81-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f8c81-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f8c81-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f8c81-120">Request headers</span></span>
|<span data-ttu-id="f8c81-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f8c81-121">Header</span></span>|<span data-ttu-id="f8c81-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f8c81-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f8c81-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f8c81-123">Authorization</span></span>|<span data-ttu-id="f8c81-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f8c81-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f8c81-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f8c81-125">Accept</span></span>|<span data-ttu-id="f8c81-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f8c81-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8c81-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f8c81-127">Request body</span></span>
<span data-ttu-id="f8c81-128">No corpo da solicitação, forneça uma representação JSON do objeto [androidDeviceOwnerScepCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="f8c81-128">In the request body, supply a JSON representation for the [androidDeviceOwnerScepCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerscepcertificateprofile.md) object.</span></span>

<span data-ttu-id="f8c81-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidDeviceOwnerScepCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerscepcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="f8c81-129">The following table shows the properties that are required when you create the [androidDeviceOwnerScepCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerscepcertificateprofile.md).</span></span>

|<span data-ttu-id="f8c81-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f8c81-130">Property</span></span>|<span data-ttu-id="f8c81-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f8c81-131">Type</span></span>|<span data-ttu-id="f8c81-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f8c81-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8c81-133">id</span><span class="sxs-lookup"><span data-stu-id="f8c81-133">id</span></span>|<span data-ttu-id="f8c81-134">String</span><span class="sxs-lookup"><span data-stu-id="f8c81-134">String</span></span>|<span data-ttu-id="f8c81-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f8c81-135">Key of the entity.</span></span> <span data-ttu-id="f8c81-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8c81-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f8c81-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f8c81-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f8c81-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f8c81-138">DateTimeOffset</span></span>|<span data-ttu-id="f8c81-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="f8c81-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f8c81-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8c81-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f8c81-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f8c81-141">roleScopeTagIds</span></span>|<span data-ttu-id="f8c81-142">Coleção String</span><span class="sxs-lookup"><span data-stu-id="f8c81-142">String collection</span></span>|<span data-ttu-id="f8c81-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="f8c81-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f8c81-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8c81-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f8c81-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f8c81-145">supportsScopeTags</span></span>|<span data-ttu-id="f8c81-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="f8c81-146">Boolean</span></span>|<span data-ttu-id="f8c81-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="f8c81-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f8c81-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="f8c81-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f8c81-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="f8c81-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f8c81-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f8c81-150">This property is read-only.</span></span> <span data-ttu-id="f8c81-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8c81-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f8c81-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f8c81-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="f8c81-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f8c81-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="f8c81-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="f8c81-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="f8c81-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8c81-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f8c81-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f8c81-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="f8c81-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f8c81-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="f8c81-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="f8c81-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="f8c81-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8c81-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f8c81-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f8c81-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="f8c81-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f8c81-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="f8c81-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="f8c81-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="f8c81-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8c81-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f8c81-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f8c81-164">createdDateTime</span></span>|<span data-ttu-id="f8c81-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f8c81-165">DateTimeOffset</span></span>|<span data-ttu-id="f8c81-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="f8c81-166">DateTime the object was created.</span></span> <span data-ttu-id="f8c81-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8c81-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f8c81-168">description</span><span class="sxs-lookup"><span data-stu-id="f8c81-168">description</span></span>|<span data-ttu-id="f8c81-169">String</span><span class="sxs-lookup"><span data-stu-id="f8c81-169">String</span></span>|<span data-ttu-id="f8c81-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f8c81-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f8c81-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8c81-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f8c81-172">displayName</span><span class="sxs-lookup"><span data-stu-id="f8c81-172">displayName</span></span>|<span data-ttu-id="f8c81-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f8c81-173">String</span></span>|<span data-ttu-id="f8c81-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f8c81-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f8c81-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8c81-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f8c81-176">versão</span><span class="sxs-lookup"><span data-stu-id="f8c81-176">version</span></span>|<span data-ttu-id="f8c81-177">Int32</span><span class="sxs-lookup"><span data-stu-id="f8c81-177">Int32</span></span>|<span data-ttu-id="f8c81-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f8c81-178">Version of the device configuration.</span></span> <span data-ttu-id="f8c81-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8c81-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f8c81-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="f8c81-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="f8c81-181">Int32</span><span class="sxs-lookup"><span data-stu-id="f8c81-181">Int32</span></span>|<span data-ttu-id="f8c81-182">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="f8c81-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="f8c81-183">Valores válidos de 1 a 99 herdados de [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="f8c81-183">Valid values 1 to 99 Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span></span>|
|<span data-ttu-id="f8c81-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="f8c81-184">subjectNameFormat</span></span>|[<span data-ttu-id="f8c81-185">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="f8c81-185">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="f8c81-186">Formato do nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="f8c81-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="f8c81-187">Herdado de [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="f8c81-187">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span></span> <span data-ttu-id="f8c81-188">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="f8c81-188">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="f8c81-189">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="f8c81-189">certificateValidityPeriodValue</span></span>|<span data-ttu-id="f8c81-190">Int32</span><span class="sxs-lookup"><span data-stu-id="f8c81-190">Int32</span></span>|<span data-ttu-id="f8c81-191">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="f8c81-191">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="f8c81-192">Herdado de [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="f8c81-192">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span></span>|
|<span data-ttu-id="f8c81-193">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="f8c81-193">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="f8c81-194">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="f8c81-194">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="f8c81-195">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="f8c81-195">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="f8c81-196">Herdado de [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="f8c81-196">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span></span> <span data-ttu-id="f8c81-197">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="f8c81-197">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="f8c81-198">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="f8c81-198">extendedKeyUsages</span></span>|<span data-ttu-id="f8c81-199">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="f8c81-199">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="f8c81-200">Configurações de EKU (uso estendido de chave).</span><span class="sxs-lookup"><span data-stu-id="f8c81-200">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="f8c81-201">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="f8c81-201">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="f8c81-202">Herdado de [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="f8c81-202">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span></span>|
|<span data-ttu-id="f8c81-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="f8c81-203">subjectAlternativeNameType</span></span>|[<span data-ttu-id="f8c81-204">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="f8c81-204">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="f8c81-205">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="f8c81-205">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="f8c81-206">Herdado de [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="f8c81-206">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span></span> <span data-ttu-id="f8c81-207">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="f8c81-207">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="f8c81-208">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="f8c81-208">scepServerUrls</span></span>|<span data-ttu-id="f8c81-209">Coleção String</span><span class="sxs-lookup"><span data-stu-id="f8c81-209">String collection</span></span>|<span data-ttu-id="f8c81-210">URL (s) do servidor de SCEP</span><span class="sxs-lookup"><span data-stu-id="f8c81-210">SCEP Server Url(s)</span></span>|
|<span data-ttu-id="f8c81-211">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="f8c81-211">subjectNameFormatString</span></span>|<span data-ttu-id="f8c81-212">String</span><span class="sxs-lookup"><span data-stu-id="f8c81-212">String</span></span>|<span data-ttu-id="f8c81-213">Formato personalizado a ser usado com SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="f8c81-213">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="f8c81-214">Exemplo: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = usuários corporativos, O = Contoso Corporation, L = Redmond, ST = WA, C = br</span><span class="sxs-lookup"><span data-stu-id="f8c81-214">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="f8c81-215">uso de</span><span class="sxs-lookup"><span data-stu-id="f8c81-215">keyUsage</span></span>|[<span data-ttu-id="f8c81-216">usos de</span><span class="sxs-lookup"><span data-stu-id="f8c81-216">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="f8c81-217">Uso da chave do SCEP.</span><span class="sxs-lookup"><span data-stu-id="f8c81-217">SCEP Key Usage.</span></span> <span data-ttu-id="f8c81-218">Os valores possíveis são: `keyEncipherment` e `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="f8c81-218">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="f8c81-219">keySize</span><span class="sxs-lookup"><span data-stu-id="f8c81-219">keySize</span></span>|[<span data-ttu-id="f8c81-220">keySize</span><span class="sxs-lookup"><span data-stu-id="f8c81-220">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="f8c81-221">Tamanho da chave SCEP.</span><span class="sxs-lookup"><span data-stu-id="f8c81-221">SCEP Key Size.</span></span> <span data-ttu-id="f8c81-222">Os valores possíveis são: `size1024` e `size2048`.</span><span class="sxs-lookup"><span data-stu-id="f8c81-222">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="f8c81-223">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="f8c81-223">hashAlgorithm</span></span>|[<span data-ttu-id="f8c81-224">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="f8c81-224">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="f8c81-225">Algoritmo de hash do SCEP.</span><span class="sxs-lookup"><span data-stu-id="f8c81-225">SCEP Hash Algorithm.</span></span> <span data-ttu-id="f8c81-226">Os valores possíveis são: `sha1` e `sha2`.</span><span class="sxs-lookup"><span data-stu-id="f8c81-226">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="f8c81-227">Subjectalternativenameformatstring foi</span><span class="sxs-lookup"><span data-stu-id="f8c81-227">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="f8c81-228">String</span><span class="sxs-lookup"><span data-stu-id="f8c81-228">String</span></span>|<span data-ttu-id="f8c81-229">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="f8c81-229">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="f8c81-230">certificateStore</span><span class="sxs-lookup"><span data-stu-id="f8c81-230">certificateStore</span></span>|[<span data-ttu-id="f8c81-231">certificateStore</span><span class="sxs-lookup"><span data-stu-id="f8c81-231">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="f8c81-232">Certificado de repositório de destino.</span><span class="sxs-lookup"><span data-stu-id="f8c81-232">Target store certificate.</span></span> <span data-ttu-id="f8c81-233">Os valores possíveis são: `user` e `machine`.</span><span class="sxs-lookup"><span data-stu-id="f8c81-233">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="f8c81-234">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="f8c81-234">customSubjectAlternativeNames</span></span>|<span data-ttu-id="f8c81-235">coleção [customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="f8c81-235">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="f8c81-236">Configurações de nome alternativo de entidade personalizada.</span><span class="sxs-lookup"><span data-stu-id="f8c81-236">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="f8c81-237">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="f8c81-237">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="f8c81-238">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8c81-238">Response</span></span>
<span data-ttu-id="f8c81-239">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [androidDeviceOwnerScepCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerscepcertificateprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f8c81-239">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerScepCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8c81-240">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f8c81-240">Example</span></span>

### <a name="request"></a><span data-ttu-id="f8c81-241">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f8c81-241">Request</span></span>
<span data-ttu-id="f8c81-242">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f8c81-242">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1982

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerScepCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="f8c81-243">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8c81-243">Response</span></span>
<span data-ttu-id="f8c81-p125">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f8c81-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2154

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerScepCertificateProfile",
  "id": "7d8b9c9a-9c9a-7d8b-9a9c-8b7d9a9c8b7d",
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



