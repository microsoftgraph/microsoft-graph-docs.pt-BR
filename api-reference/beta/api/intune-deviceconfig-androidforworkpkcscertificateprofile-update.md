---
title: Atualizar androidForWorkPkcsCertificateProfile
description: Atualize as propriedades de um objeto androidForWorkPkcsCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a95baf5d2d715c79a65fa77ccef57077b4d98390
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51138369"
---
# <a name="update-androidforworkpkcscertificateprofile"></a><span data-ttu-id="17c1c-103">Atualizar androidForWorkPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="17c1c-103">Update androidForWorkPkcsCertificateProfile</span></span>

<span data-ttu-id="17c1c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="17c1c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="17c1c-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="17c1c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="17c1c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="17c1c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="17c1c-107">Atualize as propriedades de [um objeto androidForWorkPkcsCertificateProfile.](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="17c1c-107">Update the properties of a [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="17c1c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="17c1c-108">Prerequisites</span></span>
<span data-ttu-id="17c1c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17c1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17c1c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="17c1c-111">Permission type</span></span>|<span data-ttu-id="17c1c-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="17c1c-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="17c1c-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="17c1c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="17c1c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17c1c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="17c1c-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="17c1c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="17c1c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="17c1c-116">Not supported.</span></span>|
|<span data-ttu-id="17c1c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="17c1c-117">Application</span></span>|<span data-ttu-id="17c1c-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17c1c-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="17c1c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="17c1c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="17c1c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="17c1c-120">Request headers</span></span>
|<span data-ttu-id="17c1c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="17c1c-121">Header</span></span>|<span data-ttu-id="17c1c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="17c1c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="17c1c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="17c1c-123">Authorization</span></span>|<span data-ttu-id="17c1c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="17c1c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="17c1c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="17c1c-125">Accept</span></span>|<span data-ttu-id="17c1c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="17c1c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="17c1c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="17c1c-127">Request body</span></span>
<span data-ttu-id="17c1c-128">No corpo da solicitação, fornece uma representação JSON para o [objeto androidForWorkPkcsCertificateProfile.](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="17c1c-128">In the request body, supply a JSON representation for the [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) object.</span></span>

<span data-ttu-id="17c1c-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="17c1c-129">The following table shows the properties that are required when you create the [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md).</span></span>

|<span data-ttu-id="17c1c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="17c1c-130">Property</span></span>|<span data-ttu-id="17c1c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="17c1c-131">Type</span></span>|<span data-ttu-id="17c1c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="17c1c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17c1c-133">id</span><span class="sxs-lookup"><span data-stu-id="17c1c-133">id</span></span>|<span data-ttu-id="17c1c-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="17c1c-134">String</span></span>|<span data-ttu-id="17c1c-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="17c1c-135">Key of the entity.</span></span> <span data-ttu-id="17c1c-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="17c1c-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17c1c-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="17c1c-137">lastModifiedDateTime</span></span>|<span data-ttu-id="17c1c-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17c1c-138">DateTimeOffset</span></span>|<span data-ttu-id="17c1c-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="17c1c-139">DateTime the object was last modified.</span></span> <span data-ttu-id="17c1c-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="17c1c-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17c1c-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="17c1c-141">roleScopeTagIds</span></span>|<span data-ttu-id="17c1c-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="17c1c-142">String collection</span></span>|<span data-ttu-id="17c1c-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="17c1c-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="17c1c-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="17c1c-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17c1c-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="17c1c-145">supportsScopeTags</span></span>|<span data-ttu-id="17c1c-146">Booleano</span><span class="sxs-lookup"><span data-stu-id="17c1c-146">Boolean</span></span>|<span data-ttu-id="17c1c-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="17c1c-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="17c1c-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="17c1c-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="17c1c-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="17c1c-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="17c1c-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="17c1c-150">This property is read-only.</span></span> <span data-ttu-id="17c1c-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="17c1c-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17c1c-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="17c1c-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="17c1c-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="17c1c-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="17c1c-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="17c1c-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="17c1c-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="17c1c-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17c1c-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="17c1c-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="17c1c-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="17c1c-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="17c1c-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="17c1c-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="17c1c-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="17c1c-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17c1c-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="17c1c-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="17c1c-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="17c1c-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="17c1c-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="17c1c-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="17c1c-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="17c1c-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17c1c-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="17c1c-164">createdDateTime</span></span>|<span data-ttu-id="17c1c-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17c1c-165">DateTimeOffset</span></span>|<span data-ttu-id="17c1c-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="17c1c-166">DateTime the object was created.</span></span> <span data-ttu-id="17c1c-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="17c1c-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17c1c-168">descrição</span><span class="sxs-lookup"><span data-stu-id="17c1c-168">description</span></span>|<span data-ttu-id="17c1c-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="17c1c-169">String</span></span>|<span data-ttu-id="17c1c-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="17c1c-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="17c1c-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="17c1c-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17c1c-172">displayName</span><span class="sxs-lookup"><span data-stu-id="17c1c-172">displayName</span></span>|<span data-ttu-id="17c1c-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="17c1c-173">String</span></span>|<span data-ttu-id="17c1c-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="17c1c-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="17c1c-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="17c1c-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17c1c-176">versão</span><span class="sxs-lookup"><span data-stu-id="17c1c-176">version</span></span>|<span data-ttu-id="17c1c-177">Int32</span><span class="sxs-lookup"><span data-stu-id="17c1c-177">Int32</span></span>|<span data-ttu-id="17c1c-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="17c1c-178">Version of the device configuration.</span></span> <span data-ttu-id="17c1c-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="17c1c-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="17c1c-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="17c1c-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="17c1c-181">Int32</span><span class="sxs-lookup"><span data-stu-id="17c1c-181">Int32</span></span>|<span data-ttu-id="17c1c-182">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="17c1c-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="17c1c-183">Valores válidos de 1 a 99 Herdados [de androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="17c1c-183">Valid values 1 to 99 Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="17c1c-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="17c1c-184">subjectNameFormat</span></span>|[<span data-ttu-id="17c1c-185">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="17c1c-185">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="17c1c-186">Formato de Nome do Assunto do Certificado.</span><span class="sxs-lookup"><span data-stu-id="17c1c-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="17c1c-187">Herdado [de androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="17c1c-187">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="17c1c-188">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="17c1c-188">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="17c1c-189">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="17c1c-189">certificateValidityPeriodValue</span></span>|<span data-ttu-id="17c1c-190">Int32</span><span class="sxs-lookup"><span data-stu-id="17c1c-190">Int32</span></span>|<span data-ttu-id="17c1c-191">Valor do Período de Validade do Certificado.</span><span class="sxs-lookup"><span data-stu-id="17c1c-191">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="17c1c-192">Herdado [de androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="17c1c-192">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="17c1c-193">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="17c1c-193">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="17c1c-194">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="17c1c-194">certificateValidityPeriodScale</span></span>](../resources/intune-shared-certificatevalidityperiodscale.md)|<span data-ttu-id="17c1c-195">Dimensione para o Período de Validade do Certificado.</span><span class="sxs-lookup"><span data-stu-id="17c1c-195">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="17c1c-196">Herdado [de androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="17c1c-196">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="17c1c-197">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="17c1c-197">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="17c1c-198">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="17c1c-198">extendedKeyUsages</span></span>|<span data-ttu-id="17c1c-199">[Coleção extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="17c1c-199">[extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="17c1c-200">Configurações de Uso de Chave Estendida (EKU).</span><span class="sxs-lookup"><span data-stu-id="17c1c-200">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="17c1c-201">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="17c1c-201">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="17c1c-202">Herdado [de androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="17c1c-202">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="17c1c-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="17c1c-203">subjectAlternativeNameType</span></span>|[<span data-ttu-id="17c1c-204">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="17c1c-204">subjectAlternativeNameType</span></span>](../resources/intune-shared-subjectalternativenametype.md)|<span data-ttu-id="17c1c-205">Tipo de nome alternativo do assunto do certificado.</span><span class="sxs-lookup"><span data-stu-id="17c1c-205">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="17c1c-206">Herdado [de androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="17c1c-206">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="17c1c-207">Os possíveis valores são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span><span class="sxs-lookup"><span data-stu-id="17c1c-207">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span></span>|
|<span data-ttu-id="17c1c-208">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="17c1c-208">certificationAuthority</span></span>|<span data-ttu-id="17c1c-209">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="17c1c-209">String</span></span>|<span data-ttu-id="17c1c-210">Autoridade de Certificação PKCS</span><span class="sxs-lookup"><span data-stu-id="17c1c-210">PKCS Certification Authority</span></span>|
|<span data-ttu-id="17c1c-211">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="17c1c-211">certificationAuthorityName</span></span>|<span data-ttu-id="17c1c-212">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="17c1c-212">String</span></span>|<span data-ttu-id="17c1c-213">Nome da autoridade de certificação PKCS</span><span class="sxs-lookup"><span data-stu-id="17c1c-213">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="17c1c-214">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="17c1c-214">certificateTemplateName</span></span>|<span data-ttu-id="17c1c-215">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="17c1c-215">String</span></span>|<span data-ttu-id="17c1c-216">Nome do modelo de certificado PKCS</span><span class="sxs-lookup"><span data-stu-id="17c1c-216">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="17c1c-217">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="17c1c-217">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="17c1c-218">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="17c1c-218">String</span></span>|<span data-ttu-id="17c1c-219">Cadeia de caracteres personalizada que define o Atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="17c1c-219">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="17c1c-220">Resposta</span><span class="sxs-lookup"><span data-stu-id="17c1c-220">Response</span></span>
<span data-ttu-id="17c1c-221">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="17c1c-221">If successful, this method returns a `200 OK` response code and an updated [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17c1c-222">Exemplo</span><span class="sxs-lookup"><span data-stu-id="17c1c-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="17c1c-223">Solicitação</span><span class="sxs-lookup"><span data-stu-id="17c1c-223">Request</span></span>
<span data-ttu-id="17c1c-224">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="17c1c-224">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="17c1c-225">Resposta</span><span class="sxs-lookup"><span data-stu-id="17c1c-225">Response</span></span>
<span data-ttu-id="17c1c-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="17c1c-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




