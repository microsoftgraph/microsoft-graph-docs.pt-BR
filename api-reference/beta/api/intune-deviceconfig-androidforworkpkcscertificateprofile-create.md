---
title: Criar androidForWorkPkcsCertificateProfile
description: Crie um novo objeto de androidForWorkPkcsCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2718dac1c4b624983f445afa351e8e80882cb0ff
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27963847"
---
# <a name="create-androidforworkpkcscertificateprofile"></a><span data-ttu-id="6e26b-103">Criar androidForWorkPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="6e26b-103">Create androidForWorkPkcsCertificateProfile</span></span>

> <span data-ttu-id="6e26b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6e26b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6e26b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6e26b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6e26b-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="6e26b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6e26b-107">Crie um novo objeto de [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="6e26b-107">Create a new [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6e26b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6e26b-108">Prerequisites</span></span>
<span data-ttu-id="6e26b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e26b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e26b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6e26b-111">Permission type</span></span>|<span data-ttu-id="6e26b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6e26b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6e26b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6e26b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6e26b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e26b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6e26b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6e26b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6e26b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6e26b-116">Not supported.</span></span>|
|<span data-ttu-id="6e26b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6e26b-117">Application</span></span>|<span data-ttu-id="6e26b-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6e26b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6e26b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6e26b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6e26b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6e26b-120">Request headers</span></span>
|<span data-ttu-id="6e26b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6e26b-121">Header</span></span>|<span data-ttu-id="6e26b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6e26b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6e26b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6e26b-123">Authorization</span></span>|<span data-ttu-id="6e26b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6e26b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6e26b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6e26b-125">Accept</span></span>|<span data-ttu-id="6e26b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6e26b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e26b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6e26b-127">Request body</span></span>
<span data-ttu-id="6e26b-128">No corpo da solicitação, fornece uma representação JSON para o objeto androidForWorkPkcsCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="6e26b-128">In the request body, supply a JSON representation for the androidForWorkPkcsCertificateProfile object.</span></span>

<span data-ttu-id="6e26b-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o androidForWorkPkcsCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="6e26b-129">The following table shows the properties that are required when you create the androidForWorkPkcsCertificateProfile.</span></span>

