---
title: Atualizar windowsPhone81ImportedPFXCertificateProfile
description: Atualiza as propriedades de um objeto windowsPhone81ImportedPFXCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ae9e269414ace147a56a3cf955eb5d4228b6ccd1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32512590"
---
# <a name="update-windowsphone81importedpfxcertificateprofile"></a><span data-ttu-id="5ee69-103">Atualizar windowsPhone81ImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="5ee69-103">Update windowsPhone81ImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="5ee69-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5ee69-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5ee69-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5ee69-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ee69-106">Atualiza as propriedades de um objeto [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="5ee69-106">Update the properties of a [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5ee69-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5ee69-107">Prerequisites</span></span>
<span data-ttu-id="5ee69-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ee69-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ee69-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5ee69-110">Permission type</span></span>|<span data-ttu-id="5ee69-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5ee69-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5ee69-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5ee69-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5ee69-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ee69-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5ee69-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5ee69-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5ee69-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ee69-115">Not supported.</span></span>|
|<span data-ttu-id="5ee69-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5ee69-116">Application</span></span>|<span data-ttu-id="5ee69-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ee69-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5ee69-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5ee69-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="5ee69-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5ee69-119">Request headers</span></span>
|<span data-ttu-id="5ee69-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5ee69-120">Header</span></span>|<span data-ttu-id="5ee69-121">Valor</span><span class="sxs-lookup"><span data-stu-id="5ee69-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5ee69-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5ee69-122">Authorization</span></span>|<span data-ttu-id="5ee69-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5ee69-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5ee69-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5ee69-124">Accept</span></span>|<span data-ttu-id="5ee69-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5ee69-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ee69-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5ee69-126">Request body</span></span>
<span data-ttu-id="5ee69-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="5ee69-127">In the request body, supply a JSON representation for the [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) object.</span></span>

<span data-ttu-id="5ee69-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="5ee69-128">The following table shows the properties that are required when you create the [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md).</span></span>

