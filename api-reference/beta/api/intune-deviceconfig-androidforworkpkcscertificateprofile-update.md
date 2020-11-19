---
title: Atualizar androidForWorkPkcsCertificateProfile
description: Atualiza as propriedades de um objeto androidForWorkPkcsCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7035f2091c1dbaf66c644c284a27a722de523f67
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49238462"
---
# <a name="update-androidforworkpkcscertificateprofile"></a><span data-ttu-id="6f84e-103">Atualizar androidForWorkPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="6f84e-103">Update androidForWorkPkcsCertificateProfile</span></span>

<span data-ttu-id="6f84e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f84e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6f84e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6f84e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6f84e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6f84e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6f84e-107">Atualiza as propriedades de um objeto [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="6f84e-107">Update the properties of a [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6f84e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6f84e-108">Prerequisites</span></span>
<span data-ttu-id="6f84e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f84e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f84e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6f84e-111">Permission type</span></span>|<span data-ttu-id="6f84e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6f84e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f84e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6f84e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6f84e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f84e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6f84e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6f84e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f84e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6f84e-116">Not supported.</span></span>|
|<span data-ttu-id="6f84e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6f84e-117">Application</span></span>|<span data-ttu-id="6f84e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f84e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f84e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6f84e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="6f84e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6f84e-120">Request headers</span></span>
|<span data-ttu-id="6f84e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6f84e-121">Header</span></span>|<span data-ttu-id="6f84e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6f84e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6f84e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6f84e-123">Authorization</span></span>|<span data-ttu-id="6f84e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6f84e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6f84e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6f84e-125">Accept</span></span>|<span data-ttu-id="6f84e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6f84e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f84e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6f84e-127">Request body</span></span>
<span data-ttu-id="6f84e-128">No corpo da solicitação, forneça uma representação JSON do objeto [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="6f84e-128">In the request body, supply a JSON representation for the [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) object.</span></span>

<span data-ttu-id="6f84e-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="6f84e-129">The following table shows the properties that are required when you create the [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md).</span></span>

|<span data-ttu-id="6f84e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6f84e-130">Property</span></span>|<span data-ttu-id="6f84e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6f84e-131">Type</span></span>|<span data-ttu-id="6f84e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f84e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f84e-133">id</span><span class="sxs-lookup"><span data-stu-id="6f84e-133">id</span></span>|<span data-ttu-id="6f84e-134">String</span><span class="sxs-lookup"><span data-stu-id="6f84e-134">String</span></span>|<span data-ttu-id="6f84e-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6f84e-135">Key of the entity.</span></span> <span data-ttu-id="6f84e-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f84e-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f84e-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6f84e-137">lastModifiedDateTime</span></span>|<span data-ttu-id="6f84e-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f84e-138">DateTimeOffset</span></span>|<span data-ttu-id="6f84e-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="6f84e-139">DateTime the object was last modified.</span></span> <span data-ttu-id="6f84e-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f84e-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f84e-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6f84e-141">roleScopeTagIds</span></span>|<span data-ttu-id="6f84e-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6f84e-142">String collection</span></span>|<span data-ttu-id="6f84e-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="6f84e-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6f84e-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f84e-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f84e-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6f84e-145">supportsScopeTags</span></span>|<span data-ttu-id="6f84e-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="6f84e-146">Boolean</span></span>|<span data-ttu-id="6f84e-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="6f84e-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6f84e-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="6f84e-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6f84e-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="6f84e-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6f84e-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6f84e-150">This property is read-only.</span></span> <span data-ttu-id="6f84e-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f84e-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f84e-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6f84e-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="6f84e-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6f84e-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="6f84e-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="6f84e-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="6f84e-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f84e-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f84e-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6f84e-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="6f84e-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6f84e-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="6f84e-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="6f84e-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="6f84e-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f84e-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f84e-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="6f84e-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="6f84e-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="6f84e-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="6f84e-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="6f84e-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="6f84e-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f84e-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f84e-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6f84e-164">createdDateTime</span></span>|<span data-ttu-id="6f84e-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f84e-165">DateTimeOffset</span></span>|<span data-ttu-id="6f84e-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="6f84e-166">DateTime the object was created.</span></span> <span data-ttu-id="6f84e-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f84e-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f84e-168">description</span><span class="sxs-lookup"><span data-stu-id="6f84e-168">description</span></span>|<span data-ttu-id="6f84e-169">String</span><span class="sxs-lookup"><span data-stu-id="6f84e-169">String</span></span>|<span data-ttu-id="6f84e-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6f84e-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6f84e-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f84e-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f84e-172">displayName</span><span class="sxs-lookup"><span data-stu-id="6f84e-172">displayName</span></span>|<span data-ttu-id="6f84e-173">String</span><span class="sxs-lookup"><span data-stu-id="6f84e-173">String</span></span>|<span data-ttu-id="6f84e-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6f84e-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6f84e-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f84e-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f84e-176">versão</span><span class="sxs-lookup"><span data-stu-id="6f84e-176">version</span></span>|<span data-ttu-id="6f84e-177">Int32</span><span class="sxs-lookup"><span data-stu-id="6f84e-177">Int32</span></span>|<span data-ttu-id="6f84e-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6f84e-178">Version of the device configuration.</span></span> <span data-ttu-id="6f84e-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f84e-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f84e-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="6f84e-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="6f84e-181">Int32</span><span class="sxs-lookup"><span data-stu-id="6f84e-181">Int32</span></span>|<span data-ttu-id="6f84e-182">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="6f84e-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="6f84e-183">Valores válidos de 1 a 99 herdados de [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="6f84e-183">Valid values 1 to 99 Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="6f84e-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="6f84e-184">subjectNameFormat</span></span>|[<span data-ttu-id="6f84e-185">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="6f84e-185">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="6f84e-186">Formato do nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="6f84e-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="6f84e-187">Herdado de [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="6f84e-187">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="6f84e-188">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="6f84e-188">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="6f84e-189">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="6f84e-189">certificateValidityPeriodValue</span></span>|<span data-ttu-id="6f84e-190">Int32</span><span class="sxs-lookup"><span data-stu-id="6f84e-190">Int32</span></span>|<span data-ttu-id="6f84e-191">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="6f84e-191">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="6f84e-192">Herdado de [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="6f84e-192">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="6f84e-193">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="6f84e-193">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="6f84e-194">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="6f84e-194">certificateValidityPeriodScale</span></span>](../resources/intune-shared-certificatevalidityperiodscale.md)|<span data-ttu-id="6f84e-195">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="6f84e-195">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="6f84e-196">Herdado de [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="6f84e-196">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="6f84e-197">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="6f84e-197">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="6f84e-198">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="6f84e-198">extendedKeyUsages</span></span>|<span data-ttu-id="6f84e-199">coleção [extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="6f84e-199">[extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="6f84e-200">Configurações de EKU (uso estendido de chave).</span><span class="sxs-lookup"><span data-stu-id="6f84e-200">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="6f84e-201">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="6f84e-201">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="6f84e-202">Herdado de [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="6f84e-202">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="6f84e-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="6f84e-203">subjectAlternativeNameType</span></span>|[<span data-ttu-id="6f84e-204">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="6f84e-204">subjectAlternativeNameType</span></span>](../resources/intune-shared-subjectalternativenametype.md)|<span data-ttu-id="6f84e-205">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="6f84e-205">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="6f84e-206">Herdado de [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="6f84e-206">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="6f84e-207">Os possíveis valores são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span><span class="sxs-lookup"><span data-stu-id="6f84e-207">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span></span>|
|<span data-ttu-id="6f84e-208">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="6f84e-208">certificationAuthority</span></span>|<span data-ttu-id="6f84e-209">String</span><span class="sxs-lookup"><span data-stu-id="6f84e-209">String</span></span>|<span data-ttu-id="6f84e-210">Autoridade de certificação PKCS</span><span class="sxs-lookup"><span data-stu-id="6f84e-210">PKCS Certification Authority</span></span>|
|<span data-ttu-id="6f84e-211">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="6f84e-211">certificationAuthorityName</span></span>|<span data-ttu-id="6f84e-212">String</span><span class="sxs-lookup"><span data-stu-id="6f84e-212">String</span></span>|<span data-ttu-id="6f84e-213">Nome da autoridade de certificação PKCS</span><span class="sxs-lookup"><span data-stu-id="6f84e-213">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="6f84e-214">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="6f84e-214">certificateTemplateName</span></span>|<span data-ttu-id="6f84e-215">String</span><span class="sxs-lookup"><span data-stu-id="6f84e-215">String</span></span>|<span data-ttu-id="6f84e-216">Nome do modelo de certificado PKCS</span><span class="sxs-lookup"><span data-stu-id="6f84e-216">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="6f84e-217">Subjectalternativenameformatstring foi</span><span class="sxs-lookup"><span data-stu-id="6f84e-217">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="6f84e-218">String</span><span class="sxs-lookup"><span data-stu-id="6f84e-218">String</span></span>|<span data-ttu-id="6f84e-219">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="6f84e-219">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="6f84e-220">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f84e-220">Response</span></span>
<span data-ttu-id="6f84e-221">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6f84e-221">If successful, this method returns a `200 OK` response code and an updated [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f84e-222">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6f84e-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="6f84e-223">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6f84e-223">Request</span></span>
<span data-ttu-id="6f84e-224">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6f84e-224">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6f84e-225">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f84e-225">Response</span></span>
<span data-ttu-id="6f84e-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6f84e-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




