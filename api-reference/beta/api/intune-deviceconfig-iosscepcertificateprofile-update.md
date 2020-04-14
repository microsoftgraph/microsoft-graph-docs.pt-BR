---
title: Atualizar iosScepCertificateProfile
description: Atualiza as propriedades de um objeto iosScepCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c19703d5e77d48baef8b79f258036df38bce32a7
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43438716"
---
# <a name="update-iosscepcertificateprofile"></a><span data-ttu-id="5dcf3-103">Atualizar iosScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="5dcf3-103">Update iosScepCertificateProfile</span></span>

<span data-ttu-id="5dcf3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5dcf3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5dcf3-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5dcf3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5dcf3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5dcf3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5dcf3-107">Atualiza as propriedades de um objeto [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="5dcf3-107">Update the properties of a [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5dcf3-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5dcf3-108">Prerequisites</span></span>
<span data-ttu-id="5dcf3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5dcf3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5dcf3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5dcf3-111">Permission type</span></span>|<span data-ttu-id="5dcf3-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5dcf3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5dcf3-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5dcf3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5dcf3-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5dcf3-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5dcf3-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5dcf3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5dcf3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5dcf3-116">Not supported.</span></span>|
|<span data-ttu-id="5dcf3-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5dcf3-117">Application</span></span>|<span data-ttu-id="5dcf3-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5dcf3-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5dcf3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5dcf3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="5dcf3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5dcf3-120">Request headers</span></span>
|<span data-ttu-id="5dcf3-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5dcf3-121">Header</span></span>|<span data-ttu-id="5dcf3-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5dcf3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5dcf3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5dcf3-123">Authorization</span></span>|<span data-ttu-id="5dcf3-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5dcf3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5dcf3-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5dcf3-125">Accept</span></span>|<span data-ttu-id="5dcf3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5dcf3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5dcf3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5dcf3-127">Request body</span></span>
<span data-ttu-id="5dcf3-128">No corpo da solicitação, forneça uma representação JSON do objeto [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="5dcf3-128">In the request body, supply a JSON representation for the [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object.</span></span>

<span data-ttu-id="5dcf3-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="5dcf3-129">The following table shows the properties that are required when you create the [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md).</span></span>

|<span data-ttu-id="5dcf3-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5dcf3-130">Property</span></span>|<span data-ttu-id="5dcf3-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="5dcf3-131">Type</span></span>|<span data-ttu-id="5dcf3-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="5dcf3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5dcf3-133">id</span><span class="sxs-lookup"><span data-stu-id="5dcf3-133">id</span></span>|<span data-ttu-id="5dcf3-134">String</span><span class="sxs-lookup"><span data-stu-id="5dcf3-134">String</span></span>|<span data-ttu-id="5dcf3-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="5dcf3-135">Key of the entity.</span></span> <span data-ttu-id="5dcf3-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5dcf3-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5dcf3-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5dcf3-137">lastModifiedDateTime</span></span>|<span data-ttu-id="5dcf3-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5dcf3-138">DateTimeOffset</span></span>|<span data-ttu-id="5dcf3-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="5dcf3-139">DateTime the object was last modified.</span></span> <span data-ttu-id="5dcf3-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5dcf3-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5dcf3-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5dcf3-141">roleScopeTagIds</span></span>|<span data-ttu-id="5dcf3-142">Coleção String</span><span class="sxs-lookup"><span data-stu-id="5dcf3-142">String collection</span></span>|<span data-ttu-id="5dcf3-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="5dcf3-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="5dcf3-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5dcf3-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5dcf3-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="5dcf3-145">supportsScopeTags</span></span>|<span data-ttu-id="5dcf3-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="5dcf3-146">Boolean</span></span>|<span data-ttu-id="5dcf3-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="5dcf3-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="5dcf3-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="5dcf3-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="5dcf3-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="5dcf3-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="5dcf3-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5dcf3-150">This property is read-only.</span></span> <span data-ttu-id="5dcf3-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5dcf3-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5dcf3-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="5dcf3-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="5dcf3-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="5dcf3-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="5dcf3-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="5dcf3-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="5dcf3-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5dcf3-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5dcf3-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="5dcf3-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="5dcf3-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="5dcf3-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="5dcf3-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="5dcf3-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="5dcf3-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5dcf3-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5dcf3-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="5dcf3-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="5dcf3-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="5dcf3-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="5dcf3-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="5dcf3-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="5dcf3-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5dcf3-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5dcf3-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5dcf3-164">createdDateTime</span></span>|<span data-ttu-id="5dcf3-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5dcf3-165">DateTimeOffset</span></span>|<span data-ttu-id="5dcf3-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="5dcf3-166">DateTime the object was created.</span></span> <span data-ttu-id="5dcf3-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5dcf3-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5dcf3-168">description</span><span class="sxs-lookup"><span data-stu-id="5dcf3-168">description</span></span>|<span data-ttu-id="5dcf3-169">String</span><span class="sxs-lookup"><span data-stu-id="5dcf3-169">String</span></span>|<span data-ttu-id="5dcf3-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5dcf3-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5dcf3-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5dcf3-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5dcf3-172">displayName</span><span class="sxs-lookup"><span data-stu-id="5dcf3-172">displayName</span></span>|<span data-ttu-id="5dcf3-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5dcf3-173">String</span></span>|<span data-ttu-id="5dcf3-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5dcf3-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5dcf3-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5dcf3-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5dcf3-176">versão</span><span class="sxs-lookup"><span data-stu-id="5dcf3-176">version</span></span>|<span data-ttu-id="5dcf3-177">Int32</span><span class="sxs-lookup"><span data-stu-id="5dcf3-177">Int32</span></span>|<span data-ttu-id="5dcf3-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5dcf3-178">Version of the device configuration.</span></span> <span data-ttu-id="5dcf3-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5dcf3-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5dcf3-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="5dcf3-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="5dcf3-181">Int32</span><span class="sxs-lookup"><span data-stu-id="5dcf3-181">Int32</span></span>|<span data-ttu-id="5dcf3-182">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="5dcf3-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="5dcf3-183">Valores válidos de 1 a 99 herdados de [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="5dcf3-183">Valid values 1 to 99 Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="5dcf3-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="5dcf3-184">subjectNameFormat</span></span>|[<span data-ttu-id="5dcf3-185">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="5dcf3-185">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="5dcf3-186">Formato do nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="5dcf3-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="5dcf3-187">Herdado de [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="5dcf3-187">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="5dcf3-188">Os possíveis valores são: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="5dcf3-188">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="5dcf3-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="5dcf3-189">subjectAlternativeNameType</span></span>|[<span data-ttu-id="5dcf3-190">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="5dcf3-190">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="5dcf3-191">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="5dcf3-191">Certificate Subject Alternative Name type.</span></span> <span data-ttu-id="5dcf3-192">Herdado de [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="5dcf3-192">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="5dcf3-193">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="5dcf3-193">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="5dcf3-194">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="5dcf3-194">certificateValidityPeriodValue</span></span>|<span data-ttu-id="5dcf3-195">Int32</span><span class="sxs-lookup"><span data-stu-id="5dcf3-195">Int32</span></span>|<span data-ttu-id="5dcf3-196">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="5dcf3-196">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="5dcf3-197">Herdado de [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="5dcf3-197">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="5dcf3-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="5dcf3-198">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="5dcf3-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="5dcf3-199">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="5dcf3-200">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="5dcf3-200">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="5dcf3-201">Herdado de [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="5dcf3-201">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="5dcf3-202">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="5dcf3-202">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="5dcf3-203">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="5dcf3-203">scepServerUrls</span></span>|<span data-ttu-id="5dcf3-204">Coleção String</span><span class="sxs-lookup"><span data-stu-id="5dcf3-204">String collection</span></span>|<span data-ttu-id="5dcf3-205">URL (s) do servidor de SCEP.</span><span class="sxs-lookup"><span data-stu-id="5dcf3-205">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="5dcf3-206">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="5dcf3-206">subjectNameFormatString</span></span>|<span data-ttu-id="5dcf3-207">String</span><span class="sxs-lookup"><span data-stu-id="5dcf3-207">String</span></span>|<span data-ttu-id="5dcf3-208">Formato personalizado a ser usado com SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="5dcf3-208">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="5dcf3-209">Exemplo: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = usuários corporativos, O = Contoso Corporation, L = Redmond, ST = WA, C = br</span><span class="sxs-lookup"><span data-stu-id="5dcf3-209">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="5dcf3-210">uso de</span><span class="sxs-lookup"><span data-stu-id="5dcf3-210">keyUsage</span></span>|[<span data-ttu-id="5dcf3-211">usos de</span><span class="sxs-lookup"><span data-stu-id="5dcf3-211">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="5dcf3-212">Uso da chave do SCEP.</span><span class="sxs-lookup"><span data-stu-id="5dcf3-212">SCEP Key Usage.</span></span> <span data-ttu-id="5dcf3-213">Os valores possíveis são: `keyEncipherment` e `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="5dcf3-213">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="5dcf3-214">keySize</span><span class="sxs-lookup"><span data-stu-id="5dcf3-214">keySize</span></span>|[<span data-ttu-id="5dcf3-215">keySize</span><span class="sxs-lookup"><span data-stu-id="5dcf3-215">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="5dcf3-216">Tamanho da chave SCEP.</span><span class="sxs-lookup"><span data-stu-id="5dcf3-216">SCEP Key Size.</span></span> <span data-ttu-id="5dcf3-217">Os valores possíveis são: `size1024` e `size2048`.</span><span class="sxs-lookup"><span data-stu-id="5dcf3-217">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="5dcf3-218">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="5dcf3-218">extendedKeyUsages</span></span>|<span data-ttu-id="5dcf3-219">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="5dcf3-219">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="5dcf3-220">Configurações de EKU (uso estendido de chave).</span><span class="sxs-lookup"><span data-stu-id="5dcf3-220">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="5dcf3-221">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="5dcf3-221">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="5dcf3-222">Subjectalternativenameformatstring foi</span><span class="sxs-lookup"><span data-stu-id="5dcf3-222">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="5dcf3-223">String</span><span class="sxs-lookup"><span data-stu-id="5dcf3-223">String</span></span>|<span data-ttu-id="5dcf3-224">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="5dcf3-224">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="5dcf3-225">certificateStore</span><span class="sxs-lookup"><span data-stu-id="5dcf3-225">certificateStore</span></span>|[<span data-ttu-id="5dcf3-226">certificateStore</span><span class="sxs-lookup"><span data-stu-id="5dcf3-226">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="5dcf3-227">Certificado de repositório de destino.</span><span class="sxs-lookup"><span data-stu-id="5dcf3-227">Target store certificate.</span></span> <span data-ttu-id="5dcf3-228">Os valores possíveis são: `user` e `machine`.</span><span class="sxs-lookup"><span data-stu-id="5dcf3-228">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="5dcf3-229">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="5dcf3-229">customSubjectAlternativeNames</span></span>|<span data-ttu-id="5dcf3-230">coleção [customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="5dcf3-230">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="5dcf3-231">Configurações de nome alternativo de entidade personalizada.</span><span class="sxs-lookup"><span data-stu-id="5dcf3-231">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="5dcf3-232">A variável Onpremisesuserprincipalname à é compatível, bem como outras documentadas aqui https://go.microsoft.com/fwlink/?LinkId=2027630:.</span><span class="sxs-lookup"><span data-stu-id="5dcf3-232">The OnPremisesUserPrincipalName variable is support as well as others documented here: https://go.microsoft.com/fwlink/?LinkId=2027630.</span></span> <span data-ttu-id="5dcf3-233">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="5dcf3-233">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="5dcf3-234">Resposta</span><span class="sxs-lookup"><span data-stu-id="5dcf3-234">Response</span></span>
<span data-ttu-id="5dcf3-235">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5dcf3-235">If successful, this method returns a `200 OK` response code and an updated [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5dcf3-236">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5dcf3-236">Example</span></span>

### <a name="request"></a><span data-ttu-id="5dcf3-237">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5dcf3-237">Request</span></span>
<span data-ttu-id="5dcf3-238">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5dcf3-238">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1932

{
  "@odata.type": "#microsoft.graph.iosScepCertificateProfile",
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
  "subjectNameFormat": "commonNameAsEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
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

### <a name="response"></a><span data-ttu-id="5dcf3-239">Resposta</span><span class="sxs-lookup"><span data-stu-id="5dcf3-239">Response</span></span>
<span data-ttu-id="5dcf3-p124">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5dcf3-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2104

{
  "@odata.type": "#microsoft.graph.iosScepCertificateProfile",
  "id": "0deb8dbf-8dbf-0deb-bf8d-eb0dbf8deb0d",
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
  "subjectNameFormat": "commonNameAsEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
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



