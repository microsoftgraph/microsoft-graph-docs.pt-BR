---
title: Atualizar androidForWorkImportedPFXCertificateProfile
description: Atualize as propriedades de um objeto androidForWorkImportedPFXCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a41d2493aaea2347d3e8d5ba8d7d4137045b0723
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817637"
---
# <a name="update-androidforworkimportedpfxcertificateprofile"></a><span data-ttu-id="6f40c-103">Atualizar androidForWorkImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="6f40c-103">Update androidForWorkImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="6f40c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6f40c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6f40c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6f40c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6f40c-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="6f40c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6f40c-107">Atualize as propriedades de um objeto [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="6f40c-107">Update the properties of a [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6f40c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6f40c-108">Prerequisites</span></span>
<span data-ttu-id="6f40c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f40c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f40c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6f40c-111">Permission type</span></span>|<span data-ttu-id="6f40c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6f40c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f40c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6f40c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6f40c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f40c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6f40c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6f40c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f40c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6f40c-116">Not supported.</span></span>|
|<span data-ttu-id="6f40c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6f40c-117">Application</span></span>|<span data-ttu-id="6f40c-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6f40c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f40c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6f40c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="6f40c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6f40c-120">Request headers</span></span>
|<span data-ttu-id="6f40c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6f40c-121">Header</span></span>|<span data-ttu-id="6f40c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6f40c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6f40c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6f40c-123">Authorization</span></span>|<span data-ttu-id="6f40c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6f40c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6f40c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6f40c-125">Accept</span></span>|<span data-ttu-id="6f40c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6f40c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f40c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6f40c-127">Request body</span></span>
<span data-ttu-id="6f40c-128">No corpo da solicitação, fornece uma representação JSON para o objeto [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="6f40c-128">In the request body, supply a JSON representation for the [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) object.</span></span>

<span data-ttu-id="6f40c-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="6f40c-129">The following table shows the properties that are required when you create the [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md).</span></span>

|<span data-ttu-id="6f40c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6f40c-130">Property</span></span>|<span data-ttu-id="6f40c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6f40c-131">Type</span></span>|<span data-ttu-id="6f40c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f40c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f40c-133">id</span><span class="sxs-lookup"><span data-stu-id="6f40c-133">id</span></span>|<span data-ttu-id="6f40c-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6f40c-134">String</span></span>|<span data-ttu-id="6f40c-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6f40c-135">Key of the entity.</span></span> <span data-ttu-id="6f40c-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f40c-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f40c-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6f40c-137">lastModifiedDateTime</span></span>|<span data-ttu-id="6f40c-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f40c-138">DateTimeOffset</span></span>|<span data-ttu-id="6f40c-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="6f40c-139">DateTime the object was last modified.</span></span> <span data-ttu-id="6f40c-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f40c-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f40c-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6f40c-141">roleScopeTagIds</span></span>|<span data-ttu-id="6f40c-142">String collection</span><span class="sxs-lookup"><span data-stu-id="6f40c-142">String collection</span></span>|<span data-ttu-id="6f40c-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="6f40c-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6f40c-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f40c-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f40c-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6f40c-145">supportsScopeTags</span></span>|<span data-ttu-id="6f40c-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="6f40c-146">Boolean</span></span>|<span data-ttu-id="6f40c-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="6f40c-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6f40c-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="6f40c-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6f40c-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="6f40c-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6f40c-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6f40c-150">This property is read-only.</span></span> <span data-ttu-id="6f40c-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f40c-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f40c-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6f40c-152">createdDateTime</span></span>|<span data-ttu-id="6f40c-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f40c-153">DateTimeOffset</span></span>|<span data-ttu-id="6f40c-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="6f40c-154">DateTime the object was created.</span></span> <span data-ttu-id="6f40c-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f40c-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f40c-156">description</span><span class="sxs-lookup"><span data-stu-id="6f40c-156">description</span></span>|<span data-ttu-id="6f40c-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6f40c-157">String</span></span>|<span data-ttu-id="6f40c-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6f40c-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6f40c-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f40c-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f40c-160">displayName</span><span class="sxs-lookup"><span data-stu-id="6f40c-160">displayName</span></span>|<span data-ttu-id="6f40c-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6f40c-161">String</span></span>|<span data-ttu-id="6f40c-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6f40c-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6f40c-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f40c-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f40c-164">version</span><span class="sxs-lookup"><span data-stu-id="6f40c-164">version</span></span>|<span data-ttu-id="6f40c-165">Int32</span><span class="sxs-lookup"><span data-stu-id="6f40c-165">Int32</span></span>|<span data-ttu-id="6f40c-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6f40c-166">Version of the device configuration.</span></span> <span data-ttu-id="6f40c-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f40c-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f40c-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="6f40c-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="6f40c-169">Int32</span><span class="sxs-lookup"><span data-stu-id="6f40c-169">Int32</span></span>|<span data-ttu-id="6f40c-170">Porcentagem de limite de renovação de certificados.</span><span class="sxs-lookup"><span data-stu-id="6f40c-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="6f40c-171">Válido valores de 1 a 99 Inherited de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="6f40c-171">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="6f40c-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="6f40c-172">subjectNameFormat</span></span>|[<span data-ttu-id="6f40c-173">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="6f40c-173">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="6f40c-174">Formato de nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="6f40c-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="6f40c-175">Herdada do [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="6f40c-175">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="6f40c-176">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="6f40c-176">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="6f40c-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="6f40c-177">subjectAlternativeNameType</span></span>|[<span data-ttu-id="6f40c-178">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="6f40c-178">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="6f40c-179">Tipo de nome alternativo de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="6f40c-179">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="6f40c-180">Herdada do [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="6f40c-180">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="6f40c-181">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="6f40c-181">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="6f40c-182">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="6f40c-182">certificateValidityPeriodValue</span></span>|<span data-ttu-id="6f40c-183">Int32</span><span class="sxs-lookup"><span data-stu-id="6f40c-183">Int32</span></span>|<span data-ttu-id="6f40c-184">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="6f40c-184">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="6f40c-185">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="6f40c-185">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="6f40c-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="6f40c-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="6f40c-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="6f40c-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="6f40c-188">Escala para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="6f40c-188">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="6f40c-189">Herdada do [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="6f40c-189">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="6f40c-190">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="6f40c-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="6f40c-191">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="6f40c-191">extendedKeyUsages</span></span>|<span data-ttu-id="6f40c-192">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="6f40c-192">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="6f40c-193">Configurações de uso de chave (EKU) estendido.</span><span class="sxs-lookup"><span data-stu-id="6f40c-193">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="6f40c-194">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="6f40c-194">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="6f40c-195">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="6f40c-195">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="6f40c-196">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="6f40c-196">intendedPurpose</span></span>|[<span data-ttu-id="6f40c-197">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="6f40c-197">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="6f40c-198">Ainda não documentado.</span><span class="sxs-lookup"><span data-stu-id="6f40c-198">Not yet documented.</span></span> <span data-ttu-id="6f40c-199">Os valores possíveis são: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span><span class="sxs-lookup"><span data-stu-id="6f40c-199">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="6f40c-200">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f40c-200">Response</span></span>
<span data-ttu-id="6f40c-201">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6f40c-201">If successful, this method returns a `200 OK` response code and an updated [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f40c-202">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6f40c-202">Example</span></span>
### <a name="request"></a><span data-ttu-id="6f40c-203">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6f40c-203">Request</span></span>
<span data-ttu-id="6f40c-204">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6f40c-204">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 708

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
  "intendedPurpose": "smimeEncryption"
}
```

### <a name="response"></a><span data-ttu-id="6f40c-205">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f40c-205">Response</span></span>
<span data-ttu-id="6f40c-p118">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6f40c-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 898

{
  "@odata.type": "#microsoft.graph.androidForWorkImportedPFXCertificateProfile",
  "id": "a0bfd7bc-d7bc-a0bf-bcd7-bfa0bcd7bfa0",
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
  "intendedPurpose": "smimeEncryption"
}
```





