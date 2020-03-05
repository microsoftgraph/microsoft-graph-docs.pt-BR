---
title: Atualizar windows81SCEPCertificateProfile
description: Atualiza as propriedades de um objeto windows81SCEPCertificateProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 226424c812388bd912884af2c432882d6686b692
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42477060"
---
# <a name="update-windows81scepcertificateprofile"></a><span data-ttu-id="21db0-103">Atualizar windows81SCEPCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="21db0-103">Update windows81SCEPCertificateProfile</span></span>

<span data-ttu-id="21db0-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="21db0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="21db0-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="21db0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="21db0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="21db0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21db0-107">Atualiza as propriedades de um objeto [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="21db0-107">Update the properties of a [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="21db0-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="21db0-108">Prerequisites</span></span>
<span data-ttu-id="21db0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21db0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21db0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="21db0-111">Permission type</span></span>|<span data-ttu-id="21db0-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="21db0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21db0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="21db0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="21db0-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21db0-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="21db0-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="21db0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21db0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="21db0-116">Not supported.</span></span>|
|<span data-ttu-id="21db0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="21db0-117">Application</span></span>|<span data-ttu-id="21db0-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21db0-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="21db0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="21db0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="21db0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="21db0-120">Request headers</span></span>
|<span data-ttu-id="21db0-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="21db0-121">Header</span></span>|<span data-ttu-id="21db0-122">Valor</span><span class="sxs-lookup"><span data-stu-id="21db0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="21db0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="21db0-123">Authorization</span></span>|<span data-ttu-id="21db0-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="21db0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="21db0-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="21db0-125">Accept</span></span>|<span data-ttu-id="21db0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="21db0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="21db0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="21db0-127">Request body</span></span>
<span data-ttu-id="21db0-128">No corpo da solicitação, forneça uma representação JSON do objeto [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="21db0-128">In the request body, supply a JSON representation for the [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) object.</span></span>

<span data-ttu-id="21db0-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="21db0-129">The following table shows the properties that are required when you create the [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md).</span></span>

|<span data-ttu-id="21db0-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="21db0-130">Property</span></span>|<span data-ttu-id="21db0-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="21db0-131">Type</span></span>|<span data-ttu-id="21db0-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="21db0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21db0-133">id</span><span class="sxs-lookup"><span data-stu-id="21db0-133">id</span></span>|<span data-ttu-id="21db0-134">String</span><span class="sxs-lookup"><span data-stu-id="21db0-134">String</span></span>|<span data-ttu-id="21db0-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="21db0-135">Key of the entity.</span></span> <span data-ttu-id="21db0-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="21db0-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="21db0-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="21db0-137">lastModifiedDateTime</span></span>|<span data-ttu-id="21db0-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21db0-138">DateTimeOffset</span></span>|<span data-ttu-id="21db0-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="21db0-139">DateTime the object was last modified.</span></span> <span data-ttu-id="21db0-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="21db0-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="21db0-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="21db0-141">roleScopeTagIds</span></span>|<span data-ttu-id="21db0-142">String collection</span><span class="sxs-lookup"><span data-stu-id="21db0-142">String collection</span></span>|<span data-ttu-id="21db0-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="21db0-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="21db0-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="21db0-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="21db0-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="21db0-145">supportsScopeTags</span></span>|<span data-ttu-id="21db0-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="21db0-146">Boolean</span></span>|<span data-ttu-id="21db0-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="21db0-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="21db0-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="21db0-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="21db0-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="21db0-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="21db0-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="21db0-150">This property is read-only.</span></span> <span data-ttu-id="21db0-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="21db0-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="21db0-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="21db0-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="21db0-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="21db0-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="21db0-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="21db0-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="21db0-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="21db0-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="21db0-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="21db0-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="21db0-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="21db0-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="21db0-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="21db0-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="21db0-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="21db0-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="21db0-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="21db0-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="21db0-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="21db0-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="21db0-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="21db0-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="21db0-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="21db0-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="21db0-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="21db0-164">createdDateTime</span></span>|<span data-ttu-id="21db0-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21db0-165">DateTimeOffset</span></span>|<span data-ttu-id="21db0-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="21db0-166">DateTime the object was created.</span></span> <span data-ttu-id="21db0-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="21db0-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="21db0-168">description</span><span class="sxs-lookup"><span data-stu-id="21db0-168">description</span></span>|<span data-ttu-id="21db0-169">String</span><span class="sxs-lookup"><span data-stu-id="21db0-169">String</span></span>|<span data-ttu-id="21db0-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="21db0-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="21db0-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="21db0-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="21db0-172">displayName</span><span class="sxs-lookup"><span data-stu-id="21db0-172">displayName</span></span>|<span data-ttu-id="21db0-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="21db0-173">String</span></span>|<span data-ttu-id="21db0-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="21db0-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="21db0-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="21db0-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="21db0-176">versão</span><span class="sxs-lookup"><span data-stu-id="21db0-176">version</span></span>|<span data-ttu-id="21db0-177">Int32</span><span class="sxs-lookup"><span data-stu-id="21db0-177">Int32</span></span>|<span data-ttu-id="21db0-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="21db0-178">Version of the device configuration.</span></span> <span data-ttu-id="21db0-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="21db0-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="21db0-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="21db0-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="21db0-181">Int32</span><span class="sxs-lookup"><span data-stu-id="21db0-181">Int32</span></span>|<span data-ttu-id="21db0-182">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="21db0-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="21db0-183">Valores válidos de 1 a 99 herdados de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="21db0-183">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="21db0-184">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="21db0-184">keyStorageProvider</span></span>|[<span data-ttu-id="21db0-185">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="21db0-185">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="21db0-186">Provedor de armazenamento de chave (KSP) herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="21db0-186">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="21db0-187">Os valores possíveis são: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="21db0-187">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="21db0-188">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="21db0-188">subjectNameFormat</span></span>|[<span data-ttu-id="21db0-189">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="21db0-189">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="21db0-190">Formato do nome de entidade do certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="21db0-190">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="21db0-191">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="21db0-191">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="21db0-192">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="21db0-192">subjectAlternativeNameType</span></span>|[<span data-ttu-id="21db0-193">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="21db0-193">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="21db0-194">Tipo de nome alternativo de entidade do certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="21db0-194">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="21db0-195">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="21db0-195">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="21db0-196">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="21db0-196">certificateValidityPeriodValue</span></span>|<span data-ttu-id="21db0-197">Int32</span><span class="sxs-lookup"><span data-stu-id="21db0-197">Int32</span></span>|<span data-ttu-id="21db0-198">Valor para o período de validade do certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="21db0-198">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="21db0-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="21db0-199">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="21db0-200">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="21db0-200">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="21db0-201">Dimensionar o período de validade do certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="21db0-201">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="21db0-202">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="21db0-202">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="21db0-203">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="21db0-203">extendedKeyUsages</span></span>|<span data-ttu-id="21db0-204">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="21db0-204">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="21db0-205">Configurações de EKU (uso estendido de chave).</span><span class="sxs-lookup"><span data-stu-id="21db0-205">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="21db0-206">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="21db0-206">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="21db0-207">Herdado de [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="21db0-207">Inherited from [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="21db0-208">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="21db0-208">customSubjectAlternativeNames</span></span>|<span data-ttu-id="21db0-209">coleção [customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="21db0-209">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="21db0-210">Configurações de nome alternativo de entidade personalizada.</span><span class="sxs-lookup"><span data-stu-id="21db0-210">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="21db0-211">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="21db0-211">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="21db0-212">Herdado de [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="21db0-212">Inherited from [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="21db0-213">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="21db0-213">scepServerUrls</span></span>|<span data-ttu-id="21db0-214">String collection</span><span class="sxs-lookup"><span data-stu-id="21db0-214">String collection</span></span>|<span data-ttu-id="21db0-215">URL (s) do servidor de SCEP.</span><span class="sxs-lookup"><span data-stu-id="21db0-215">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="21db0-216">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="21db0-216">subjectNameFormatString</span></span>|<span data-ttu-id="21db0-217">String</span><span class="sxs-lookup"><span data-stu-id="21db0-217">String</span></span>|<span data-ttu-id="21db0-218">Formato personalizado a ser usado com SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="21db0-218">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="21db0-219">Exemplo: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = usuários corporativos, O = Contoso Corporation, L = Redmond, ST = WA, C = br</span><span class="sxs-lookup"><span data-stu-id="21db0-219">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="21db0-220">uso de</span><span class="sxs-lookup"><span data-stu-id="21db0-220">keyUsage</span></span>|[<span data-ttu-id="21db0-221">usos de</span><span class="sxs-lookup"><span data-stu-id="21db0-221">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="21db0-222">Uso da chave do SCEP.</span><span class="sxs-lookup"><span data-stu-id="21db0-222">SCEP Key Usage.</span></span> <span data-ttu-id="21db0-223">Os valores possíveis são: `keyEncipherment` e `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="21db0-223">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="21db0-224">keySize</span><span class="sxs-lookup"><span data-stu-id="21db0-224">keySize</span></span>|[<span data-ttu-id="21db0-225">keySize</span><span class="sxs-lookup"><span data-stu-id="21db0-225">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="21db0-226">Tamanho da chave SCEP.</span><span class="sxs-lookup"><span data-stu-id="21db0-226">SCEP Key Size.</span></span> <span data-ttu-id="21db0-227">Os valores possíveis são: `size1024` e `size2048`.</span><span class="sxs-lookup"><span data-stu-id="21db0-227">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="21db0-228">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="21db0-228">hashAlgorithm</span></span>|[<span data-ttu-id="21db0-229">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="21db0-229">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="21db0-230">Algoritmo de hash do SCEP.</span><span class="sxs-lookup"><span data-stu-id="21db0-230">SCEP Hash Algorithm.</span></span> <span data-ttu-id="21db0-231">Os valores possíveis são: `sha1` e `sha2`.</span><span class="sxs-lookup"><span data-stu-id="21db0-231">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="21db0-232">Subjectalternativenameformatstring foi</span><span class="sxs-lookup"><span data-stu-id="21db0-232">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="21db0-233">String</span><span class="sxs-lookup"><span data-stu-id="21db0-233">String</span></span>|<span data-ttu-id="21db0-234">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="21db0-234">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="21db0-235">certificateStore</span><span class="sxs-lookup"><span data-stu-id="21db0-235">certificateStore</span></span>|[<span data-ttu-id="21db0-236">certificateStore</span><span class="sxs-lookup"><span data-stu-id="21db0-236">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="21db0-237">Certificado de repositório de destino.</span><span class="sxs-lookup"><span data-stu-id="21db0-237">Target store certificate.</span></span> <span data-ttu-id="21db0-238">Os valores possíveis são: `user` e `machine`.</span><span class="sxs-lookup"><span data-stu-id="21db0-238">Possible values are: `user`, `machine`.</span></span>|



## <a name="response"></a><span data-ttu-id="21db0-239">Resposta</span><span class="sxs-lookup"><span data-stu-id="21db0-239">Response</span></span>
<span data-ttu-id="21db0-240">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="21db0-240">If successful, this method returns a `200 OK` response code and an updated [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21db0-241">Exemplo</span><span class="sxs-lookup"><span data-stu-id="21db0-241">Example</span></span>

### <a name="request"></a><span data-ttu-id="21db0-242">Solicitação</span><span class="sxs-lookup"><span data-stu-id="21db0-242">Request</span></span>
<span data-ttu-id="21db0-243">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="21db0-243">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2024

{
  "@odata.type": "#microsoft.graph.windows81SCEPCertificateProfile",
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
  "keyStorageProvider": "useTpmKspOtherwiseFail",
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
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
    }
  ],
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "certificateStore": "machine"
}
```

### <a name="response"></a><span data-ttu-id="21db0-244">Resposta</span><span class="sxs-lookup"><span data-stu-id="21db0-244">Response</span></span>
<span data-ttu-id="21db0-p125">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="21db0-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2196

{
  "@odata.type": "#microsoft.graph.windows81SCEPCertificateProfile",
  "id": "2daf8af2-8af2-2daf-f28a-af2df28aaf2d",
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
  "keyStorageProvider": "useTpmKspOtherwiseFail",
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
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
    }
  ],
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "certificateStore": "machine"
}
```





