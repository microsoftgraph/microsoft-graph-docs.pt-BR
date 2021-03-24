---
title: Criar androidForWorkPkcsCertificateProfile
description: Crie um novo objeto androidForWorkPkcsCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f95f36d6eed71e7b38bdff3e443e71ed3533f607
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51142594"
---
# <a name="create-androidforworkpkcscertificateprofile"></a><span data-ttu-id="d87dd-103">Criar androidForWorkPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="d87dd-103">Create androidForWorkPkcsCertificateProfile</span></span>

<span data-ttu-id="d87dd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d87dd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d87dd-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d87dd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d87dd-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d87dd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d87dd-107">Crie um novo [objeto androidForWorkPkcsCertificateProfile.](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d87dd-107">Create a new [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d87dd-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d87dd-108">Prerequisites</span></span>
<span data-ttu-id="d87dd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d87dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d87dd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d87dd-111">Permission type</span></span>|<span data-ttu-id="d87dd-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d87dd-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d87dd-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d87dd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d87dd-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d87dd-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d87dd-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d87dd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d87dd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d87dd-116">Not supported.</span></span>|
|<span data-ttu-id="d87dd-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d87dd-117">Application</span></span>|<span data-ttu-id="d87dd-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d87dd-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d87dd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d87dd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d87dd-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d87dd-120">Request headers</span></span>
|<span data-ttu-id="d87dd-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d87dd-121">Header</span></span>|<span data-ttu-id="d87dd-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d87dd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d87dd-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d87dd-123">Authorization</span></span>|<span data-ttu-id="d87dd-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d87dd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d87dd-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d87dd-125">Accept</span></span>|<span data-ttu-id="d87dd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d87dd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d87dd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d87dd-127">Request body</span></span>
<span data-ttu-id="d87dd-128">No corpo da solicitação, fornece uma representação JSON para o objeto androidForWorkPkcsCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="d87dd-128">In the request body, supply a JSON representation for the androidForWorkPkcsCertificateProfile object.</span></span>

<span data-ttu-id="d87dd-129">A tabela a seguir mostra as propriedades necessárias ao criar o androidForWorkPkcsCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="d87dd-129">The following table shows the properties that are required when you create the androidForWorkPkcsCertificateProfile.</span></span>

|<span data-ttu-id="d87dd-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d87dd-130">Property</span></span>|<span data-ttu-id="d87dd-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d87dd-131">Type</span></span>|<span data-ttu-id="d87dd-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d87dd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d87dd-133">id</span><span class="sxs-lookup"><span data-stu-id="d87dd-133">id</span></span>|<span data-ttu-id="d87dd-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d87dd-134">String</span></span>|<span data-ttu-id="d87dd-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d87dd-135">Key of the entity.</span></span> <span data-ttu-id="d87dd-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d87dd-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d87dd-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d87dd-137">lastModifiedDateTime</span></span>|<span data-ttu-id="d87dd-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d87dd-138">DateTimeOffset</span></span>|<span data-ttu-id="d87dd-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="d87dd-139">DateTime the object was last modified.</span></span> <span data-ttu-id="d87dd-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d87dd-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d87dd-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d87dd-141">roleScopeTagIds</span></span>|<span data-ttu-id="d87dd-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d87dd-142">String collection</span></span>|<span data-ttu-id="d87dd-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="d87dd-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d87dd-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d87dd-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d87dd-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d87dd-145">supportsScopeTags</span></span>|<span data-ttu-id="d87dd-146">Booleano</span><span class="sxs-lookup"><span data-stu-id="d87dd-146">Boolean</span></span>|<span data-ttu-id="d87dd-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="d87dd-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d87dd-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="d87dd-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d87dd-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="d87dd-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d87dd-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d87dd-150">This property is read-only.</span></span> <span data-ttu-id="d87dd-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d87dd-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d87dd-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d87dd-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="d87dd-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d87dd-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="d87dd-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="d87dd-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="d87dd-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d87dd-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d87dd-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d87dd-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="d87dd-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d87dd-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="d87dd-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="d87dd-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="d87dd-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d87dd-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d87dd-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d87dd-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="d87dd-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d87dd-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="d87dd-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="d87dd-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="d87dd-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d87dd-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d87dd-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d87dd-164">createdDateTime</span></span>|<span data-ttu-id="d87dd-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d87dd-165">DateTimeOffset</span></span>|<span data-ttu-id="d87dd-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="d87dd-166">DateTime the object was created.</span></span> <span data-ttu-id="d87dd-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d87dd-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d87dd-168">descrição</span><span class="sxs-lookup"><span data-stu-id="d87dd-168">description</span></span>|<span data-ttu-id="d87dd-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d87dd-169">String</span></span>|<span data-ttu-id="d87dd-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d87dd-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d87dd-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d87dd-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d87dd-172">displayName</span><span class="sxs-lookup"><span data-stu-id="d87dd-172">displayName</span></span>|<span data-ttu-id="d87dd-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d87dd-173">String</span></span>|<span data-ttu-id="d87dd-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d87dd-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d87dd-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d87dd-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d87dd-176">versão</span><span class="sxs-lookup"><span data-stu-id="d87dd-176">version</span></span>|<span data-ttu-id="d87dd-177">Int32</span><span class="sxs-lookup"><span data-stu-id="d87dd-177">Int32</span></span>|<span data-ttu-id="d87dd-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d87dd-178">Version of the device configuration.</span></span> <span data-ttu-id="d87dd-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d87dd-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d87dd-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="d87dd-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="d87dd-181">Int32</span><span class="sxs-lookup"><span data-stu-id="d87dd-181">Int32</span></span>|<span data-ttu-id="d87dd-182">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="d87dd-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="d87dd-183">Valores válidos de 1 a 99 Herdados [de androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="d87dd-183">Valid values 1 to 99 Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="d87dd-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="d87dd-184">subjectNameFormat</span></span>|[<span data-ttu-id="d87dd-185">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="d87dd-185">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="d87dd-186">Formato de Nome do Assunto do Certificado.</span><span class="sxs-lookup"><span data-stu-id="d87dd-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="d87dd-187">Herdado [de androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="d87dd-187">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="d87dd-188">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="d87dd-188">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="d87dd-189">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="d87dd-189">certificateValidityPeriodValue</span></span>|<span data-ttu-id="d87dd-190">Int32</span><span class="sxs-lookup"><span data-stu-id="d87dd-190">Int32</span></span>|<span data-ttu-id="d87dd-191">Valor do Período de Validade do Certificado.</span><span class="sxs-lookup"><span data-stu-id="d87dd-191">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="d87dd-192">Herdado [de androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="d87dd-192">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="d87dd-193">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="d87dd-193">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="d87dd-194">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="d87dd-194">certificateValidityPeriodScale</span></span>](../resources/intune-shared-certificatevalidityperiodscale.md)|<span data-ttu-id="d87dd-195">Dimensione para o Período de Validade do Certificado.</span><span class="sxs-lookup"><span data-stu-id="d87dd-195">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="d87dd-196">Herdado [de androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="d87dd-196">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="d87dd-197">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="d87dd-197">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="d87dd-198">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="d87dd-198">extendedKeyUsages</span></span>|<span data-ttu-id="d87dd-199">[Coleção extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="d87dd-199">[extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="d87dd-200">Configurações de Uso de Chave Estendida (EKU).</span><span class="sxs-lookup"><span data-stu-id="d87dd-200">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="d87dd-201">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="d87dd-201">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="d87dd-202">Herdado [de androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="d87dd-202">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="d87dd-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="d87dd-203">subjectAlternativeNameType</span></span>|[<span data-ttu-id="d87dd-204">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="d87dd-204">subjectAlternativeNameType</span></span>](../resources/intune-shared-subjectalternativenametype.md)|<span data-ttu-id="d87dd-205">Tipo de nome alternativo do assunto do certificado.</span><span class="sxs-lookup"><span data-stu-id="d87dd-205">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="d87dd-206">Herdado [de androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="d87dd-206">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="d87dd-207">Os possíveis valores são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span><span class="sxs-lookup"><span data-stu-id="d87dd-207">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span></span>|
|<span data-ttu-id="d87dd-208">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="d87dd-208">certificationAuthority</span></span>|<span data-ttu-id="d87dd-209">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d87dd-209">String</span></span>|<span data-ttu-id="d87dd-210">Autoridade de Certificação PKCS</span><span class="sxs-lookup"><span data-stu-id="d87dd-210">PKCS Certification Authority</span></span>|
|<span data-ttu-id="d87dd-211">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="d87dd-211">certificationAuthorityName</span></span>|<span data-ttu-id="d87dd-212">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d87dd-212">String</span></span>|<span data-ttu-id="d87dd-213">Nome da autoridade de certificação PKCS</span><span class="sxs-lookup"><span data-stu-id="d87dd-213">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="d87dd-214">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="d87dd-214">certificateTemplateName</span></span>|<span data-ttu-id="d87dd-215">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d87dd-215">String</span></span>|<span data-ttu-id="d87dd-216">Nome do modelo de certificado PKCS</span><span class="sxs-lookup"><span data-stu-id="d87dd-216">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="d87dd-217">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="d87dd-217">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="d87dd-218">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d87dd-218">String</span></span>|<span data-ttu-id="d87dd-219">Cadeia de caracteres personalizada que define o Atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="d87dd-219">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="d87dd-220">Resposta</span><span class="sxs-lookup"><span data-stu-id="d87dd-220">Response</span></span>
<span data-ttu-id="d87dd-221">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d87dd-221">If successful, this method returns a `201 Created` response code and a [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d87dd-222">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d87dd-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="d87dd-223">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d87dd-223">Request</span></span>
<span data-ttu-id="d87dd-224">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d87dd-224">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="d87dd-225">Resposta</span><span class="sxs-lookup"><span data-stu-id="d87dd-225">Response</span></span>
<span data-ttu-id="d87dd-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d87dd-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




