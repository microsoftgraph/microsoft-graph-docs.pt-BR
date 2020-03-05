---
title: Atualizar androidScepCertificateProfile
description: Atualiza as propriedades de um objeto androidScepCertificateProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 808822b8dd60e611ca8e36c505545a8a15626e2e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42443640"
---
# <a name="update-androidscepcertificateprofile"></a><span data-ttu-id="3f6cb-103">Atualizar androidScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="3f6cb-103">Update androidScepCertificateProfile</span></span>

<span data-ttu-id="3f6cb-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="3f6cb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3f6cb-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3f6cb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3f6cb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3f6cb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f6cb-107">Atualiza as propriedades de um objeto [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="3f6cb-107">Update the properties of a [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3f6cb-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3f6cb-108">Prerequisites</span></span>
<span data-ttu-id="3f6cb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3f6cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3f6cb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3f6cb-111">Permission type</span></span>|<span data-ttu-id="3f6cb-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3f6cb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3f6cb-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3f6cb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3f6cb-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f6cb-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3f6cb-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3f6cb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3f6cb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3f6cb-116">Not supported.</span></span>|
|<span data-ttu-id="3f6cb-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3f6cb-117">Application</span></span>|<span data-ttu-id="3f6cb-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f6cb-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3f6cb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3f6cb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="3f6cb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3f6cb-120">Request headers</span></span>
|<span data-ttu-id="3f6cb-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3f6cb-121">Header</span></span>|<span data-ttu-id="3f6cb-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3f6cb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3f6cb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3f6cb-123">Authorization</span></span>|<span data-ttu-id="3f6cb-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3f6cb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3f6cb-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3f6cb-125">Accept</span></span>|<span data-ttu-id="3f6cb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3f6cb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3f6cb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3f6cb-127">Request body</span></span>
<span data-ttu-id="3f6cb-128">No corpo da solicitação, forneça uma representação JSON do objeto [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="3f6cb-128">In the request body, supply a JSON representation for the [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) object.</span></span>

<span data-ttu-id="3f6cb-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="3f6cb-129">The following table shows the properties that are required when you create the [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md).</span></span>

|<span data-ttu-id="3f6cb-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3f6cb-130">Property</span></span>|<span data-ttu-id="3f6cb-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="3f6cb-131">Type</span></span>|<span data-ttu-id="3f6cb-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3f6cb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f6cb-133">id</span><span class="sxs-lookup"><span data-stu-id="3f6cb-133">id</span></span>|<span data-ttu-id="3f6cb-134">String</span><span class="sxs-lookup"><span data-stu-id="3f6cb-134">String</span></span>|<span data-ttu-id="3f6cb-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="3f6cb-135">Key of the entity.</span></span> <span data-ttu-id="3f6cb-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3f6cb-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f6cb-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3f6cb-137">lastModifiedDateTime</span></span>|<span data-ttu-id="3f6cb-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f6cb-138">DateTimeOffset</span></span>|<span data-ttu-id="3f6cb-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="3f6cb-139">DateTime the object was last modified.</span></span> <span data-ttu-id="3f6cb-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3f6cb-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f6cb-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3f6cb-141">roleScopeTagIds</span></span>|<span data-ttu-id="3f6cb-142">String collection</span><span class="sxs-lookup"><span data-stu-id="3f6cb-142">String collection</span></span>|<span data-ttu-id="3f6cb-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="3f6cb-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3f6cb-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3f6cb-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f6cb-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="3f6cb-145">supportsScopeTags</span></span>|<span data-ttu-id="3f6cb-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f6cb-146">Boolean</span></span>|<span data-ttu-id="3f6cb-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="3f6cb-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="3f6cb-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="3f6cb-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="3f6cb-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="3f6cb-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="3f6cb-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3f6cb-150">This property is read-only.</span></span> <span data-ttu-id="3f6cb-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3f6cb-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f6cb-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="3f6cb-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="3f6cb-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="3f6cb-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="3f6cb-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="3f6cb-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="3f6cb-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3f6cb-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f6cb-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="3f6cb-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="3f6cb-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="3f6cb-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="3f6cb-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="3f6cb-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="3f6cb-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3f6cb-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f6cb-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="3f6cb-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="3f6cb-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="3f6cb-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="3f6cb-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="3f6cb-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="3f6cb-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3f6cb-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f6cb-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3f6cb-164">createdDateTime</span></span>|<span data-ttu-id="3f6cb-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f6cb-165">DateTimeOffset</span></span>|<span data-ttu-id="3f6cb-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="3f6cb-166">DateTime the object was created.</span></span> <span data-ttu-id="3f6cb-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3f6cb-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f6cb-168">description</span><span class="sxs-lookup"><span data-stu-id="3f6cb-168">description</span></span>|<span data-ttu-id="3f6cb-169">String</span><span class="sxs-lookup"><span data-stu-id="3f6cb-169">String</span></span>|<span data-ttu-id="3f6cb-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3f6cb-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3f6cb-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3f6cb-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f6cb-172">displayName</span><span class="sxs-lookup"><span data-stu-id="3f6cb-172">displayName</span></span>|<span data-ttu-id="3f6cb-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3f6cb-173">String</span></span>|<span data-ttu-id="3f6cb-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3f6cb-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3f6cb-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3f6cb-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f6cb-176">versão</span><span class="sxs-lookup"><span data-stu-id="3f6cb-176">version</span></span>|<span data-ttu-id="3f6cb-177">Int32</span><span class="sxs-lookup"><span data-stu-id="3f6cb-177">Int32</span></span>|<span data-ttu-id="3f6cb-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3f6cb-178">Version of the device configuration.</span></span> <span data-ttu-id="3f6cb-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3f6cb-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f6cb-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="3f6cb-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="3f6cb-181">Int32</span><span class="sxs-lookup"><span data-stu-id="3f6cb-181">Int32</span></span>|<span data-ttu-id="3f6cb-182">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="3f6cb-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="3f6cb-183">Valores válidos de 1 a 99 herdados de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="3f6cb-183">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="3f6cb-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="3f6cb-184">subjectNameFormat</span></span>|[<span data-ttu-id="3f6cb-185">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="3f6cb-185">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="3f6cb-186">Formato do nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="3f6cb-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="3f6cb-187">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="3f6cb-187">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="3f6cb-188">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="3f6cb-188">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="3f6cb-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="3f6cb-189">subjectAlternativeNameType</span></span>|[<span data-ttu-id="3f6cb-190">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="3f6cb-190">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="3f6cb-191">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="3f6cb-191">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="3f6cb-192">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="3f6cb-192">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="3f6cb-193">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="3f6cb-193">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="3f6cb-194">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="3f6cb-194">certificateValidityPeriodValue</span></span>|<span data-ttu-id="3f6cb-195">Int32</span><span class="sxs-lookup"><span data-stu-id="3f6cb-195">Int32</span></span>|<span data-ttu-id="3f6cb-196">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="3f6cb-196">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="3f6cb-197">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="3f6cb-197">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="3f6cb-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="3f6cb-198">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="3f6cb-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="3f6cb-199">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="3f6cb-200">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="3f6cb-200">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="3f6cb-201">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="3f6cb-201">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="3f6cb-202">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="3f6cb-202">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="3f6cb-203">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="3f6cb-203">extendedKeyUsages</span></span>|<span data-ttu-id="3f6cb-204">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="3f6cb-204">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="3f6cb-205">Configurações de EKU (uso estendido de chave).</span><span class="sxs-lookup"><span data-stu-id="3f6cb-205">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="3f6cb-206">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="3f6cb-206">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="3f6cb-207">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="3f6cb-207">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="3f6cb-208">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="3f6cb-208">scepServerUrls</span></span>|<span data-ttu-id="3f6cb-209">String collection</span><span class="sxs-lookup"><span data-stu-id="3f6cb-209">String collection</span></span>|<span data-ttu-id="3f6cb-210">URL (s) do servidor de SCEP</span><span class="sxs-lookup"><span data-stu-id="3f6cb-210">SCEP Server Url(s)</span></span>|
|<span data-ttu-id="3f6cb-211">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="3f6cb-211">subjectNameFormatString</span></span>|<span data-ttu-id="3f6cb-212">String</span><span class="sxs-lookup"><span data-stu-id="3f6cb-212">String</span></span>|<span data-ttu-id="3f6cb-213">Formato personalizado a ser usado com SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="3f6cb-213">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="3f6cb-214">Exemplo: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = usuários corporativos, O = Contoso Corporation, L = Redmond, ST = WA, C = br</span><span class="sxs-lookup"><span data-stu-id="3f6cb-214">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="3f6cb-215">uso de</span><span class="sxs-lookup"><span data-stu-id="3f6cb-215">keyUsage</span></span>|[<span data-ttu-id="3f6cb-216">usos de</span><span class="sxs-lookup"><span data-stu-id="3f6cb-216">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="3f6cb-217">Uso da chave do SCEP.</span><span class="sxs-lookup"><span data-stu-id="3f6cb-217">SCEP Key Usage.</span></span> <span data-ttu-id="3f6cb-218">Os valores possíveis são: `keyEncipherment` e `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="3f6cb-218">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="3f6cb-219">keySize</span><span class="sxs-lookup"><span data-stu-id="3f6cb-219">keySize</span></span>|[<span data-ttu-id="3f6cb-220">keySize</span><span class="sxs-lookup"><span data-stu-id="3f6cb-220">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="3f6cb-221">Tamanho da chave SCEP.</span><span class="sxs-lookup"><span data-stu-id="3f6cb-221">SCEP Key Size.</span></span> <span data-ttu-id="3f6cb-222">Os valores possíveis são: `size1024` e `size2048`.</span><span class="sxs-lookup"><span data-stu-id="3f6cb-222">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="3f6cb-223">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="3f6cb-223">hashAlgorithm</span></span>|[<span data-ttu-id="3f6cb-224">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="3f6cb-224">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="3f6cb-225">Algoritmo de hash do SCEP.</span><span class="sxs-lookup"><span data-stu-id="3f6cb-225">SCEP Hash Algorithm.</span></span> <span data-ttu-id="3f6cb-226">Os valores possíveis são: `sha1` e `sha2`.</span><span class="sxs-lookup"><span data-stu-id="3f6cb-226">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="3f6cb-227">Subjectalternativenameformatstring foi</span><span class="sxs-lookup"><span data-stu-id="3f6cb-227">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="3f6cb-228">String</span><span class="sxs-lookup"><span data-stu-id="3f6cb-228">String</span></span>|<span data-ttu-id="3f6cb-229">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="3f6cb-229">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="3f6cb-230">Resposta</span><span class="sxs-lookup"><span data-stu-id="3f6cb-230">Response</span></span>
<span data-ttu-id="3f6cb-231">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3f6cb-231">If successful, this method returns a `200 OK` response code and an updated [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3f6cb-232">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3f6cb-232">Example</span></span>

### <a name="request"></a><span data-ttu-id="3f6cb-233">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3f6cb-233">Request</span></span>
<span data-ttu-id="3f6cb-234">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3f6cb-234">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3f6cb-235">Resposta</span><span class="sxs-lookup"><span data-stu-id="3f6cb-235">Response</span></span>
<span data-ttu-id="3f6cb-p123">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3f6cb-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





