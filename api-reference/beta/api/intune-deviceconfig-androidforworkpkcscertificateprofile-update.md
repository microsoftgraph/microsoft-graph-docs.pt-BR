---
title: Atualizar androidForWorkPkcsCertificateProfile
description: Atualize as propriedades de um objeto androidForWorkPkcsCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 28f2b67f858b95b934c8578f34565e20a4d79d59
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27887168"
---
# <a name="update-androidforworkpkcscertificateprofile"></a><span data-ttu-id="dbb18-103">Atualizar androidForWorkPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="dbb18-103">Update androidForWorkPkcsCertificateProfile</span></span>

> <span data-ttu-id="dbb18-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="dbb18-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dbb18-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="dbb18-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dbb18-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="dbb18-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dbb18-107">Atualize as propriedades de um objeto [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="dbb18-107">Update the properties of a [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="dbb18-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dbb18-108">Prerequisites</span></span>
<span data-ttu-id="dbb18-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dbb18-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dbb18-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dbb18-111">Permission type</span></span>|<span data-ttu-id="dbb18-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="dbb18-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dbb18-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dbb18-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dbb18-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dbb18-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dbb18-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dbb18-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dbb18-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dbb18-116">Not supported.</span></span>|
|<span data-ttu-id="dbb18-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dbb18-117">Application</span></span>|<span data-ttu-id="dbb18-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dbb18-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dbb18-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dbb18-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="dbb18-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dbb18-120">Request headers</span></span>
|<span data-ttu-id="dbb18-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dbb18-121">Header</span></span>|<span data-ttu-id="dbb18-122">Valor</span><span class="sxs-lookup"><span data-stu-id="dbb18-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dbb18-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="dbb18-123">Authorization</span></span>|<span data-ttu-id="dbb18-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dbb18-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dbb18-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dbb18-125">Accept</span></span>|<span data-ttu-id="dbb18-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dbb18-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dbb18-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dbb18-127">Request body</span></span>
<span data-ttu-id="dbb18-128">No corpo da solicitação, fornece uma representação JSON para o objeto [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="dbb18-128">In the request body, supply a JSON representation for the [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) object.</span></span>

<span data-ttu-id="dbb18-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="dbb18-129">The following table shows the properties that are required when you create the [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md).</span></span>

|<span data-ttu-id="dbb18-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dbb18-130">Property</span></span>|<span data-ttu-id="dbb18-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="dbb18-131">Type</span></span>|<span data-ttu-id="dbb18-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="dbb18-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dbb18-133">id</span><span class="sxs-lookup"><span data-stu-id="dbb18-133">id</span></span>|<span data-ttu-id="dbb18-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dbb18-134">String</span></span>|<span data-ttu-id="dbb18-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="dbb18-135">Key of the entity.</span></span> <span data-ttu-id="dbb18-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dbb18-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dbb18-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dbb18-137">lastModifiedDateTime</span></span>|<span data-ttu-id="dbb18-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dbb18-138">DateTimeOffset</span></span>|<span data-ttu-id="dbb18-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="dbb18-139">DateTime the object was last modified.</span></span> <span data-ttu-id="dbb18-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dbb18-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dbb18-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="dbb18-141">roleScopeTagIds</span></span>|<span data-ttu-id="dbb18-142">String collection</span><span class="sxs-lookup"><span data-stu-id="dbb18-142">String collection</span></span>|<span data-ttu-id="dbb18-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="dbb18-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="dbb18-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dbb18-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dbb18-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="dbb18-145">supportsScopeTags</span></span>|<span data-ttu-id="dbb18-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="dbb18-146">Boolean</span></span>|<span data-ttu-id="dbb18-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="dbb18-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="dbb18-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="dbb18-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="dbb18-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="dbb18-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="dbb18-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dbb18-150">This property is read-only.</span></span> <span data-ttu-id="dbb18-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dbb18-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dbb18-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dbb18-152">createdDateTime</span></span>|<span data-ttu-id="dbb18-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dbb18-153">DateTimeOffset</span></span>|<span data-ttu-id="dbb18-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="dbb18-154">DateTime the object was created.</span></span> <span data-ttu-id="dbb18-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dbb18-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dbb18-156">description</span><span class="sxs-lookup"><span data-stu-id="dbb18-156">description</span></span>|<span data-ttu-id="dbb18-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dbb18-157">String</span></span>|<span data-ttu-id="dbb18-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="dbb18-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="dbb18-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dbb18-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dbb18-160">displayName</span><span class="sxs-lookup"><span data-stu-id="dbb18-160">displayName</span></span>|<span data-ttu-id="dbb18-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dbb18-161">String</span></span>|<span data-ttu-id="dbb18-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="dbb18-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="dbb18-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dbb18-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dbb18-164">version</span><span class="sxs-lookup"><span data-stu-id="dbb18-164">version</span></span>|<span data-ttu-id="dbb18-165">Int32</span><span class="sxs-lookup"><span data-stu-id="dbb18-165">Int32</span></span>|<span data-ttu-id="dbb18-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="dbb18-166">Version of the device configuration.</span></span> <span data-ttu-id="dbb18-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dbb18-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dbb18-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="dbb18-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="dbb18-169">Int32</span><span class="sxs-lookup"><span data-stu-id="dbb18-169">Int32</span></span>|<span data-ttu-id="dbb18-170">Porcentagem de limite de renovação de certificados.</span><span class="sxs-lookup"><span data-stu-id="dbb18-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="dbb18-171">Válido valores de 1 a 99 Inherited de [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="dbb18-171">Valid values 1 to 99 Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="dbb18-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="dbb18-172">subjectNameFormat</span></span>|[<span data-ttu-id="dbb18-173">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="dbb18-173">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="dbb18-174">Formato de nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="dbb18-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="dbb18-175">Herdada do [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="dbb18-175">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="dbb18-176">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="dbb18-176">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="dbb18-177">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="dbb18-177">certificateValidityPeriodValue</span></span>|<span data-ttu-id="dbb18-178">Int32</span><span class="sxs-lookup"><span data-stu-id="dbb18-178">Int32</span></span>|<span data-ttu-id="dbb18-179">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="dbb18-179">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="dbb18-180">Herdado de [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="dbb18-180">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="dbb18-181">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="dbb18-181">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="dbb18-182">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="dbb18-182">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="dbb18-183">Escala para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="dbb18-183">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="dbb18-184">Herdada do [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="dbb18-184">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="dbb18-185">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="dbb18-185">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="dbb18-186">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="dbb18-186">extendedKeyUsages</span></span>|<span data-ttu-id="dbb18-187">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="dbb18-187">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="dbb18-188">Configurações de uso de chave (EKU) estendido.</span><span class="sxs-lookup"><span data-stu-id="dbb18-188">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="dbb18-189">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="dbb18-189">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="dbb18-190">Herdado de [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="dbb18-190">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="dbb18-191">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="dbb18-191">certificationAuthority</span></span>|<span data-ttu-id="dbb18-192">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dbb18-192">String</span></span>|<span data-ttu-id="dbb18-193">Autoridade de certificação PKCS</span><span class="sxs-lookup"><span data-stu-id="dbb18-193">PKCS Certification Authority</span></span>|
|<span data-ttu-id="dbb18-194">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="dbb18-194">certificationAuthorityName</span></span>|<span data-ttu-id="dbb18-195">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dbb18-195">String</span></span>|<span data-ttu-id="dbb18-196">Nome da autoridade de certificação PKCS</span><span class="sxs-lookup"><span data-stu-id="dbb18-196">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="dbb18-197">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="dbb18-197">certificateTemplateName</span></span>|<span data-ttu-id="dbb18-198">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dbb18-198">String</span></span>|<span data-ttu-id="dbb18-199">Nome do modelo de certificado PKCS</span><span class="sxs-lookup"><span data-stu-id="dbb18-199">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="dbb18-200">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="dbb18-200">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="dbb18-201">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dbb18-201">String</span></span>|<span data-ttu-id="dbb18-202">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="dbb18-202">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="dbb18-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="dbb18-203">subjectAlternativeNameType</span></span>|[<span data-ttu-id="dbb18-204">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="dbb18-204">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="dbb18-205">Tipo de nome alternativo de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="dbb18-205">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="dbb18-206">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="dbb18-206">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|



## <a name="response"></a><span data-ttu-id="dbb18-207">Resposta</span><span class="sxs-lookup"><span data-stu-id="dbb18-207">Response</span></span>
<span data-ttu-id="dbb18-208">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dbb18-208">If successful, this method returns a `200 OK` response code and an updated [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dbb18-209">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dbb18-209">Example</span></span>
### <a name="request"></a><span data-ttu-id="dbb18-210">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dbb18-210">Request</span></span>
<span data-ttu-id="dbb18-211">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dbb18-211">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="dbb18-212">Resposta</span><span class="sxs-lookup"><span data-stu-id="dbb18-212">Response</span></span>
<span data-ttu-id="dbb18-p117">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dbb18-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





