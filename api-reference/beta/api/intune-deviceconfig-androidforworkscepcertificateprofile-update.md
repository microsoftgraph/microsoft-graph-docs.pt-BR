---
title: Atualizar androidForWorkScepCertificateProfile
description: Atualize as propriedades de um objeto androidForWorkScepCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a0cb546566584408d2428c05a3d5326aaebda67f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27879342"
---
# <a name="update-androidforworkscepcertificateprofile"></a><span data-ttu-id="685a8-103">Atualizar androidForWorkScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="685a8-103">Update androidForWorkScepCertificateProfile</span></span>

> <span data-ttu-id="685a8-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="685a8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="685a8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="685a8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="685a8-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="685a8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="685a8-107">Atualize as propriedades de um objeto [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="685a8-107">Update the properties of a [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="685a8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="685a8-108">Prerequisites</span></span>
<span data-ttu-id="685a8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="685a8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="685a8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="685a8-111">Permission type</span></span>|<span data-ttu-id="685a8-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="685a8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="685a8-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="685a8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="685a8-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="685a8-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="685a8-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="685a8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="685a8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="685a8-116">Not supported.</span></span>|
|<span data-ttu-id="685a8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="685a8-117">Application</span></span>|<span data-ttu-id="685a8-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="685a8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="685a8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="685a8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="685a8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="685a8-120">Request headers</span></span>
|<span data-ttu-id="685a8-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="685a8-121">Header</span></span>|<span data-ttu-id="685a8-122">Valor</span><span class="sxs-lookup"><span data-stu-id="685a8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="685a8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="685a8-123">Authorization</span></span>|<span data-ttu-id="685a8-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="685a8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="685a8-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="685a8-125">Accept</span></span>|<span data-ttu-id="685a8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="685a8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="685a8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="685a8-127">Request body</span></span>
<span data-ttu-id="685a8-128">No corpo da solicitação, fornece uma representação JSON para o objeto [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="685a8-128">In the request body, supply a JSON representation for the [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) object.</span></span>

<span data-ttu-id="685a8-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="685a8-129">The following table shows the properties that are required when you create the [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md).</span></span>

|<span data-ttu-id="685a8-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="685a8-130">Property</span></span>|<span data-ttu-id="685a8-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="685a8-131">Type</span></span>|<span data-ttu-id="685a8-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="685a8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="685a8-133">id</span><span class="sxs-lookup"><span data-stu-id="685a8-133">id</span></span>|<span data-ttu-id="685a8-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="685a8-134">String</span></span>|<span data-ttu-id="685a8-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="685a8-135">Key of the entity.</span></span> <span data-ttu-id="685a8-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="685a8-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="685a8-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="685a8-137">lastModifiedDateTime</span></span>|<span data-ttu-id="685a8-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="685a8-138">DateTimeOffset</span></span>|<span data-ttu-id="685a8-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="685a8-139">DateTime the object was last modified.</span></span> <span data-ttu-id="685a8-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="685a8-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="685a8-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="685a8-141">roleScopeTagIds</span></span>|<span data-ttu-id="685a8-142">String collection</span><span class="sxs-lookup"><span data-stu-id="685a8-142">String collection</span></span>|<span data-ttu-id="685a8-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="685a8-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="685a8-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="685a8-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="685a8-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="685a8-145">supportsScopeTags</span></span>|<span data-ttu-id="685a8-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="685a8-146">Boolean</span></span>|<span data-ttu-id="685a8-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="685a8-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="685a8-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="685a8-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="685a8-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="685a8-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="685a8-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="685a8-150">This property is read-only.</span></span> <span data-ttu-id="685a8-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="685a8-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="685a8-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="685a8-152">createdDateTime</span></span>|<span data-ttu-id="685a8-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="685a8-153">DateTimeOffset</span></span>|<span data-ttu-id="685a8-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="685a8-154">DateTime the object was created.</span></span> <span data-ttu-id="685a8-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="685a8-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="685a8-156">description</span><span class="sxs-lookup"><span data-stu-id="685a8-156">description</span></span>|<span data-ttu-id="685a8-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="685a8-157">String</span></span>|<span data-ttu-id="685a8-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="685a8-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="685a8-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="685a8-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="685a8-160">displayName</span><span class="sxs-lookup"><span data-stu-id="685a8-160">displayName</span></span>|<span data-ttu-id="685a8-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="685a8-161">String</span></span>|<span data-ttu-id="685a8-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="685a8-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="685a8-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="685a8-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="685a8-164">version</span><span class="sxs-lookup"><span data-stu-id="685a8-164">version</span></span>|<span data-ttu-id="685a8-165">Int32</span><span class="sxs-lookup"><span data-stu-id="685a8-165">Int32</span></span>|<span data-ttu-id="685a8-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="685a8-166">Version of the device configuration.</span></span> <span data-ttu-id="685a8-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="685a8-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="685a8-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="685a8-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="685a8-169">Int32</span><span class="sxs-lookup"><span data-stu-id="685a8-169">Int32</span></span>|<span data-ttu-id="685a8-170">Porcentagem de limite de renovação de certificados.</span><span class="sxs-lookup"><span data-stu-id="685a8-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="685a8-171">Válido valores de 1 a 99 Inherited de [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="685a8-171">Valid values 1 to 99 Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="685a8-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="685a8-172">subjectNameFormat</span></span>|[<span data-ttu-id="685a8-173">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="685a8-173">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="685a8-174">Formato de nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="685a8-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="685a8-175">Herdada do [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="685a8-175">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="685a8-176">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="685a8-176">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="685a8-177">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="685a8-177">certificateValidityPeriodValue</span></span>|<span data-ttu-id="685a8-178">Int32</span><span class="sxs-lookup"><span data-stu-id="685a8-178">Int32</span></span>|<span data-ttu-id="685a8-179">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="685a8-179">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="685a8-180">Herdado de [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="685a8-180">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="685a8-181">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="685a8-181">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="685a8-182">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="685a8-182">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="685a8-183">Escala para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="685a8-183">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="685a8-184">Herdada do [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="685a8-184">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="685a8-185">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="685a8-185">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="685a8-186">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="685a8-186">extendedKeyUsages</span></span>|<span data-ttu-id="685a8-187">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="685a8-187">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="685a8-188">Configurações de uso de chave (EKU) estendido.</span><span class="sxs-lookup"><span data-stu-id="685a8-188">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="685a8-189">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="685a8-189">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="685a8-190">Herdado de [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="685a8-190">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="685a8-191">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="685a8-191">scepServerUrls</span></span>|<span data-ttu-id="685a8-192">String collection</span><span class="sxs-lookup"><span data-stu-id="685a8-192">String collection</span></span>|<span data-ttu-id="685a8-193">URL de servidor SCEP (s)</span><span class="sxs-lookup"><span data-stu-id="685a8-193">SCEP Server Url(s)</span></span>|
|<span data-ttu-id="685a8-194">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="685a8-194">subjectNameFormatString</span></span>|<span data-ttu-id="685a8-195">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="685a8-195">String</span></span>|<span data-ttu-id="685a8-196">Um formato personalizado a ser usada com SubjectNameFormat = personalizado.</span><span class="sxs-lookup"><span data-stu-id="685a8-196">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="685a8-197">Exemplo: CN = {{EmailAddress}}, F = {{EmailAddress}}, OU = usuários do Enterprise, O = Contoso Corporation, L = Redmond, ST = WA, C = US</span><span class="sxs-lookup"><span data-stu-id="685a8-197">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="685a8-198">keyUsage</span><span class="sxs-lookup"><span data-stu-id="685a8-198">keyUsage</span></span>|[<span data-ttu-id="685a8-199">keyUsages</span><span class="sxs-lookup"><span data-stu-id="685a8-199">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="685a8-200">Uso de chave SCEP.</span><span class="sxs-lookup"><span data-stu-id="685a8-200">SCEP Key Usage.</span></span> <span data-ttu-id="685a8-201">Os valores possíveis são: `keyEncipherment` e `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="685a8-201">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="685a8-202">keySize</span><span class="sxs-lookup"><span data-stu-id="685a8-202">keySize</span></span>|[<span data-ttu-id="685a8-203">keySize</span><span class="sxs-lookup"><span data-stu-id="685a8-203">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="685a8-204">Tamanho da chave SCEP.</span><span class="sxs-lookup"><span data-stu-id="685a8-204">SCEP Key Size.</span></span> <span data-ttu-id="685a8-205">Os valores possíveis são: `size1024` e `size2048`.</span><span class="sxs-lookup"><span data-stu-id="685a8-205">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="685a8-206">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="685a8-206">hashAlgorithm</span></span>|[<span data-ttu-id="685a8-207">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="685a8-207">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="685a8-208">Algoritmo de Hash SCEP.</span><span class="sxs-lookup"><span data-stu-id="685a8-208">SCEP Hash Algorithm.</span></span> <span data-ttu-id="685a8-209">Os valores possíveis são: `sha1` e `sha2`.</span><span class="sxs-lookup"><span data-stu-id="685a8-209">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="685a8-210">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="685a8-210">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="685a8-211">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="685a8-211">String</span></span>|<span data-ttu-id="685a8-212">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="685a8-212">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="685a8-213">certificateStore</span><span class="sxs-lookup"><span data-stu-id="685a8-213">certificateStore</span></span>|[<span data-ttu-id="685a8-214">certificateStore</span><span class="sxs-lookup"><span data-stu-id="685a8-214">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="685a8-215">Certificado do repositório de destino.</span><span class="sxs-lookup"><span data-stu-id="685a8-215">Target store certificate.</span></span> <span data-ttu-id="685a8-216">Os valores possíveis são: `user` e `machine`.</span><span class="sxs-lookup"><span data-stu-id="685a8-216">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="685a8-217">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="685a8-217">customSubjectAlternativeNames</span></span>|<span data-ttu-id="685a8-218">coleção [customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="685a8-218">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="685a8-219">Configurações de Alterantive nome de entidade personalizada.</span><span class="sxs-lookup"><span data-stu-id="685a8-219">Custom Subject Alterantive Name Settings.</span></span> <span data-ttu-id="685a8-220">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="685a8-220">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="685a8-221">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="685a8-221">subjectAlternativeNameType</span></span>|[<span data-ttu-id="685a8-222">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="685a8-222">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="685a8-223">Tipo de nome alternativo de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="685a8-223">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="685a8-224">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="685a8-224">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|



## <a name="response"></a><span data-ttu-id="685a8-225">Resposta</span><span class="sxs-lookup"><span data-stu-id="685a8-225">Response</span></span>
<span data-ttu-id="685a8-226">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="685a8-226">If successful, this method returns a `200 OK` response code and an updated [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="685a8-227">Exemplo</span><span class="sxs-lookup"><span data-stu-id="685a8-227">Example</span></span>
### <a name="request"></a><span data-ttu-id="685a8-228">Solicitação</span><span class="sxs-lookup"><span data-stu-id="685a8-228">Request</span></span>
<span data-ttu-id="685a8-229">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="685a8-229">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1194

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
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "certificateStore": "machine",
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
    }
  ],
  "subjectAlternativeNameType": "emailAddress"
}
```

### <a name="response"></a><span data-ttu-id="685a8-230">Resposta</span><span class="sxs-lookup"><span data-stu-id="685a8-230">Response</span></span>
<span data-ttu-id="685a8-p123">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="685a8-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1377

{
  "@odata.type": "#microsoft.graph.androidForWorkScepCertificateProfile",
  "id": "09e532af-32af-09e5-af32-e509af32e509",
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
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "certificateStore": "machine",
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
    }
  ],
  "subjectAlternativeNameType": "emailAddress"
}
```





