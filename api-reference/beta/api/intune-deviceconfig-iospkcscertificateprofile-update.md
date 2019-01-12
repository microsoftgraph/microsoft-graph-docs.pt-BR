---
title: Atualizar iosPkcsCertificateProfile
description: Atualize as propriedades de um objeto iosPkcsCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a0522b86eb762b34eb8b644f6416c16fa62f0c7e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27918729"
---
# <a name="update-iospkcscertificateprofile"></a><span data-ttu-id="b93f8-103">Atualizar iosPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="b93f8-103">Update iosPkcsCertificateProfile</span></span>

> <span data-ttu-id="b93f8-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b93f8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b93f8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b93f8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b93f8-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b93f8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b93f8-107">Atualize as propriedades de um objeto [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="b93f8-107">Update the properties of a [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b93f8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b93f8-108">Prerequisites</span></span>
<span data-ttu-id="b93f8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b93f8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b93f8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b93f8-111">Permission type</span></span>|<span data-ttu-id="b93f8-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b93f8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b93f8-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b93f8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b93f8-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b93f8-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b93f8-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b93f8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b93f8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b93f8-116">Not supported.</span></span>|
|<span data-ttu-id="b93f8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b93f8-117">Application</span></span>|<span data-ttu-id="b93f8-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b93f8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b93f8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b93f8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b93f8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b93f8-120">Request headers</span></span>
|<span data-ttu-id="b93f8-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b93f8-121">Header</span></span>|<span data-ttu-id="b93f8-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b93f8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b93f8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b93f8-123">Authorization</span></span>|<span data-ttu-id="b93f8-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b93f8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b93f8-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b93f8-125">Accept</span></span>|<span data-ttu-id="b93f8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b93f8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b93f8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b93f8-127">Request body</span></span>
<span data-ttu-id="b93f8-128">No corpo da solicitação, fornece uma representação JSON para o objeto [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="b93f8-128">In the request body, supply a JSON representation for the [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) object.</span></span>

<span data-ttu-id="b93f8-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="b93f8-129">The following table shows the properties that are required when you create the [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md).</span></span>

|<span data-ttu-id="b93f8-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b93f8-130">Property</span></span>|<span data-ttu-id="b93f8-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b93f8-131">Type</span></span>|<span data-ttu-id="b93f8-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b93f8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b93f8-133">id</span><span class="sxs-lookup"><span data-stu-id="b93f8-133">id</span></span>|<span data-ttu-id="b93f8-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b93f8-134">String</span></span>|<span data-ttu-id="b93f8-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b93f8-135">Key of the entity.</span></span> <span data-ttu-id="b93f8-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b93f8-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b93f8-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b93f8-137">lastModifiedDateTime</span></span>|<span data-ttu-id="b93f8-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b93f8-138">DateTimeOffset</span></span>|<span data-ttu-id="b93f8-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="b93f8-139">DateTime the object was last modified.</span></span> <span data-ttu-id="b93f8-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b93f8-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b93f8-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b93f8-141">roleScopeTagIds</span></span>|<span data-ttu-id="b93f8-142">String collection</span><span class="sxs-lookup"><span data-stu-id="b93f8-142">String collection</span></span>|<span data-ttu-id="b93f8-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="b93f8-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b93f8-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b93f8-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b93f8-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b93f8-145">supportsScopeTags</span></span>|<span data-ttu-id="b93f8-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="b93f8-146">Boolean</span></span>|<span data-ttu-id="b93f8-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="b93f8-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b93f8-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="b93f8-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b93f8-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="b93f8-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b93f8-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b93f8-150">This property is read-only.</span></span> <span data-ttu-id="b93f8-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b93f8-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b93f8-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b93f8-152">createdDateTime</span></span>|<span data-ttu-id="b93f8-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b93f8-153">DateTimeOffset</span></span>|<span data-ttu-id="b93f8-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="b93f8-154">DateTime the object was created.</span></span> <span data-ttu-id="b93f8-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b93f8-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b93f8-156">description</span><span class="sxs-lookup"><span data-stu-id="b93f8-156">description</span></span>|<span data-ttu-id="b93f8-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b93f8-157">String</span></span>|<span data-ttu-id="b93f8-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b93f8-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b93f8-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b93f8-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b93f8-160">displayName</span><span class="sxs-lookup"><span data-stu-id="b93f8-160">displayName</span></span>|<span data-ttu-id="b93f8-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b93f8-161">String</span></span>|<span data-ttu-id="b93f8-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b93f8-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b93f8-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b93f8-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b93f8-164">version</span><span class="sxs-lookup"><span data-stu-id="b93f8-164">version</span></span>|<span data-ttu-id="b93f8-165">Int32</span><span class="sxs-lookup"><span data-stu-id="b93f8-165">Int32</span></span>|<span data-ttu-id="b93f8-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b93f8-166">Version of the device configuration.</span></span> <span data-ttu-id="b93f8-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b93f8-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b93f8-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="b93f8-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="b93f8-169">Int32</span><span class="sxs-lookup"><span data-stu-id="b93f8-169">Int32</span></span>|<span data-ttu-id="b93f8-170">Porcentagem de limite de renovação de certificados.</span><span class="sxs-lookup"><span data-stu-id="b93f8-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="b93f8-171">Válido valores de 1 a 99 Inherited de [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="b93f8-171">Valid values 1 to 99 Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="b93f8-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="b93f8-172">subjectNameFormat</span></span>|[<span data-ttu-id="b93f8-173">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="b93f8-173">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="b93f8-174">Formato de nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="b93f8-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="b93f8-175">Herdada do [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="b93f8-175">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="b93f8-176">Os possíveis valores são: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="b93f8-176">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="b93f8-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="b93f8-177">subjectAlternativeNameType</span></span>|[<span data-ttu-id="b93f8-178">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="b93f8-178">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="b93f8-179">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="b93f8-179">Certificate Subject Alternative Name type.</span></span> <span data-ttu-id="b93f8-180">Herdada do [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="b93f8-180">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="b93f8-181">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="b93f8-181">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="b93f8-182">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="b93f8-182">certificateValidityPeriodValue</span></span>|<span data-ttu-id="b93f8-183">Int32</span><span class="sxs-lookup"><span data-stu-id="b93f8-183">Int32</span></span>|<span data-ttu-id="b93f8-184">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="b93f8-184">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="b93f8-185">Herdado de [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="b93f8-185">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="b93f8-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="b93f8-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="b93f8-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="b93f8-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="b93f8-188">Escala para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="b93f8-188">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="b93f8-189">Herdada do [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="b93f8-189">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="b93f8-190">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="b93f8-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="b93f8-191">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="b93f8-191">certificationAuthority</span></span>|<span data-ttu-id="b93f8-192">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b93f8-192">String</span></span>|<span data-ttu-id="b93f8-193">Autoridade de certificação PKCS.</span><span class="sxs-lookup"><span data-stu-id="b93f8-193">PKCS Certification Authority.</span></span>|
|<span data-ttu-id="b93f8-194">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="b93f8-194">certificationAuthorityName</span></span>|<span data-ttu-id="b93f8-195">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b93f8-195">String</span></span>|<span data-ttu-id="b93f8-196">Nome da autoridade de certificação PKCS.</span><span class="sxs-lookup"><span data-stu-id="b93f8-196">PKCS Certification Authority Name.</span></span>|
|<span data-ttu-id="b93f8-197">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="b93f8-197">certificateTemplateName</span></span>|<span data-ttu-id="b93f8-198">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b93f8-198">String</span></span>|<span data-ttu-id="b93f8-199">Nome do modelo de certificado PKCS.</span><span class="sxs-lookup"><span data-stu-id="b93f8-199">PKCS Certificate Template Name.</span></span>|
|<span data-ttu-id="b93f8-200">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="b93f8-200">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="b93f8-201">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b93f8-201">String</span></span>|<span data-ttu-id="b93f8-202">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="b93f8-202">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="b93f8-203">Resposta</span><span class="sxs-lookup"><span data-stu-id="b93f8-203">Response</span></span>
<span data-ttu-id="b93f8-204">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b93f8-204">If successful, this method returns a `200 OK` response code and an updated [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b93f8-205">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b93f8-205">Example</span></span>
### <a name="request"></a><span data-ttu-id="b93f8-206">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b93f8-206">Request</span></span>
<span data-ttu-id="b93f8-207">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b93f8-207">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 761

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
  "subjectNameFormat": "commonNameAsEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```

### <a name="response"></a><span data-ttu-id="b93f8-208">Resposta</span><span class="sxs-lookup"><span data-stu-id="b93f8-208">Response</span></span>
<span data-ttu-id="b93f8-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b93f8-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 933

{
  "@odata.type": "#microsoft.graph.iosPkcsCertificateProfile",
  "id": "ed0264dd-64dd-ed02-dd64-02eddd6402ed",
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
  "subjectNameFormat": "commonNameAsEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```





