---
title: Atualizar androidPkcsCertificateProfile
description: Atualize as propriedades de um objeto androidPkcsCertificateProfile.
author: tfitzmac
ms.openlocfilehash: 6600f2a98fa73cfd86d0c728edbd96c36bb876e3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308243"
---
# <a name="update-androidpkcscertificateprofile"></a><span data-ttu-id="03c3e-103">Atualizar androidPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="03c3e-103">Update androidPkcsCertificateProfile</span></span>

> <span data-ttu-id="03c3e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="03c3e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="03c3e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="03c3e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="03c3e-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="03c3e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="03c3e-107">Atualize as propriedades de um objeto [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="03c3e-107">Update the properties of a [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="03c3e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="03c3e-108">Prerequisites</span></span>
<span data-ttu-id="03c3e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03c3e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03c3e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="03c3e-111">Permission type</span></span>|<span data-ttu-id="03c3e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="03c3e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="03c3e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="03c3e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="03c3e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03c3e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="03c3e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="03c3e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="03c3e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="03c3e-116">Not supported.</span></span>|
|<span data-ttu-id="03c3e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="03c3e-117">Application</span></span>|<span data-ttu-id="03c3e-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="03c3e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="03c3e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="03c3e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="03c3e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="03c3e-120">Request headers</span></span>
|<span data-ttu-id="03c3e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="03c3e-121">Header</span></span>|<span data-ttu-id="03c3e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="03c3e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="03c3e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="03c3e-123">Authorization</span></span>|<span data-ttu-id="03c3e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="03c3e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="03c3e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="03c3e-125">Accept</span></span>|<span data-ttu-id="03c3e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="03c3e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="03c3e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="03c3e-127">Request body</span></span>
<span data-ttu-id="03c3e-128">No corpo da solicitação, fornece uma representação JSON para o objeto [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="03c3e-128">In the request body, supply a JSON representation for the [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) object.</span></span>

<span data-ttu-id="03c3e-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="03c3e-129">The following table shows the properties that are required when you create the [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md).</span></span>

|<span data-ttu-id="03c3e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="03c3e-130">Property</span></span>|<span data-ttu-id="03c3e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="03c3e-131">Type</span></span>|<span data-ttu-id="03c3e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="03c3e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03c3e-133">id</span><span class="sxs-lookup"><span data-stu-id="03c3e-133">id</span></span>|<span data-ttu-id="03c3e-134">String</span><span class="sxs-lookup"><span data-stu-id="03c3e-134">String</span></span>|<span data-ttu-id="03c3e-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="03c3e-135">Key of the entity.</span></span> <span data-ttu-id="03c3e-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03c3e-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03c3e-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="03c3e-137">lastModifiedDateTime</span></span>|<span data-ttu-id="03c3e-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03c3e-138">DateTimeOffset</span></span>|<span data-ttu-id="03c3e-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="03c3e-139">DateTime the object was last modified.</span></span> <span data-ttu-id="03c3e-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03c3e-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03c3e-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="03c3e-141">roleScopeTagIds</span></span>|<span data-ttu-id="03c3e-142">String collection</span><span class="sxs-lookup"><span data-stu-id="03c3e-142">String collection</span></span>|<span data-ttu-id="03c3e-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="03c3e-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="03c3e-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03c3e-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03c3e-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="03c3e-145">supportsScopeTags</span></span>|<span data-ttu-id="03c3e-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="03c3e-146">Boolean</span></span>|<span data-ttu-id="03c3e-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="03c3e-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="03c3e-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="03c3e-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="03c3e-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="03c3e-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="03c3e-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="03c3e-150">This property is read-only.</span></span> <span data-ttu-id="03c3e-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03c3e-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03c3e-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="03c3e-152">createdDateTime</span></span>|<span data-ttu-id="03c3e-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03c3e-153">DateTimeOffset</span></span>|<span data-ttu-id="03c3e-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="03c3e-154">DateTime the object was created.</span></span> <span data-ttu-id="03c3e-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03c3e-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03c3e-156">description</span><span class="sxs-lookup"><span data-stu-id="03c3e-156">description</span></span>|<span data-ttu-id="03c3e-157">String</span><span class="sxs-lookup"><span data-stu-id="03c3e-157">String</span></span>|<span data-ttu-id="03c3e-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="03c3e-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="03c3e-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03c3e-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03c3e-160">displayName</span><span class="sxs-lookup"><span data-stu-id="03c3e-160">displayName</span></span>|<span data-ttu-id="03c3e-161">String</span><span class="sxs-lookup"><span data-stu-id="03c3e-161">String</span></span>|<span data-ttu-id="03c3e-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="03c3e-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="03c3e-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03c3e-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03c3e-164">version</span><span class="sxs-lookup"><span data-stu-id="03c3e-164">version</span></span>|<span data-ttu-id="03c3e-165">Int32</span><span class="sxs-lookup"><span data-stu-id="03c3e-165">Int32</span></span>|<span data-ttu-id="03c3e-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="03c3e-166">Version of the device configuration.</span></span> <span data-ttu-id="03c3e-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03c3e-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03c3e-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="03c3e-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="03c3e-169">Int32</span><span class="sxs-lookup"><span data-stu-id="03c3e-169">Int32</span></span>|<span data-ttu-id="03c3e-170">Porcentagem de limite de renovação de certificados.</span><span class="sxs-lookup"><span data-stu-id="03c3e-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="03c3e-171">Válido valores de 1 a 99 Inherited de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="03c3e-171">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="03c3e-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="03c3e-172">subjectNameFormat</span></span>|[<span data-ttu-id="03c3e-173">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="03c3e-173">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="03c3e-174">Formato de nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="03c3e-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="03c3e-175">Herdada do [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="03c3e-175">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="03c3e-176">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="03c3e-176">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="03c3e-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="03c3e-177">subjectAlternativeNameType</span></span>|[<span data-ttu-id="03c3e-178">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="03c3e-178">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="03c3e-179">Tipo de nome alternativo de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="03c3e-179">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="03c3e-180">Herdada do [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="03c3e-180">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="03c3e-181">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="03c3e-181">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="03c3e-182">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="03c3e-182">certificateValidityPeriodValue</span></span>|<span data-ttu-id="03c3e-183">Int32</span><span class="sxs-lookup"><span data-stu-id="03c3e-183">Int32</span></span>|<span data-ttu-id="03c3e-184">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="03c3e-184">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="03c3e-185">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="03c3e-185">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="03c3e-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="03c3e-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="03c3e-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="03c3e-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="03c3e-188">Escala para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="03c3e-188">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="03c3e-189">Herdada do [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="03c3e-189">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="03c3e-190">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="03c3e-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="03c3e-191">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="03c3e-191">extendedKeyUsages</span></span>|<span data-ttu-id="03c3e-192">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="03c3e-192">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="03c3e-193">Configurações de uso de chave (EKU) estendido.</span><span class="sxs-lookup"><span data-stu-id="03c3e-193">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="03c3e-194">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="03c3e-194">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="03c3e-195">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="03c3e-195">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="03c3e-196">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="03c3e-196">certificationAuthority</span></span>|<span data-ttu-id="03c3e-197">String</span><span class="sxs-lookup"><span data-stu-id="03c3e-197">String</span></span>|<span data-ttu-id="03c3e-198">Autoridade de certificação PKCS</span><span class="sxs-lookup"><span data-stu-id="03c3e-198">PKCS Certification Authority</span></span>|
|<span data-ttu-id="03c3e-199">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="03c3e-199">certificationAuthorityName</span></span>|<span data-ttu-id="03c3e-200">String</span><span class="sxs-lookup"><span data-stu-id="03c3e-200">String</span></span>|<span data-ttu-id="03c3e-201">Nome da autoridade de certificação PKCS</span><span class="sxs-lookup"><span data-stu-id="03c3e-201">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="03c3e-202">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="03c3e-202">certificateTemplateName</span></span>|<span data-ttu-id="03c3e-203">String</span><span class="sxs-lookup"><span data-stu-id="03c3e-203">String</span></span>|<span data-ttu-id="03c3e-204">Nome do modelo de certificado PKCS</span><span class="sxs-lookup"><span data-stu-id="03c3e-204">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="03c3e-205">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="03c3e-205">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="03c3e-206">String</span><span class="sxs-lookup"><span data-stu-id="03c3e-206">String</span></span>|<span data-ttu-id="03c3e-207">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="03c3e-207">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="03c3e-208">Resposta</span><span class="sxs-lookup"><span data-stu-id="03c3e-208">Response</span></span>
<span data-ttu-id="03c3e-209">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="03c3e-209">If successful, this method returns a `200 OK` response code and an updated [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03c3e-210">Exemplo</span><span class="sxs-lookup"><span data-stu-id="03c3e-210">Example</span></span>
### <a name="request"></a><span data-ttu-id="03c3e-211">Solicitação</span><span class="sxs-lookup"><span data-stu-id="03c3e-211">Request</span></span>
<span data-ttu-id="03c3e-212">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="03c3e-212">Here is an example of the request.</span></span>
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
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```

### <a name="response"></a><span data-ttu-id="03c3e-213">Resposta</span><span class="sxs-lookup"><span data-stu-id="03c3e-213">Response</span></span>
<span data-ttu-id="03c3e-p117">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="03c3e-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1130

{
  "@odata.type": "#microsoft.graph.androidPkcsCertificateProfile",
  "id": "bb55705b-705b-bb55-5b70-55bb5b7055bb",
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
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```