|<span data-ttu-id="5ee69-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5ee69-129">Property</span></span>|<span data-ttu-id="5ee69-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="5ee69-130">Type</span></span>|<span data-ttu-id="5ee69-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ee69-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ee69-132">id</span><span class="sxs-lookup"><span data-stu-id="5ee69-132">id</span></span>|<span data-ttu-id="5ee69-133">String</span><span class="sxs-lookup"><span data-stu-id="5ee69-133">String</span></span>|<span data-ttu-id="5ee69-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="5ee69-134">Key of the entity.</span></span> <span data-ttu-id="5ee69-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ee69-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ee69-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5ee69-136">lastModifiedDateTime</span></span>|<span data-ttu-id="5ee69-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ee69-137">DateTimeOffset</span></span>|<span data-ttu-id="5ee69-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="5ee69-138">DateTime the object was last modified.</span></span> <span data-ttu-id="5ee69-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ee69-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ee69-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5ee69-140">roleScopeTagIds</span></span>|<span data-ttu-id="5ee69-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="5ee69-141">String collection</span></span>|<span data-ttu-id="5ee69-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="5ee69-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="5ee69-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ee69-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ee69-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="5ee69-144">supportsScopeTags</span></span>|<span data-ttu-id="5ee69-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="5ee69-145">Boolean</span></span>|<span data-ttu-id="5ee69-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="5ee69-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="5ee69-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="5ee69-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="5ee69-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="5ee69-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="5ee69-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5ee69-149">This property is read-only.</span></span> <span data-ttu-id="5ee69-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ee69-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ee69-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5ee69-151">createdDateTime</span></span>|<span data-ttu-id="5ee69-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ee69-152">DateTimeOffset</span></span>|<span data-ttu-id="5ee69-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="5ee69-153">DateTime the object was created.</span></span> <span data-ttu-id="5ee69-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ee69-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ee69-155">description</span><span class="sxs-lookup"><span data-stu-id="5ee69-155">description</span></span>|<span data-ttu-id="5ee69-156">String</span><span class="sxs-lookup"><span data-stu-id="5ee69-156">String</span></span>|<span data-ttu-id="5ee69-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5ee69-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5ee69-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ee69-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ee69-159">displayName</span><span class="sxs-lookup"><span data-stu-id="5ee69-159">displayName</span></span>|<span data-ttu-id="5ee69-160">String</span><span class="sxs-lookup"><span data-stu-id="5ee69-160">String</span></span>|<span data-ttu-id="5ee69-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5ee69-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5ee69-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ee69-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ee69-163">versão</span><span class="sxs-lookup"><span data-stu-id="5ee69-163">version</span></span>|<span data-ttu-id="5ee69-164">Int32</span><span class="sxs-lookup"><span data-stu-id="5ee69-164">Int32</span></span>|<span data-ttu-id="5ee69-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5ee69-165">Version of the device configuration.</span></span> <span data-ttu-id="5ee69-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ee69-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ee69-167">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="5ee69-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="5ee69-168">Int32</span><span class="sxs-lookup"><span data-stu-id="5ee69-168">Int32</span></span>|<span data-ttu-id="5ee69-169">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="5ee69-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="5ee69-170">Valores válidos de 1 a 99 herdados de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="5ee69-170">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="5ee69-171">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="5ee69-171">keyStorageProvider</span></span>|[<span data-ttu-id="5ee69-172">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="5ee69-172">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="5ee69-173">Provedor de armazenamento de chave (KSP) herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="5ee69-173">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="5ee69-174">Os valores possíveis são: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="5ee69-174">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="5ee69-175">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="5ee69-175">subjectNameFormat</span></span>|[<span data-ttu-id="5ee69-176">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="5ee69-176">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="5ee69-177">Formato do nome de entidade do certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="5ee69-177">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="5ee69-178">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="5ee69-178">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="5ee69-179">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="5ee69-179">subjectAlternativeNameType</span></span>|[<span data-ttu-id="5ee69-180">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="5ee69-180">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="5ee69-181">Tipo de nome alternativo de entidade do certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="5ee69-181">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="5ee69-182">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="5ee69-182">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="5ee69-183">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="5ee69-183">certificateValidityPeriodValue</span></span>|<span data-ttu-id="5ee69-184">Int32</span><span class="sxs-lookup"><span data-stu-id="5ee69-184">Int32</span></span>|<span data-ttu-id="5ee69-185">Valor para o período de validade do certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="5ee69-185">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="5ee69-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="5ee69-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="5ee69-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="5ee69-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="5ee69-188">Dimensionar o período de validade do certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="5ee69-188">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="5ee69-189">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="5ee69-189">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="5ee69-190">Da intendedpurpose</span><span class="sxs-lookup"><span data-stu-id="5ee69-190">intendedPurpose</span></span>|[<span data-ttu-id="5ee69-191">Da intendedpurpose</span><span class="sxs-lookup"><span data-stu-id="5ee69-191">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="5ee69-192">Ainda não documentado.</span><span class="sxs-lookup"><span data-stu-id="5ee69-192">Not yet documented.</span></span> <span data-ttu-id="5ee69-193">Os valores possíveis são: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span><span class="sxs-lookup"><span data-stu-id="5ee69-193">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="5ee69-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ee69-194">Response</span></span>
<span data-ttu-id="5ee69-195">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5ee69-195">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ee69-196">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5ee69-196">Example</span></span>

### <a name="request"></a><span data-ttu-id="5ee69-197">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ee69-197">Request</span></span>
<span data-ttu-id="5ee69-198">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5ee69-198">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 591

{
  "@odata.type": "#microsoft.graph.windowsPhone81ImportedPFXCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="5ee69-199">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ee69-199">Response</span></span>
<span data-ttu-id="5ee69-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5ee69-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 763

{
  "@odata.type": "#microsoft.graph.windowsPhone81ImportedPFXCertificateProfile",
  "id": "08c7f847-f847-08c7-47f8-c70847f8c708",
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





