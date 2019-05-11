---
title: Atualizar windows10ImportedPFXCertificateProfile
description: Atualiza as propriedades de um objeto windows10ImportedPFXCertificateProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 271076658b8feb56ef9e0f168f1dfe18fe5533de
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33918644"
---
# <a name="update-windows10importedpfxcertificateprofile"></a><span data-ttu-id="c96ee-103">Atualizar windows10ImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="c96ee-103">Update windows10ImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="c96ee-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c96ee-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c96ee-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c96ee-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c96ee-106">Atualiza as propriedades de um objeto [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="c96ee-106">Update the properties of a [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c96ee-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c96ee-107">Prerequisites</span></span>
<span data-ttu-id="c96ee-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c96ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c96ee-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c96ee-110">Permission type</span></span>|<span data-ttu-id="c96ee-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c96ee-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c96ee-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c96ee-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c96ee-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c96ee-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c96ee-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c96ee-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c96ee-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c96ee-115">Not supported.</span></span>|
|<span data-ttu-id="c96ee-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c96ee-116">Application</span></span>|<span data-ttu-id="c96ee-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c96ee-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c96ee-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c96ee-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="c96ee-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c96ee-119">Request headers</span></span>
|<span data-ttu-id="c96ee-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c96ee-120">Header</span></span>|<span data-ttu-id="c96ee-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c96ee-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c96ee-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c96ee-122">Authorization</span></span>|<span data-ttu-id="c96ee-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c96ee-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c96ee-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c96ee-124">Accept</span></span>|<span data-ttu-id="c96ee-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c96ee-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c96ee-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c96ee-126">Request body</span></span>
<span data-ttu-id="c96ee-127">No corpo da solicitação, forneça uma representação JSON do objeto [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="c96ee-127">In the request body, supply a JSON representation for the [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) object.</span></span>

<span data-ttu-id="c96ee-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="c96ee-128">The following table shows the properties that are required when you create the [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md).</span></span>

|<span data-ttu-id="c96ee-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c96ee-129">Property</span></span>|<span data-ttu-id="c96ee-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="c96ee-130">Type</span></span>|<span data-ttu-id="c96ee-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="c96ee-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c96ee-132">id</span><span class="sxs-lookup"><span data-stu-id="c96ee-132">id</span></span>|<span data-ttu-id="c96ee-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c96ee-133">String</span></span>|<span data-ttu-id="c96ee-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c96ee-134">Key of the entity.</span></span> <span data-ttu-id="c96ee-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c96ee-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c96ee-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c96ee-136">lastModifiedDateTime</span></span>|<span data-ttu-id="c96ee-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c96ee-137">DateTimeOffset</span></span>|<span data-ttu-id="c96ee-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="c96ee-138">DateTime the object was last modified.</span></span> <span data-ttu-id="c96ee-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c96ee-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c96ee-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c96ee-140">roleScopeTagIds</span></span>|<span data-ttu-id="c96ee-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c96ee-141">String collection</span></span>|<span data-ttu-id="c96ee-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="c96ee-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c96ee-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c96ee-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c96ee-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c96ee-144">supportsScopeTags</span></span>|<span data-ttu-id="c96ee-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="c96ee-145">Boolean</span></span>|<span data-ttu-id="c96ee-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="c96ee-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c96ee-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="c96ee-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c96ee-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="c96ee-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c96ee-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c96ee-149">This property is read-only.</span></span> <span data-ttu-id="c96ee-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c96ee-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c96ee-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c96ee-151">createdDateTime</span></span>|<span data-ttu-id="c96ee-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c96ee-152">DateTimeOffset</span></span>|<span data-ttu-id="c96ee-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="c96ee-153">DateTime the object was created.</span></span> <span data-ttu-id="c96ee-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c96ee-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c96ee-155">description</span><span class="sxs-lookup"><span data-stu-id="c96ee-155">description</span></span>|<span data-ttu-id="c96ee-156">String</span><span class="sxs-lookup"><span data-stu-id="c96ee-156">String</span></span>|<span data-ttu-id="c96ee-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c96ee-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c96ee-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c96ee-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c96ee-159">displayName</span><span class="sxs-lookup"><span data-stu-id="c96ee-159">displayName</span></span>|<span data-ttu-id="c96ee-160">String</span><span class="sxs-lookup"><span data-stu-id="c96ee-160">String</span></span>|<span data-ttu-id="c96ee-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c96ee-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c96ee-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c96ee-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c96ee-163">versão</span><span class="sxs-lookup"><span data-stu-id="c96ee-163">version</span></span>|<span data-ttu-id="c96ee-164">Int32</span><span class="sxs-lookup"><span data-stu-id="c96ee-164">Int32</span></span>|<span data-ttu-id="c96ee-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c96ee-165">Version of the device configuration.</span></span> <span data-ttu-id="c96ee-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c96ee-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c96ee-167">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="c96ee-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="c96ee-168">Int32</span><span class="sxs-lookup"><span data-stu-id="c96ee-168">Int32</span></span>|<span data-ttu-id="c96ee-169">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="c96ee-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="c96ee-170">Valores válidos de 1 a 99 herdados de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="c96ee-170">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="c96ee-171">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="c96ee-171">keyStorageProvider</span></span>|[<span data-ttu-id="c96ee-172">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="c96ee-172">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="c96ee-173">Provedor de armazenamento de chave (KSP) herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="c96ee-173">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="c96ee-174">Os valores possíveis são: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="c96ee-174">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="c96ee-175">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="c96ee-175">subjectNameFormat</span></span>|[<span data-ttu-id="c96ee-176">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="c96ee-176">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="c96ee-177">Formato do nome de entidade do certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="c96ee-177">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="c96ee-178">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="c96ee-178">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="c96ee-179">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="c96ee-179">subjectAlternativeNameType</span></span>|[<span data-ttu-id="c96ee-180">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="c96ee-180">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="c96ee-181">Tipo de nome alternativo de entidade do certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="c96ee-181">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="c96ee-182">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="c96ee-182">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="c96ee-183">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="c96ee-183">certificateValidityPeriodValue</span></span>|<span data-ttu-id="c96ee-184">Int32</span><span class="sxs-lookup"><span data-stu-id="c96ee-184">Int32</span></span>|<span data-ttu-id="c96ee-185">Valor para o período de validade do certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="c96ee-185">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="c96ee-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="c96ee-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="c96ee-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="c96ee-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="c96ee-188">Dimensionar o período de validade do certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="c96ee-188">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="c96ee-189">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="c96ee-189">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="c96ee-190">Da intendedpurpose</span><span class="sxs-lookup"><span data-stu-id="c96ee-190">intendedPurpose</span></span>|[<span data-ttu-id="c96ee-191">Da intendedpurpose</span><span class="sxs-lookup"><span data-stu-id="c96ee-191">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="c96ee-192">Ainda não documentado.</span><span class="sxs-lookup"><span data-stu-id="c96ee-192">Not yet documented.</span></span> <span data-ttu-id="c96ee-193">Os valores possíveis são: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span><span class="sxs-lookup"><span data-stu-id="c96ee-193">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="c96ee-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="c96ee-194">Response</span></span>
<span data-ttu-id="c96ee-195">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c96ee-195">If successful, this method returns a `200 OK` response code and an updated [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c96ee-196">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c96ee-196">Example</span></span>

### <a name="request"></a><span data-ttu-id="c96ee-197">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c96ee-197">Request</span></span>
<span data-ttu-id="c96ee-198">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c96ee-198">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 586

{
  "@odata.type": "#microsoft.graph.windows10ImportedPFXCertificateProfile",
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
  "intendedPurpose": "smimeEncryption"
}
```

### <a name="response"></a><span data-ttu-id="c96ee-199">Resposta</span><span class="sxs-lookup"><span data-stu-id="c96ee-199">Response</span></span>
<span data-ttu-id="c96ee-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c96ee-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 758

{
  "@odata.type": "#microsoft.graph.windows10ImportedPFXCertificateProfile",
  "id": "b582514b-514b-b582-4b51-82b54b5182b5",
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
  "intendedPurpose": "smimeEncryption"
}
```




