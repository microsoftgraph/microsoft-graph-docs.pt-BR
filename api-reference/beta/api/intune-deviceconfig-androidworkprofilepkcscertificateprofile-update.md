---
title: Atualizar androidWorkProfilePkcsCertificateProfile
description: Atualize as propriedades de um objeto androidWorkProfilePkcsCertificateProfile.
author: tfitzmac
ms.openlocfilehash: dbd3adbcc15b7b46e51ff3a2874e340c78339ac2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27355892"
---
# <a name="update-androidworkprofilepkcscertificateprofile"></a><span data-ttu-id="86ad2-103">Atualizar androidWorkProfilePkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="86ad2-103">Update androidWorkProfilePkcsCertificateProfile</span></span>

> <span data-ttu-id="86ad2-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="86ad2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="86ad2-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="86ad2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="86ad2-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="86ad2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="86ad2-107">Atualize as propriedades de um objeto [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="86ad2-107">Update the properties of a [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="86ad2-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="86ad2-108">Prerequisites</span></span>
<span data-ttu-id="86ad2-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86ad2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86ad2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="86ad2-111">Permission type</span></span>|<span data-ttu-id="86ad2-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="86ad2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86ad2-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="86ad2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="86ad2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86ad2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="86ad2-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="86ad2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86ad2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="86ad2-116">Not supported.</span></span>|
|<span data-ttu-id="86ad2-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="86ad2-117">Application</span></span>|<span data-ttu-id="86ad2-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="86ad2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="86ad2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="86ad2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="86ad2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="86ad2-120">Request headers</span></span>
|<span data-ttu-id="86ad2-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="86ad2-121">Header</span></span>|<span data-ttu-id="86ad2-122">Valor</span><span class="sxs-lookup"><span data-stu-id="86ad2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="86ad2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="86ad2-123">Authorization</span></span>|<span data-ttu-id="86ad2-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="86ad2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="86ad2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="86ad2-125">Accept</span></span>|<span data-ttu-id="86ad2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="86ad2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="86ad2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="86ad2-127">Request body</span></span>
<span data-ttu-id="86ad2-128">No corpo da solicitação, fornece uma representação JSON para o objeto [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="86ad2-128">In the request body, supply a JSON representation for the [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) object.</span></span>

<span data-ttu-id="86ad2-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="86ad2-129">The following table shows the properties that are required when you create the [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md).</span></span>

|<span data-ttu-id="86ad2-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="86ad2-130">Property</span></span>|<span data-ttu-id="86ad2-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="86ad2-131">Type</span></span>|<span data-ttu-id="86ad2-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="86ad2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86ad2-133">id</span><span class="sxs-lookup"><span data-stu-id="86ad2-133">id</span></span>|<span data-ttu-id="86ad2-134">String</span><span class="sxs-lookup"><span data-stu-id="86ad2-134">String</span></span>|<span data-ttu-id="86ad2-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="86ad2-135">Key of the entity.</span></span> <span data-ttu-id="86ad2-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86ad2-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86ad2-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="86ad2-137">lastModifiedDateTime</span></span>|<span data-ttu-id="86ad2-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86ad2-138">DateTimeOffset</span></span>|<span data-ttu-id="86ad2-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="86ad2-139">DateTime the object was last modified.</span></span> <span data-ttu-id="86ad2-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86ad2-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86ad2-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="86ad2-141">roleScopeTagIds</span></span>|<span data-ttu-id="86ad2-142">String collection</span><span class="sxs-lookup"><span data-stu-id="86ad2-142">String collection</span></span>|<span data-ttu-id="86ad2-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="86ad2-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="86ad2-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86ad2-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86ad2-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="86ad2-145">supportsScopeTags</span></span>|<span data-ttu-id="86ad2-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="86ad2-146">Boolean</span></span>|<span data-ttu-id="86ad2-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="86ad2-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="86ad2-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="86ad2-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="86ad2-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="86ad2-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="86ad2-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="86ad2-150">This property is read-only.</span></span> <span data-ttu-id="86ad2-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86ad2-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86ad2-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="86ad2-152">createdDateTime</span></span>|<span data-ttu-id="86ad2-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86ad2-153">DateTimeOffset</span></span>|<span data-ttu-id="86ad2-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="86ad2-154">DateTime the object was created.</span></span> <span data-ttu-id="86ad2-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86ad2-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86ad2-156">description</span><span class="sxs-lookup"><span data-stu-id="86ad2-156">description</span></span>|<span data-ttu-id="86ad2-157">String</span><span class="sxs-lookup"><span data-stu-id="86ad2-157">String</span></span>|<span data-ttu-id="86ad2-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="86ad2-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="86ad2-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86ad2-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86ad2-160">displayName</span><span class="sxs-lookup"><span data-stu-id="86ad2-160">displayName</span></span>|<span data-ttu-id="86ad2-161">String</span><span class="sxs-lookup"><span data-stu-id="86ad2-161">String</span></span>|<span data-ttu-id="86ad2-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="86ad2-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="86ad2-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86ad2-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86ad2-164">version</span><span class="sxs-lookup"><span data-stu-id="86ad2-164">version</span></span>|<span data-ttu-id="86ad2-165">Int32</span><span class="sxs-lookup"><span data-stu-id="86ad2-165">Int32</span></span>|<span data-ttu-id="86ad2-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="86ad2-166">Version of the device configuration.</span></span> <span data-ttu-id="86ad2-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86ad2-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86ad2-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="86ad2-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="86ad2-169">Int32</span><span class="sxs-lookup"><span data-stu-id="86ad2-169">Int32</span></span>|<span data-ttu-id="86ad2-170">Porcentagem de limite de renovação de certificados.</span><span class="sxs-lookup"><span data-stu-id="86ad2-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="86ad2-171">Válido valores de 1 a 99 Inherited de [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="86ad2-171">Valid values 1 to 99 Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="86ad2-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="86ad2-172">subjectNameFormat</span></span>|[<span data-ttu-id="86ad2-173">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="86ad2-173">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="86ad2-174">Formato de nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="86ad2-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="86ad2-175">Herdada do [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="86ad2-175">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="86ad2-176">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="86ad2-176">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="86ad2-177">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="86ad2-177">certificateValidityPeriodValue</span></span>|<span data-ttu-id="86ad2-178">Int32</span><span class="sxs-lookup"><span data-stu-id="86ad2-178">Int32</span></span>|<span data-ttu-id="86ad2-179">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="86ad2-179">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="86ad2-180">Herdado de [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="86ad2-180">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="86ad2-181">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="86ad2-181">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="86ad2-182">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="86ad2-182">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="86ad2-183">Escala para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="86ad2-183">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="86ad2-184">Herdada do [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="86ad2-184">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="86ad2-185">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="86ad2-185">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="86ad2-186">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="86ad2-186">extendedKeyUsages</span></span>|<span data-ttu-id="86ad2-187">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="86ad2-187">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="86ad2-188">Configurações de uso de chave (EKU) estendido.</span><span class="sxs-lookup"><span data-stu-id="86ad2-188">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="86ad2-189">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="86ad2-189">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="86ad2-190">Herdado de [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="86ad2-190">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="86ad2-191">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="86ad2-191">certificationAuthority</span></span>|<span data-ttu-id="86ad2-192">String</span><span class="sxs-lookup"><span data-stu-id="86ad2-192">String</span></span>|<span data-ttu-id="86ad2-193">Autoridade de certificação PKCS</span><span class="sxs-lookup"><span data-stu-id="86ad2-193">PKCS Certification Authority</span></span>|
|<span data-ttu-id="86ad2-194">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="86ad2-194">certificationAuthorityName</span></span>|<span data-ttu-id="86ad2-195">String</span><span class="sxs-lookup"><span data-stu-id="86ad2-195">String</span></span>|<span data-ttu-id="86ad2-196">Nome da autoridade de certificação PKCS</span><span class="sxs-lookup"><span data-stu-id="86ad2-196">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="86ad2-197">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="86ad2-197">certificateTemplateName</span></span>|<span data-ttu-id="86ad2-198">String</span><span class="sxs-lookup"><span data-stu-id="86ad2-198">String</span></span>|<span data-ttu-id="86ad2-199">Nome do modelo de certificado PKCS</span><span class="sxs-lookup"><span data-stu-id="86ad2-199">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="86ad2-200">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="86ad2-200">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="86ad2-201">String</span><span class="sxs-lookup"><span data-stu-id="86ad2-201">String</span></span>|<span data-ttu-id="86ad2-202">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="86ad2-202">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="86ad2-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="86ad2-203">subjectAlternativeNameType</span></span>|[<span data-ttu-id="86ad2-204">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="86ad2-204">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="86ad2-205">Tipo de nome alternativo de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="86ad2-205">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="86ad2-206">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="86ad2-206">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|



## <a name="response"></a><span data-ttu-id="86ad2-207">Resposta</span><span class="sxs-lookup"><span data-stu-id="86ad2-207">Response</span></span>
<span data-ttu-id="86ad2-208">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="86ad2-208">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86ad2-209">Exemplo</span><span class="sxs-lookup"><span data-stu-id="86ad2-209">Example</span></span>
### <a name="request"></a><span data-ttu-id="86ad2-210">Solicitação</span><span class="sxs-lookup"><span data-stu-id="86ad2-210">Request</span></span>
<span data-ttu-id="86ad2-211">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="86ad2-211">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 954

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
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "subjectAlternativeNameType": "emailAddress"
}
```

### <a name="response"></a><span data-ttu-id="86ad2-212">Resposta</span><span class="sxs-lookup"><span data-stu-id="86ad2-212">Response</span></span>
<span data-ttu-id="86ad2-p117">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="86ad2-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1141

{
  "@odata.type": "#microsoft.graph.androidWorkProfilePkcsCertificateProfile",
  "id": "a7d4a505-a505-a7d4-05a5-d4a705a5d4a7",
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
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "subjectAlternativeNameType": "emailAddress"
}
```





