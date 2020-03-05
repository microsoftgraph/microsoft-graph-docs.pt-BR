---
title: Atualizar windows10PkcsCertificateProfile
description: Atualiza as propriedades de um objeto windows10PkcsCertificateProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: edff7c82688c8198d8e5b3fe74dc88a26d4f49ff
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42478145"
---
# <a name="update-windows10pkcscertificateprofile"></a><span data-ttu-id="45e79-103">Atualizar windows10PkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="45e79-103">Update windows10PkcsCertificateProfile</span></span>

<span data-ttu-id="45e79-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="45e79-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="45e79-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="45e79-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="45e79-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="45e79-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45e79-107">Atualiza as propriedades de um objeto [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="45e79-107">Update the properties of a [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="45e79-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="45e79-108">Prerequisites</span></span>
<span data-ttu-id="45e79-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45e79-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45e79-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="45e79-111">Permission type</span></span>|<span data-ttu-id="45e79-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="45e79-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45e79-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="45e79-113">Delegated (work or school account)</span></span>|<span data-ttu-id="45e79-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45e79-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="45e79-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="45e79-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45e79-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="45e79-116">Not supported.</span></span>|
|<span data-ttu-id="45e79-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="45e79-117">Application</span></span>|<span data-ttu-id="45e79-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45e79-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="45e79-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="45e79-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="45e79-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="45e79-120">Request headers</span></span>
|<span data-ttu-id="45e79-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="45e79-121">Header</span></span>|<span data-ttu-id="45e79-122">Valor</span><span class="sxs-lookup"><span data-stu-id="45e79-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45e79-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="45e79-123">Authorization</span></span>|<span data-ttu-id="45e79-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="45e79-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="45e79-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="45e79-125">Accept</span></span>|<span data-ttu-id="45e79-126">application/json</span><span class="sxs-lookup"><span data-stu-id="45e79-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45e79-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="45e79-127">Request body</span></span>
<span data-ttu-id="45e79-128">No corpo da solicitação, forneça uma representação JSON do objeto [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="45e79-128">In the request body, supply a JSON representation for the [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) object.</span></span>

<span data-ttu-id="45e79-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="45e79-129">The following table shows the properties that are required when you create the [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md).</span></span>

|<span data-ttu-id="45e79-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="45e79-130">Property</span></span>|<span data-ttu-id="45e79-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="45e79-131">Type</span></span>|<span data-ttu-id="45e79-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="45e79-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45e79-133">id</span><span class="sxs-lookup"><span data-stu-id="45e79-133">id</span></span>|<span data-ttu-id="45e79-134">String</span><span class="sxs-lookup"><span data-stu-id="45e79-134">String</span></span>|<span data-ttu-id="45e79-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="45e79-135">Key of the entity.</span></span> <span data-ttu-id="45e79-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45e79-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45e79-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="45e79-137">lastModifiedDateTime</span></span>|<span data-ttu-id="45e79-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45e79-138">DateTimeOffset</span></span>|<span data-ttu-id="45e79-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="45e79-139">DateTime the object was last modified.</span></span> <span data-ttu-id="45e79-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45e79-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45e79-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="45e79-141">roleScopeTagIds</span></span>|<span data-ttu-id="45e79-142">String collection</span><span class="sxs-lookup"><span data-stu-id="45e79-142">String collection</span></span>|<span data-ttu-id="45e79-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="45e79-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="45e79-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45e79-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45e79-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="45e79-145">supportsScopeTags</span></span>|<span data-ttu-id="45e79-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="45e79-146">Boolean</span></span>|<span data-ttu-id="45e79-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="45e79-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="45e79-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="45e79-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="45e79-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="45e79-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="45e79-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45e79-150">This property is read-only.</span></span> <span data-ttu-id="45e79-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45e79-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45e79-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="45e79-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="45e79-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="45e79-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="45e79-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="45e79-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="45e79-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45e79-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45e79-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="45e79-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="45e79-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="45e79-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="45e79-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="45e79-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="45e79-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45e79-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45e79-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="45e79-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="45e79-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="45e79-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="45e79-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="45e79-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="45e79-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45e79-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45e79-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="45e79-164">createdDateTime</span></span>|<span data-ttu-id="45e79-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45e79-165">DateTimeOffset</span></span>|<span data-ttu-id="45e79-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="45e79-166">DateTime the object was created.</span></span> <span data-ttu-id="45e79-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45e79-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45e79-168">description</span><span class="sxs-lookup"><span data-stu-id="45e79-168">description</span></span>|<span data-ttu-id="45e79-169">String</span><span class="sxs-lookup"><span data-stu-id="45e79-169">String</span></span>|<span data-ttu-id="45e79-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="45e79-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="45e79-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45e79-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45e79-172">displayName</span><span class="sxs-lookup"><span data-stu-id="45e79-172">displayName</span></span>|<span data-ttu-id="45e79-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="45e79-173">String</span></span>|<span data-ttu-id="45e79-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="45e79-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="45e79-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45e79-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45e79-176">versão</span><span class="sxs-lookup"><span data-stu-id="45e79-176">version</span></span>|<span data-ttu-id="45e79-177">Int32</span><span class="sxs-lookup"><span data-stu-id="45e79-177">Int32</span></span>|<span data-ttu-id="45e79-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="45e79-178">Version of the device configuration.</span></span> <span data-ttu-id="45e79-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45e79-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45e79-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="45e79-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="45e79-181">Int32</span><span class="sxs-lookup"><span data-stu-id="45e79-181">Int32</span></span>|<span data-ttu-id="45e79-182">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="45e79-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="45e79-183">Valores válidos de 1 a 99 herdados de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="45e79-183">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="45e79-184">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="45e79-184">keyStorageProvider</span></span>|[<span data-ttu-id="45e79-185">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="45e79-185">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="45e79-186">Provedor de armazenamento de chave (KSP) herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="45e79-186">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="45e79-187">Os valores possíveis são: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="45e79-187">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="45e79-188">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="45e79-188">subjectNameFormat</span></span>|[<span data-ttu-id="45e79-189">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="45e79-189">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="45e79-190">Formato do nome de entidade do certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="45e79-190">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="45e79-191">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="45e79-191">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="45e79-192">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="45e79-192">subjectAlternativeNameType</span></span>|[<span data-ttu-id="45e79-193">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="45e79-193">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="45e79-194">Tipo de nome alternativo de entidade do certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="45e79-194">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="45e79-195">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="45e79-195">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="45e79-196">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="45e79-196">certificateValidityPeriodValue</span></span>|<span data-ttu-id="45e79-197">Int32</span><span class="sxs-lookup"><span data-stu-id="45e79-197">Int32</span></span>|<span data-ttu-id="45e79-198">Valor para o período de validade do certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="45e79-198">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="45e79-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="45e79-199">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="45e79-200">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="45e79-200">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="45e79-201">Dimensionar o período de validade do certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="45e79-201">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="45e79-202">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="45e79-202">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="45e79-203">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="45e79-203">certificationAuthority</span></span>|<span data-ttu-id="45e79-204">String</span><span class="sxs-lookup"><span data-stu-id="45e79-204">String</span></span>|<span data-ttu-id="45e79-205">Autoridade de certificação PKCS</span><span class="sxs-lookup"><span data-stu-id="45e79-205">PKCS Certification Authority</span></span>|
|<span data-ttu-id="45e79-206">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="45e79-206">certificationAuthorityName</span></span>|<span data-ttu-id="45e79-207">String</span><span class="sxs-lookup"><span data-stu-id="45e79-207">String</span></span>|<span data-ttu-id="45e79-208">Nome da autoridade de certificação PKCS</span><span class="sxs-lookup"><span data-stu-id="45e79-208">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="45e79-209">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="45e79-209">certificateTemplateName</span></span>|<span data-ttu-id="45e79-210">String</span><span class="sxs-lookup"><span data-stu-id="45e79-210">String</span></span>|<span data-ttu-id="45e79-211">Nome do modelo de certificado PKCS</span><span class="sxs-lookup"><span data-stu-id="45e79-211">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="45e79-212">Subjectalternativenameformatstring foi</span><span class="sxs-lookup"><span data-stu-id="45e79-212">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="45e79-213">String</span><span class="sxs-lookup"><span data-stu-id="45e79-213">String</span></span>|<span data-ttu-id="45e79-214">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="45e79-214">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="45e79-215">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="45e79-215">extendedKeyUsages</span></span>|<span data-ttu-id="45e79-216">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="45e79-216">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="45e79-217">Configurações de EKU (uso estendido de chave).</span><span class="sxs-lookup"><span data-stu-id="45e79-217">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="45e79-218">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="45e79-218">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="45e79-219">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="45e79-219">subjectNameFormatString</span></span>|<span data-ttu-id="45e79-220">String</span><span class="sxs-lookup"><span data-stu-id="45e79-220">String</span></span>|<span data-ttu-id="45e79-221">Formato personalizado a ser usado com SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="45e79-221">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="45e79-222">Exemplo: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = usuários corporativos, O = Contoso Corporation, L = Redmond, ST = WA, C = br</span><span class="sxs-lookup"><span data-stu-id="45e79-222">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="45e79-223">certificateStore</span><span class="sxs-lookup"><span data-stu-id="45e79-223">certificateStore</span></span>|[<span data-ttu-id="45e79-224">certificateStore</span><span class="sxs-lookup"><span data-stu-id="45e79-224">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="45e79-225">Certificado de repositório de destino.</span><span class="sxs-lookup"><span data-stu-id="45e79-225">Target store certificate.</span></span> <span data-ttu-id="45e79-226">Os valores possíveis são: `user` e `machine`.</span><span class="sxs-lookup"><span data-stu-id="45e79-226">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="45e79-227">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="45e79-227">customSubjectAlternativeNames</span></span>|<span data-ttu-id="45e79-228">coleção [customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="45e79-228">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="45e79-229">Configurações de nome alternativo de entidade personalizada.</span><span class="sxs-lookup"><span data-stu-id="45e79-229">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="45e79-230">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="45e79-230">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="45e79-231">Resposta</span><span class="sxs-lookup"><span data-stu-id="45e79-231">Response</span></span>
<span data-ttu-id="45e79-232">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="45e79-232">If successful, this method returns a `200 OK` response code and an updated [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45e79-233">Exemplo</span><span class="sxs-lookup"><span data-stu-id="45e79-233">Example</span></span>

### <a name="request"></a><span data-ttu-id="45e79-234">Solicitação</span><span class="sxs-lookup"><span data-stu-id="45e79-234">Request</span></span>
<span data-ttu-id="45e79-235">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="45e79-235">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2074

{
  "@odata.type": "#microsoft.graph.windows10PkcsCertificateProfile",
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
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
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

### <a name="response"></a><span data-ttu-id="45e79-236">Resposta</span><span class="sxs-lookup"><span data-stu-id="45e79-236">Response</span></span>
<span data-ttu-id="45e79-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="45e79-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2246

{
  "@odata.type": "#microsoft.graph.windows10PkcsCertificateProfile",
  "id": "414c69c0-69c0-414c-c069-4c41c0694c41",
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
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
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





