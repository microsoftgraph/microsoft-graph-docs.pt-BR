---
title: Atualizar windows81SCEPCertificateProfile
description: Atualize as propriedades de um objeto windows81SCEPCertificateProfile.
ms.openlocfilehash: 5714179b9e54d32d48dece053f5bb6e7fa8eaee7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036085"
---
# <a name="update-windows81scepcertificateprofile"></a><span data-ttu-id="9d88f-103">Atualizar windows81SCEPCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="9d88f-103">Update windows81SCEPCertificateProfile</span></span>

> <span data-ttu-id="9d88f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9d88f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9d88f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9d88f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9d88f-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="9d88f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9d88f-107">Atualize as propriedades de um objeto [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="9d88f-107">Update the properties of a [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9d88f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9d88f-108">Prerequisites</span></span>
<span data-ttu-id="9d88f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d88f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d88f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9d88f-111">Permission type</span></span>|<span data-ttu-id="9d88f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9d88f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9d88f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9d88f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9d88f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d88f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9d88f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9d88f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9d88f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9d88f-116">Not supported.</span></span>|
|<span data-ttu-id="9d88f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9d88f-117">Application</span></span>|<span data-ttu-id="9d88f-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9d88f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9d88f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9d88f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="9d88f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9d88f-120">Request headers</span></span>
|<span data-ttu-id="9d88f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9d88f-121">Header</span></span>|<span data-ttu-id="9d88f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9d88f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9d88f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9d88f-123">Authorization</span></span>|<span data-ttu-id="9d88f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9d88f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9d88f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9d88f-125">Accept</span></span>|<span data-ttu-id="9d88f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9d88f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d88f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9d88f-127">Request body</span></span>
<span data-ttu-id="9d88f-128">No corpo da solicitação, fornece uma representação JSON para o objeto [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="9d88f-128">In the request body, supply a JSON representation for the [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) object.</span></span>

<span data-ttu-id="9d88f-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="9d88f-129">The following table shows the properties that are required when you create the [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md).</span></span>

|<span data-ttu-id="9d88f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9d88f-130">Property</span></span>|<span data-ttu-id="9d88f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9d88f-131">Type</span></span>|<span data-ttu-id="9d88f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d88f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d88f-133">id</span><span class="sxs-lookup"><span data-stu-id="9d88f-133">id</span></span>|<span data-ttu-id="9d88f-134">String</span><span class="sxs-lookup"><span data-stu-id="9d88f-134">String</span></span>|<span data-ttu-id="9d88f-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9d88f-135">Key of the entity.</span></span> <span data-ttu-id="9d88f-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9d88f-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9d88f-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9d88f-137">lastModifiedDateTime</span></span>|<span data-ttu-id="9d88f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d88f-138">DateTimeOffset</span></span>|<span data-ttu-id="9d88f-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="9d88f-139">DateTime the object was last modified.</span></span> <span data-ttu-id="9d88f-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9d88f-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9d88f-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9d88f-141">roleScopeTagIds</span></span>|<span data-ttu-id="9d88f-142">String collection</span><span class="sxs-lookup"><span data-stu-id="9d88f-142">String collection</span></span>|<span data-ttu-id="9d88f-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="9d88f-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9d88f-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9d88f-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9d88f-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="9d88f-145">supportsScopeTags</span></span>|<span data-ttu-id="9d88f-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="9d88f-146">Boolean</span></span>|<span data-ttu-id="9d88f-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="9d88f-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9d88f-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="9d88f-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9d88f-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="9d88f-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9d88f-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9d88f-150">This property is read-only.</span></span> <span data-ttu-id="9d88f-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9d88f-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9d88f-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9d88f-152">createdDateTime</span></span>|<span data-ttu-id="9d88f-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d88f-153">DateTimeOffset</span></span>|<span data-ttu-id="9d88f-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="9d88f-154">DateTime the object was created.</span></span> <span data-ttu-id="9d88f-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9d88f-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9d88f-156">description</span><span class="sxs-lookup"><span data-stu-id="9d88f-156">description</span></span>|<span data-ttu-id="9d88f-157">String</span><span class="sxs-lookup"><span data-stu-id="9d88f-157">String</span></span>|<span data-ttu-id="9d88f-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9d88f-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9d88f-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9d88f-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9d88f-160">displayName</span><span class="sxs-lookup"><span data-stu-id="9d88f-160">displayName</span></span>|<span data-ttu-id="9d88f-161">String</span><span class="sxs-lookup"><span data-stu-id="9d88f-161">String</span></span>|<span data-ttu-id="9d88f-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9d88f-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9d88f-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9d88f-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9d88f-164">version</span><span class="sxs-lookup"><span data-stu-id="9d88f-164">version</span></span>|<span data-ttu-id="9d88f-165">Int32</span><span class="sxs-lookup"><span data-stu-id="9d88f-165">Int32</span></span>|<span data-ttu-id="9d88f-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9d88f-166">Version of the device configuration.</span></span> <span data-ttu-id="9d88f-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9d88f-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9d88f-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="9d88f-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="9d88f-169">Int32</span><span class="sxs-lookup"><span data-stu-id="9d88f-169">Int32</span></span>|<span data-ttu-id="9d88f-170">Porcentagem de limite de renovação de certificados.</span><span class="sxs-lookup"><span data-stu-id="9d88f-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="9d88f-171">Válido valores de 1 a 99 Inherited de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="9d88f-171">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="9d88f-172">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="9d88f-172">keyStorageProvider</span></span>|[<span data-ttu-id="9d88f-173">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="9d88f-173">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="9d88f-174">Provedor de armazenamento de chave (KSP) Inherited de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="9d88f-174">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="9d88f-175">Os valores possíveis são: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="9d88f-175">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="9d88f-176">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="9d88f-176">subjectNameFormat</span></span>|[<span data-ttu-id="9d88f-177">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="9d88f-177">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="9d88f-178">Certificado assunto nome formato herdado do [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="9d88f-178">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="9d88f-179">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="9d88f-179">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="9d88f-180">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="9d88f-180">subjectAlternativeNameType</span></span>|[<span data-ttu-id="9d88f-181">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="9d88f-181">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="9d88f-182">Certificado Subject Alternative nome tipo herdada do [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="9d88f-182">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="9d88f-183">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="9d88f-183">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="9d88f-184">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="9d88f-184">certificateValidityPeriodValue</span></span>|<span data-ttu-id="9d88f-185">Int32</span><span class="sxs-lookup"><span data-stu-id="9d88f-185">Int32</span></span>|<span data-ttu-id="9d88f-186">Valor para o período de validade de certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="9d88f-186">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="9d88f-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="9d88f-187">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="9d88f-188">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="9d88f-188">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="9d88f-189">Escala para o período de validade de certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="9d88f-189">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="9d88f-190">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="9d88f-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="9d88f-191">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="9d88f-191">extendedKeyUsages</span></span>|<span data-ttu-id="9d88f-192">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="9d88f-192">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="9d88f-193">Configurações de uso de chave (EKU) estendido.</span><span class="sxs-lookup"><span data-stu-id="9d88f-193">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="9d88f-194">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="9d88f-194">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="9d88f-195">Herdado de [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="9d88f-195">Inherited from [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="9d88f-196">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="9d88f-196">customSubjectAlternativeNames</span></span>|<span data-ttu-id="9d88f-197">coleção [customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="9d88f-197">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="9d88f-198">Configurações de Alterantive nome de entidade personalizada.</span><span class="sxs-lookup"><span data-stu-id="9d88f-198">Custom Subject Alterantive Name Settings.</span></span> <span data-ttu-id="9d88f-199">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="9d88f-199">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="9d88f-200">Herdado de [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="9d88f-200">Inherited from [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="9d88f-201">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="9d88f-201">scepServerUrls</span></span>|<span data-ttu-id="9d88f-202">String collection</span><span class="sxs-lookup"><span data-stu-id="9d88f-202">String collection</span></span>|<span data-ttu-id="9d88f-203">URLs de servidor SCEP.</span><span class="sxs-lookup"><span data-stu-id="9d88f-203">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="9d88f-204">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="9d88f-204">subjectNameFormatString</span></span>|<span data-ttu-id="9d88f-205">String</span><span class="sxs-lookup"><span data-stu-id="9d88f-205">String</span></span>|<span data-ttu-id="9d88f-206">Um formato personalizado a ser usada com SubjectNameFormat = personalizado.</span><span class="sxs-lookup"><span data-stu-id="9d88f-206">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="9d88f-207">Exemplo: CN = {{EmailAddress}}, F = {{EmailAddress}}, OU = usuários do Enterprise, O = Contoso Corporation, L = Redmond, ST = WA, C = US</span><span class="sxs-lookup"><span data-stu-id="9d88f-207">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="9d88f-208">keyUsage</span><span class="sxs-lookup"><span data-stu-id="9d88f-208">keyUsage</span></span>|[<span data-ttu-id="9d88f-209">keyUsages</span><span class="sxs-lookup"><span data-stu-id="9d88f-209">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="9d88f-210">Uso de chave SCEP.</span><span class="sxs-lookup"><span data-stu-id="9d88f-210">SCEP Key Usage.</span></span> <span data-ttu-id="9d88f-211">Os valores possíveis são: `keyEncipherment` e `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="9d88f-211">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="9d88f-212">keySize</span><span class="sxs-lookup"><span data-stu-id="9d88f-212">keySize</span></span>|[<span data-ttu-id="9d88f-213">keySize</span><span class="sxs-lookup"><span data-stu-id="9d88f-213">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="9d88f-214">Tamanho da chave SCEP.</span><span class="sxs-lookup"><span data-stu-id="9d88f-214">SCEP Key Size.</span></span> <span data-ttu-id="9d88f-215">Os valores possíveis são: `size1024` e `size2048`.</span><span class="sxs-lookup"><span data-stu-id="9d88f-215">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="9d88f-216">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="9d88f-216">hashAlgorithm</span></span>|[<span data-ttu-id="9d88f-217">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="9d88f-217">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="9d88f-218">Algoritmo de Hash SCEP.</span><span class="sxs-lookup"><span data-stu-id="9d88f-218">SCEP Hash Algorithm.</span></span> <span data-ttu-id="9d88f-219">Os valores possíveis são: `sha1` e `sha2`.</span><span class="sxs-lookup"><span data-stu-id="9d88f-219">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="9d88f-220">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="9d88f-220">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="9d88f-221">String</span><span class="sxs-lookup"><span data-stu-id="9d88f-221">String</span></span>|<span data-ttu-id="9d88f-222">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="9d88f-222">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="9d88f-223">certificateStore</span><span class="sxs-lookup"><span data-stu-id="9d88f-223">certificateStore</span></span>|[<span data-ttu-id="9d88f-224">certificateStore</span><span class="sxs-lookup"><span data-stu-id="9d88f-224">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="9d88f-225">Certificado do repositório de destino.</span><span class="sxs-lookup"><span data-stu-id="9d88f-225">Target store certificate.</span></span> <span data-ttu-id="9d88f-226">Os valores possíveis são: `user` e `machine`.</span><span class="sxs-lookup"><span data-stu-id="9d88f-226">Possible values are: `user`, `machine`.</span></span>|



## <a name="response"></a><span data-ttu-id="9d88f-227">Resposta</span><span class="sxs-lookup"><span data-stu-id="9d88f-227">Response</span></span>
<span data-ttu-id="9d88f-228">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9d88f-228">If successful, this method returns a `200 OK` response code and an updated [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d88f-229">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9d88f-229">Example</span></span>
### <a name="request"></a><span data-ttu-id="9d88f-230">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9d88f-230">Request</span></span>
<span data-ttu-id="9d88f-231">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9d88f-231">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1245

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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

### <a name="response"></a><span data-ttu-id="9d88f-232">Resposta</span><span class="sxs-lookup"><span data-stu-id="9d88f-232">Response</span></span>
<span data-ttu-id="9d88f-p123">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9d88f-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1423

{
  "@odata.type": "#microsoft.graph.windows81SCEPCertificateProfile",
  "id": "2daf8af2-8af2-2daf-f28a-af2df28aaf2d",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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





