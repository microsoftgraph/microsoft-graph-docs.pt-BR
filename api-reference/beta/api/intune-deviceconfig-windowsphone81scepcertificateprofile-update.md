---
title: Atualizar windowsPhone81SCEPCertificateProfile
description: Atualize as propriedades de um objeto windowsPhone81SCEPCertificateProfile.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e41cd55846cf5a87bfa8b43aaef31e6a7b1eb245
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404691"
---
# <a name="update-windowsphone81scepcertificateprofile"></a><span data-ttu-id="e40bc-103">Atualizar windowsPhone81SCEPCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="e40bc-103">Update windowsPhone81SCEPCertificateProfile</span></span>

> <span data-ttu-id="e40bc-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="e40bc-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e40bc-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e40bc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e40bc-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="e40bc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e40bc-107">Atualize as propriedades de um objeto [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="e40bc-107">Update the properties of a [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e40bc-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e40bc-108">Prerequisites</span></span>
<span data-ttu-id="e40bc-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e40bc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e40bc-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e40bc-111">Permission type</span></span>|<span data-ttu-id="e40bc-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e40bc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e40bc-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e40bc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e40bc-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e40bc-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e40bc-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e40bc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e40bc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e40bc-116">Not supported.</span></span>|
|<span data-ttu-id="e40bc-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e40bc-117">Application</span></span>|<span data-ttu-id="e40bc-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e40bc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e40bc-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e40bc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="e40bc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e40bc-120">Request headers</span></span>
|<span data-ttu-id="e40bc-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e40bc-121">Header</span></span>|<span data-ttu-id="e40bc-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e40bc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e40bc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e40bc-123">Authorization</span></span>|<span data-ttu-id="e40bc-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e40bc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e40bc-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e40bc-125">Accept</span></span>|<span data-ttu-id="e40bc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e40bc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e40bc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e40bc-127">Request body</span></span>
<span data-ttu-id="e40bc-128">No corpo da solicitação, fornece uma representação JSON para o objeto [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="e40bc-128">In the request body, supply a JSON representation for the [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object.</span></span>

<span data-ttu-id="e40bc-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="e40bc-129">The following table shows the properties that are required when you create the [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md).</span></span>

|<span data-ttu-id="e40bc-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e40bc-130">Property</span></span>|<span data-ttu-id="e40bc-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e40bc-131">Type</span></span>|<span data-ttu-id="e40bc-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e40bc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e40bc-133">id</span><span class="sxs-lookup"><span data-stu-id="e40bc-133">id</span></span>|<span data-ttu-id="e40bc-134">String</span><span class="sxs-lookup"><span data-stu-id="e40bc-134">String</span></span>|<span data-ttu-id="e40bc-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e40bc-135">Key of the entity.</span></span> <span data-ttu-id="e40bc-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e40bc-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e40bc-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e40bc-137">lastModifiedDateTime</span></span>|<span data-ttu-id="e40bc-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e40bc-138">DateTimeOffset</span></span>|<span data-ttu-id="e40bc-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="e40bc-139">DateTime the object was last modified.</span></span> <span data-ttu-id="e40bc-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e40bc-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e40bc-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e40bc-141">roleScopeTagIds</span></span>|<span data-ttu-id="e40bc-142">String collection</span><span class="sxs-lookup"><span data-stu-id="e40bc-142">String collection</span></span>|<span data-ttu-id="e40bc-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="e40bc-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e40bc-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e40bc-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e40bc-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="e40bc-145">supportsScopeTags</span></span>|<span data-ttu-id="e40bc-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="e40bc-146">Boolean</span></span>|<span data-ttu-id="e40bc-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="e40bc-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e40bc-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="e40bc-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e40bc-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="e40bc-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e40bc-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e40bc-150">This property is read-only.</span></span> <span data-ttu-id="e40bc-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e40bc-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e40bc-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e40bc-152">createdDateTime</span></span>|<span data-ttu-id="e40bc-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e40bc-153">DateTimeOffset</span></span>|<span data-ttu-id="e40bc-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="e40bc-154">DateTime the object was created.</span></span> <span data-ttu-id="e40bc-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e40bc-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e40bc-156">description</span><span class="sxs-lookup"><span data-stu-id="e40bc-156">description</span></span>|<span data-ttu-id="e40bc-157">String</span><span class="sxs-lookup"><span data-stu-id="e40bc-157">String</span></span>|<span data-ttu-id="e40bc-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e40bc-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e40bc-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e40bc-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e40bc-160">displayName</span><span class="sxs-lookup"><span data-stu-id="e40bc-160">displayName</span></span>|<span data-ttu-id="e40bc-161">String</span><span class="sxs-lookup"><span data-stu-id="e40bc-161">String</span></span>|<span data-ttu-id="e40bc-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e40bc-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e40bc-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e40bc-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e40bc-164">version</span><span class="sxs-lookup"><span data-stu-id="e40bc-164">version</span></span>|<span data-ttu-id="e40bc-165">Int32</span><span class="sxs-lookup"><span data-stu-id="e40bc-165">Int32</span></span>|<span data-ttu-id="e40bc-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e40bc-166">Version of the device configuration.</span></span> <span data-ttu-id="e40bc-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e40bc-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e40bc-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="e40bc-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="e40bc-169">Int32</span><span class="sxs-lookup"><span data-stu-id="e40bc-169">Int32</span></span>|<span data-ttu-id="e40bc-170">Porcentagem de limite de renovação de certificados.</span><span class="sxs-lookup"><span data-stu-id="e40bc-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="e40bc-171">Herdado de [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="e40bc-171">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="e40bc-172">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="e40bc-172">keyStorageProvider</span></span>|[<span data-ttu-id="e40bc-173">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="e40bc-173">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="e40bc-174">Provedor de armazenamento de chave (KSP).</span><span class="sxs-lookup"><span data-stu-id="e40bc-174">Key Storage Provider (KSP).</span></span> <span data-ttu-id="e40bc-175">Herdada do [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="e40bc-175">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="e40bc-176">Os valores possíveis são: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="e40bc-176">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="e40bc-177">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="e40bc-177">subjectNameFormat</span></span>|[<span data-ttu-id="e40bc-178">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="e40bc-178">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="e40bc-179">Formato de nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="e40bc-179">Certificate Subject Name Format.</span></span> <span data-ttu-id="e40bc-180">Herdada do [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="e40bc-180">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="e40bc-181">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="e40bc-181">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="e40bc-182">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="e40bc-182">subjectAlternativeNameType</span></span>|[<span data-ttu-id="e40bc-183">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="e40bc-183">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="e40bc-184">Tipo de nome alternativo de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="e40bc-184">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="e40bc-185">Herdada do [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="e40bc-185">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="e40bc-186">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="e40bc-186">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="e40bc-187">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="e40bc-187">certificateValidityPeriodValue</span></span>|<span data-ttu-id="e40bc-188">Int32</span><span class="sxs-lookup"><span data-stu-id="e40bc-188">Int32</span></span>|<span data-ttu-id="e40bc-189">Valor para o período de Validtiy do certificado.</span><span class="sxs-lookup"><span data-stu-id="e40bc-189">Value for the Certificate Validtiy Period.</span></span> <span data-ttu-id="e40bc-190">Herdado de [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="e40bc-190">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="e40bc-191">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="e40bc-191">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="e40bc-192">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="e40bc-192">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="e40bc-193">Escala para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="e40bc-193">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="e40bc-194">Herdada do [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="e40bc-194">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="e40bc-195">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="e40bc-195">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="e40bc-196">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="e40bc-196">extendedKeyUsages</span></span>|<span data-ttu-id="e40bc-197">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="e40bc-197">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="e40bc-198">Configurações de uso de chave (EKU) estendido.</span><span class="sxs-lookup"><span data-stu-id="e40bc-198">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="e40bc-199">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="e40bc-199">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="e40bc-200">Herdado de [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="e40bc-200">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="e40bc-201">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="e40bc-201">scepServerUrls</span></span>|<span data-ttu-id="e40bc-202">String collection</span><span class="sxs-lookup"><span data-stu-id="e40bc-202">String collection</span></span>|<span data-ttu-id="e40bc-203">URLs de servidor SCEP.</span><span class="sxs-lookup"><span data-stu-id="e40bc-203">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="e40bc-204">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="e40bc-204">subjectNameFormatString</span></span>|<span data-ttu-id="e40bc-205">String</span><span class="sxs-lookup"><span data-stu-id="e40bc-205">String</span></span>|<span data-ttu-id="e40bc-206">Um formato personalizado a ser usada com SubjectNameFormat = personalizado.</span><span class="sxs-lookup"><span data-stu-id="e40bc-206">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="e40bc-207">Exemplo: CN = {{EmailAddress}}, F = {{EmailAddress}}, OU = usuários do Enterprise, O = Contoso Corporation, L = Redmond, ST = WA, C = US</span><span class="sxs-lookup"><span data-stu-id="e40bc-207">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="e40bc-208">keyUsage</span><span class="sxs-lookup"><span data-stu-id="e40bc-208">keyUsage</span></span>|[<span data-ttu-id="e40bc-209">keyUsages</span><span class="sxs-lookup"><span data-stu-id="e40bc-209">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="e40bc-210">Uso de chave SCEP.</span><span class="sxs-lookup"><span data-stu-id="e40bc-210">SCEP Key Usage.</span></span> <span data-ttu-id="e40bc-211">Os valores possíveis são: `keyEncipherment` e `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="e40bc-211">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="e40bc-212">keySize</span><span class="sxs-lookup"><span data-stu-id="e40bc-212">keySize</span></span>|[<span data-ttu-id="e40bc-213">keySize</span><span class="sxs-lookup"><span data-stu-id="e40bc-213">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="e40bc-214">Tamanho da chave SCEP.</span><span class="sxs-lookup"><span data-stu-id="e40bc-214">SCEP Key Size.</span></span> <span data-ttu-id="e40bc-215">Os valores possíveis são: `size1024` e `size2048`.</span><span class="sxs-lookup"><span data-stu-id="e40bc-215">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="e40bc-216">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="e40bc-216">hashAlgorithm</span></span>|[<span data-ttu-id="e40bc-217">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="e40bc-217">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="e40bc-218">Algoritmo de Hash SCEP.</span><span class="sxs-lookup"><span data-stu-id="e40bc-218">SCEP Hash Algorithm.</span></span> <span data-ttu-id="e40bc-219">Os valores possíveis são: `sha1` e `sha2`.</span><span class="sxs-lookup"><span data-stu-id="e40bc-219">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="e40bc-220">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="e40bc-220">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="e40bc-221">String</span><span class="sxs-lookup"><span data-stu-id="e40bc-221">String</span></span>|<span data-ttu-id="e40bc-222">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="e40bc-222">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="e40bc-223">Resposta</span><span class="sxs-lookup"><span data-stu-id="e40bc-223">Response</span></span>
<span data-ttu-id="e40bc-224">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e40bc-224">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e40bc-225">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e40bc-225">Example</span></span>

### <a name="request"></a><span data-ttu-id="e40bc-226">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e40bc-226">Request</span></span>
<span data-ttu-id="e40bc-227">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e40bc-227">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1032

{
  "@odata.type": "#microsoft.graph.windowsPhone81SCEPCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="e40bc-228">Resposta</span><span class="sxs-lookup"><span data-stu-id="e40bc-228">Response</span></span>
<span data-ttu-id="e40bc-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e40bc-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1204

{
  "@odata.type": "#microsoft.graph.windowsPhone81SCEPCertificateProfile",
  "id": "f070e30e-e30e-f070-0ee3-70f00ee370f0",
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