|<span data-ttu-id="6e26b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6e26b-130">Property</span></span>|<span data-ttu-id="6e26b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6e26b-131">Type</span></span>|<span data-ttu-id="6e26b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e26b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e26b-133">id</span><span class="sxs-lookup"><span data-stu-id="6e26b-133">id</span></span>|<span data-ttu-id="6e26b-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6e26b-134">String</span></span>|<span data-ttu-id="6e26b-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6e26b-135">Key of the entity.</span></span> <span data-ttu-id="6e26b-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e26b-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6e26b-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6e26b-137">lastModifiedDateTime</span></span>|<span data-ttu-id="6e26b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6e26b-138">DateTimeOffset</span></span>|<span data-ttu-id="6e26b-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="6e26b-139">DateTime the object was last modified.</span></span> <span data-ttu-id="6e26b-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e26b-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6e26b-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6e26b-141">roleScopeTagIds</span></span>|<span data-ttu-id="6e26b-142">String collection</span><span class="sxs-lookup"><span data-stu-id="6e26b-142">String collection</span></span>|<span data-ttu-id="6e26b-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="6e26b-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6e26b-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e26b-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6e26b-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6e26b-145">supportsScopeTags</span></span>|<span data-ttu-id="6e26b-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="6e26b-146">Boolean</span></span>|<span data-ttu-id="6e26b-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="6e26b-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6e26b-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="6e26b-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6e26b-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="6e26b-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6e26b-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6e26b-150">This property is read-only.</span></span> <span data-ttu-id="6e26b-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e26b-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6e26b-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6e26b-152">createdDateTime</span></span>|<span data-ttu-id="6e26b-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6e26b-153">DateTimeOffset</span></span>|<span data-ttu-id="6e26b-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="6e26b-154">DateTime the object was created.</span></span> <span data-ttu-id="6e26b-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e26b-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6e26b-156">description</span><span class="sxs-lookup"><span data-stu-id="6e26b-156">description</span></span>|<span data-ttu-id="6e26b-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6e26b-157">String</span></span>|<span data-ttu-id="6e26b-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6e26b-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6e26b-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e26b-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6e26b-160">displayName</span><span class="sxs-lookup"><span data-stu-id="6e26b-160">displayName</span></span>|<span data-ttu-id="6e26b-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6e26b-161">String</span></span>|<span data-ttu-id="6e26b-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6e26b-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6e26b-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e26b-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6e26b-164">version</span><span class="sxs-lookup"><span data-stu-id="6e26b-164">version</span></span>|<span data-ttu-id="6e26b-165">Int32</span><span class="sxs-lookup"><span data-stu-id="6e26b-165">Int32</span></span>|<span data-ttu-id="6e26b-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6e26b-166">Version of the device configuration.</span></span> <span data-ttu-id="6e26b-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e26b-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6e26b-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="6e26b-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="6e26b-169">Int32</span><span class="sxs-lookup"><span data-stu-id="6e26b-169">Int32</span></span>|<span data-ttu-id="6e26b-170">Porcentagem de limite de renovação de certificados.</span><span class="sxs-lookup"><span data-stu-id="6e26b-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="6e26b-171">Válido valores de 1 a 99 Inherited de [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="6e26b-171">Valid values 1 to 99 Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="6e26b-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="6e26b-172">subjectNameFormat</span></span>|[<span data-ttu-id="6e26b-173">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="6e26b-173">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="6e26b-174">Formato de nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="6e26b-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="6e26b-175">Herdada do [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="6e26b-175">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="6e26b-176">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="6e26b-176">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="6e26b-177">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="6e26b-177">certificateValidityPeriodValue</span></span>|<span data-ttu-id="6e26b-178">Int32</span><span class="sxs-lookup"><span data-stu-id="6e26b-178">Int32</span></span>|<span data-ttu-id="6e26b-179">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="6e26b-179">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="6e26b-180">Herdado de [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="6e26b-180">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="6e26b-181">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="6e26b-181">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="6e26b-182">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="6e26b-182">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="6e26b-183">Escala para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="6e26b-183">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="6e26b-184">Herdada do [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="6e26b-184">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="6e26b-185">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="6e26b-185">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="6e26b-186">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="6e26b-186">extendedKeyUsages</span></span>|<span data-ttu-id="6e26b-187">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="6e26b-187">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="6e26b-188">Configurações de uso de chave (EKU) estendido.</span><span class="sxs-lookup"><span data-stu-id="6e26b-188">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="6e26b-189">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="6e26b-189">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="6e26b-190">Herdado de [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="6e26b-190">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="6e26b-191">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="6e26b-191">certificationAuthority</span></span>|<span data-ttu-id="6e26b-192">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6e26b-192">String</span></span>|<span data-ttu-id="6e26b-193">Autoridade de certificação PKCS</span><span class="sxs-lookup"><span data-stu-id="6e26b-193">PKCS Certification Authority</span></span>|
|<span data-ttu-id="6e26b-194">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="6e26b-194">certificationAuthorityName</span></span>|<span data-ttu-id="6e26b-195">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6e26b-195">String</span></span>|<span data-ttu-id="6e26b-196">Nome da autoridade de certificação PKCS</span><span class="sxs-lookup"><span data-stu-id="6e26b-196">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="6e26b-197">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="6e26b-197">certificateTemplateName</span></span>|<span data-ttu-id="6e26b-198">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6e26b-198">String</span></span>|<span data-ttu-id="6e26b-199">Nome do modelo de certificado PKCS</span><span class="sxs-lookup"><span data-stu-id="6e26b-199">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="6e26b-200">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="6e26b-200">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="6e26b-201">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6e26b-201">String</span></span>|<span data-ttu-id="6e26b-202">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="6e26b-202">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="6e26b-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="6e26b-203">subjectAlternativeNameType</span></span>|[<span data-ttu-id="6e26b-204">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="6e26b-204">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="6e26b-205">Tipo de nome alternativo de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="6e26b-205">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="6e26b-206">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="6e26b-206">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|



## <a name="response"></a><span data-ttu-id="6e26b-207">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e26b-207">Response</span></span>
<span data-ttu-id="6e26b-208">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6e26b-208">If successful, this method returns a `201 Created` response code and a [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e26b-209">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6e26b-209">Example</span></span>
### <a name="request"></a><span data-ttu-id="6e26b-210">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6e26b-210">Request</span></span>
<span data-ttu-id="6e26b-211">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6e26b-211">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1029

{
  "@odata.type": "#microsoft.graph.androidForWorkPkcsCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="6e26b-212">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e26b-212">Response</span></span>
<span data-ttu-id="6e26b-p117">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6e26b-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1137

{
  "@odata.type": "#microsoft.graph.androidForWorkPkcsCertificateProfile",
  "id": "0a2d7691-7691-0a2d-9176-2d0a91762d0a",
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





