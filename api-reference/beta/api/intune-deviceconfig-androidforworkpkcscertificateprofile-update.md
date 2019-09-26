---
title: Atualizar androidForWorkPkcsCertificateProfile
description: Atualiza as propriedades de um objeto androidForWorkPkcsCertificateProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1d33e7ea2524e0f7b245f3de183c76fdc91bed43
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37169308"
---
# <a name="update-androidforworkpkcscertificateprofile"></a><span data-ttu-id="b096a-103">Atualizar androidForWorkPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="b096a-103">Update androidForWorkPkcsCertificateProfile</span></span>

> <span data-ttu-id="b096a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b096a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b096a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b096a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b096a-106">Atualiza as propriedades de um objeto [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="b096a-106">Update the properties of a [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b096a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b096a-107">Prerequisites</span></span>
<span data-ttu-id="b096a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b096a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b096a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b096a-110">Permission type</span></span>|<span data-ttu-id="b096a-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b096a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b096a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b096a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b096a-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b096a-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b096a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b096a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b096a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b096a-115">Not supported.</span></span>|
|<span data-ttu-id="b096a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b096a-116">Application</span></span>|<span data-ttu-id="b096a-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b096a-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b096a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b096a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b096a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b096a-119">Request headers</span></span>
|<span data-ttu-id="b096a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b096a-120">Header</span></span>|<span data-ttu-id="b096a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b096a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b096a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b096a-122">Authorization</span></span>|<span data-ttu-id="b096a-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b096a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b096a-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b096a-124">Accept</span></span>|<span data-ttu-id="b096a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b096a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b096a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b096a-126">Request body</span></span>
<span data-ttu-id="b096a-127">No corpo da solicitação, forneça uma representação JSON do objeto [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="b096a-127">In the request body, supply a JSON representation for the [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) object.</span></span>

<span data-ttu-id="b096a-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="b096a-128">The following table shows the properties that are required when you create the [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md).</span></span>

|<span data-ttu-id="b096a-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b096a-129">Property</span></span>|<span data-ttu-id="b096a-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b096a-130">Type</span></span>|<span data-ttu-id="b096a-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b096a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b096a-132">id</span><span class="sxs-lookup"><span data-stu-id="b096a-132">id</span></span>|<span data-ttu-id="b096a-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b096a-133">String</span></span>|<span data-ttu-id="b096a-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b096a-134">Key of the entity.</span></span> <span data-ttu-id="b096a-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b096a-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b096a-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b096a-136">lastModifiedDateTime</span></span>|<span data-ttu-id="b096a-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b096a-137">DateTimeOffset</span></span>|<span data-ttu-id="b096a-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="b096a-138">DateTime the object was last modified.</span></span> <span data-ttu-id="b096a-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b096a-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b096a-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b096a-140">roleScopeTagIds</span></span>|<span data-ttu-id="b096a-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b096a-141">String collection</span></span>|<span data-ttu-id="b096a-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="b096a-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b096a-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b096a-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b096a-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b096a-144">supportsScopeTags</span></span>|<span data-ttu-id="b096a-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="b096a-145">Boolean</span></span>|<span data-ttu-id="b096a-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="b096a-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b096a-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="b096a-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b096a-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="b096a-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b096a-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b096a-149">This property is read-only.</span></span> <span data-ttu-id="b096a-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b096a-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b096a-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b096a-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="b096a-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b096a-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="b096a-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="b096a-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="b096a-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b096a-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b096a-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b096a-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="b096a-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b096a-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="b096a-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="b096a-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="b096a-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b096a-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b096a-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b096a-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="b096a-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b096a-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="b096a-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="b096a-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="b096a-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b096a-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b096a-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b096a-163">createdDateTime</span></span>|<span data-ttu-id="b096a-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b096a-164">DateTimeOffset</span></span>|<span data-ttu-id="b096a-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="b096a-165">DateTime the object was created.</span></span> <span data-ttu-id="b096a-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b096a-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b096a-167">descrição</span><span class="sxs-lookup"><span data-stu-id="b096a-167">description</span></span>|<span data-ttu-id="b096a-168">String</span><span class="sxs-lookup"><span data-stu-id="b096a-168">String</span></span>|<span data-ttu-id="b096a-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b096a-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b096a-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b096a-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b096a-171">displayName</span><span class="sxs-lookup"><span data-stu-id="b096a-171">displayName</span></span>|<span data-ttu-id="b096a-172">String</span><span class="sxs-lookup"><span data-stu-id="b096a-172">String</span></span>|<span data-ttu-id="b096a-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b096a-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b096a-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b096a-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b096a-175">versão</span><span class="sxs-lookup"><span data-stu-id="b096a-175">version</span></span>|<span data-ttu-id="b096a-176">Int32</span><span class="sxs-lookup"><span data-stu-id="b096a-176">Int32</span></span>|<span data-ttu-id="b096a-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b096a-177">Version of the device configuration.</span></span> <span data-ttu-id="b096a-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b096a-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b096a-179">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="b096a-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="b096a-180">Int32</span><span class="sxs-lookup"><span data-stu-id="b096a-180">Int32</span></span>|<span data-ttu-id="b096a-181">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="b096a-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="b096a-182">Valores válidos de 1 a 99 herdados de [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="b096a-182">Valid values 1 to 99 Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="b096a-183">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="b096a-183">subjectNameFormat</span></span>|[<span data-ttu-id="b096a-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="b096a-184">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="b096a-185">Formato do nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="b096a-185">Certificate Subject Name Format.</span></span> <span data-ttu-id="b096a-186">Herdado de [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="b096a-186">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="b096a-187">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="b096a-187">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="b096a-188">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="b096a-188">certificateValidityPeriodValue</span></span>|<span data-ttu-id="b096a-189">Int32</span><span class="sxs-lookup"><span data-stu-id="b096a-189">Int32</span></span>|<span data-ttu-id="b096a-190">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="b096a-190">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="b096a-191">Herdado de [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="b096a-191">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="b096a-192">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="b096a-192">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="b096a-193">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="b096a-193">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="b096a-194">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="b096a-194">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="b096a-195">Herdado de [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="b096a-195">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="b096a-196">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="b096a-196">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="b096a-197">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="b096a-197">extendedKeyUsages</span></span>|<span data-ttu-id="b096a-198">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="b096a-198">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="b096a-199">Configurações de EKU (uso estendido de chave).</span><span class="sxs-lookup"><span data-stu-id="b096a-199">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="b096a-200">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="b096a-200">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="b096a-201">Herdado de [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="b096a-201">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="b096a-202">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="b096a-202">subjectAlternativeNameType</span></span>|[<span data-ttu-id="b096a-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="b096a-203">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="b096a-204">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="b096a-204">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="b096a-205">Herdado de [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="b096a-205">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="b096a-206">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="b096a-206">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="b096a-207">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="b096a-207">certificationAuthority</span></span>|<span data-ttu-id="b096a-208">String</span><span class="sxs-lookup"><span data-stu-id="b096a-208">String</span></span>|<span data-ttu-id="b096a-209">Autoridade de certificação PKCS</span><span class="sxs-lookup"><span data-stu-id="b096a-209">PKCS Certification Authority</span></span>|
|<span data-ttu-id="b096a-210">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="b096a-210">certificationAuthorityName</span></span>|<span data-ttu-id="b096a-211">String</span><span class="sxs-lookup"><span data-stu-id="b096a-211">String</span></span>|<span data-ttu-id="b096a-212">Nome da autoridade de certificação PKCS</span><span class="sxs-lookup"><span data-stu-id="b096a-212">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="b096a-213">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="b096a-213">certificateTemplateName</span></span>|<span data-ttu-id="b096a-214">String</span><span class="sxs-lookup"><span data-stu-id="b096a-214">String</span></span>|<span data-ttu-id="b096a-215">Nome do modelo de certificado PKCS</span><span class="sxs-lookup"><span data-stu-id="b096a-215">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="b096a-216">Subjectalternativenameformatstring foi</span><span class="sxs-lookup"><span data-stu-id="b096a-216">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="b096a-217">String</span><span class="sxs-lookup"><span data-stu-id="b096a-217">String</span></span>|<span data-ttu-id="b096a-218">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="b096a-218">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="b096a-219">Resposta</span><span class="sxs-lookup"><span data-stu-id="b096a-219">Response</span></span>
<span data-ttu-id="b096a-220">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b096a-220">If successful, this method returns a `200 OK` response code and an updated [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b096a-221">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b096a-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="b096a-222">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b096a-222">Request</span></span>
<span data-ttu-id="b096a-223">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b096a-223">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1738

{
  "@odata.type": "#microsoft.graph.androidForWorkPkcsCertificateProfile",
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
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```

### <a name="response"></a><span data-ttu-id="b096a-224">Resposta</span><span class="sxs-lookup"><span data-stu-id="b096a-224">Response</span></span>
<span data-ttu-id="b096a-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b096a-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1910

{
  "@odata.type": "#microsoft.graph.androidForWorkPkcsCertificateProfile",
  "id": "0a2d7691-7691-0a2d-9176-2d0a91762d0a",
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
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```




