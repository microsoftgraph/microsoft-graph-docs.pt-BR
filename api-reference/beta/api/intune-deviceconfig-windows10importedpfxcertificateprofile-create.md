---
title: Criar windows10ImportedPFXCertificateProfile
description: Criar um novo objeto windows10ImportedPFXCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0ae2fa6642c8e4278be33995892c4946df48ead5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32516795"
---
# <a name="create-windows10importedpfxcertificateprofile"></a><span data-ttu-id="a70fb-103">Criar windows10ImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="a70fb-103">Create windows10ImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="a70fb-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a70fb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a70fb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a70fb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a70fb-106">Criar um novo objeto [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="a70fb-106">Create a new [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a70fb-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a70fb-107">Prerequisites</span></span>
<span data-ttu-id="a70fb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a70fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a70fb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a70fb-110">Permission type</span></span>|<span data-ttu-id="a70fb-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a70fb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a70fb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a70fb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a70fb-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a70fb-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a70fb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a70fb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a70fb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a70fb-115">Not supported.</span></span>|
|<span data-ttu-id="a70fb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a70fb-116">Application</span></span>|<span data-ttu-id="a70fb-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a70fb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a70fb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a70fb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a70fb-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a70fb-119">Request headers</span></span>
|<span data-ttu-id="a70fb-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a70fb-120">Header</span></span>|<span data-ttu-id="a70fb-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a70fb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a70fb-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a70fb-122">Authorization</span></span>|<span data-ttu-id="a70fb-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a70fb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a70fb-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a70fb-124">Accept</span></span>|<span data-ttu-id="a70fb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a70fb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a70fb-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a70fb-126">Request body</span></span>
<span data-ttu-id="a70fb-127">No corpo da solicitação, forneça uma representação JSON do objeto windows10ImportedPFXCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="a70fb-127">In the request body, supply a JSON representation for the windows10ImportedPFXCertificateProfile object.</span></span>

<span data-ttu-id="a70fb-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windows10ImportedPFXCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="a70fb-128">The following table shows the properties that are required when you create the windows10ImportedPFXCertificateProfile.</span></span>

|<span data-ttu-id="a70fb-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a70fb-129">Property</span></span>|<span data-ttu-id="a70fb-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a70fb-130">Type</span></span>|<span data-ttu-id="a70fb-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a70fb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a70fb-132">id</span><span class="sxs-lookup"><span data-stu-id="a70fb-132">id</span></span>|<span data-ttu-id="a70fb-133">String</span><span class="sxs-lookup"><span data-stu-id="a70fb-133">String</span></span>|<span data-ttu-id="a70fb-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a70fb-134">Key of the entity.</span></span> <span data-ttu-id="a70fb-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a70fb-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a70fb-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a70fb-136">lastModifiedDateTime</span></span>|<span data-ttu-id="a70fb-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a70fb-137">DateTimeOffset</span></span>|<span data-ttu-id="a70fb-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="a70fb-138">DateTime the object was last modified.</span></span> <span data-ttu-id="a70fb-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a70fb-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a70fb-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a70fb-140">roleScopeTagIds</span></span>|<span data-ttu-id="a70fb-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a70fb-141">String collection</span></span>|<span data-ttu-id="a70fb-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="a70fb-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a70fb-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a70fb-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a70fb-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a70fb-144">supportsScopeTags</span></span>|<span data-ttu-id="a70fb-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="a70fb-145">Boolean</span></span>|<span data-ttu-id="a70fb-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="a70fb-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a70fb-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="a70fb-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a70fb-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="a70fb-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a70fb-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a70fb-149">This property is read-only.</span></span> <span data-ttu-id="a70fb-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a70fb-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a70fb-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a70fb-151">createdDateTime</span></span>|<span data-ttu-id="a70fb-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a70fb-152">DateTimeOffset</span></span>|<span data-ttu-id="a70fb-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="a70fb-153">DateTime the object was created.</span></span> <span data-ttu-id="a70fb-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a70fb-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a70fb-155">description</span><span class="sxs-lookup"><span data-stu-id="a70fb-155">description</span></span>|<span data-ttu-id="a70fb-156">String</span><span class="sxs-lookup"><span data-stu-id="a70fb-156">String</span></span>|<span data-ttu-id="a70fb-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a70fb-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a70fb-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a70fb-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a70fb-159">displayName</span><span class="sxs-lookup"><span data-stu-id="a70fb-159">displayName</span></span>|<span data-ttu-id="a70fb-160">String</span><span class="sxs-lookup"><span data-stu-id="a70fb-160">String</span></span>|<span data-ttu-id="a70fb-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a70fb-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a70fb-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a70fb-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a70fb-163">versão</span><span class="sxs-lookup"><span data-stu-id="a70fb-163">version</span></span>|<span data-ttu-id="a70fb-164">Int32</span><span class="sxs-lookup"><span data-stu-id="a70fb-164">Int32</span></span>|<span data-ttu-id="a70fb-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a70fb-165">Version of the device configuration.</span></span> <span data-ttu-id="a70fb-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a70fb-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a70fb-167">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="a70fb-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="a70fb-168">Int32</span><span class="sxs-lookup"><span data-stu-id="a70fb-168">Int32</span></span>|<span data-ttu-id="a70fb-169">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="a70fb-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="a70fb-170">Valores válidos de 1 a 99 herdados de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="a70fb-170">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="a70fb-171">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="a70fb-171">keyStorageProvider</span></span>|[<span data-ttu-id="a70fb-172">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="a70fb-172">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="a70fb-173">Provedor de armazenamento de chave (KSP) herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="a70fb-173">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="a70fb-174">Os valores possíveis são: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="a70fb-174">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="a70fb-175">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="a70fb-175">subjectNameFormat</span></span>|[<span data-ttu-id="a70fb-176">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="a70fb-176">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="a70fb-177">Formato do nome de entidade do certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="a70fb-177">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="a70fb-178">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="a70fb-178">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="a70fb-179">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="a70fb-179">subjectAlternativeNameType</span></span>|[<span data-ttu-id="a70fb-180">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="a70fb-180">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="a70fb-181">Tipo de nome alternativo de entidade do certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="a70fb-181">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="a70fb-182">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="a70fb-182">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="a70fb-183">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="a70fb-183">certificateValidityPeriodValue</span></span>|<span data-ttu-id="a70fb-184">Int32</span><span class="sxs-lookup"><span data-stu-id="a70fb-184">Int32</span></span>|<span data-ttu-id="a70fb-185">Valor para o período de validade do certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="a70fb-185">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="a70fb-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="a70fb-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="a70fb-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="a70fb-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="a70fb-188">Dimensionar o período de validade do certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="a70fb-188">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="a70fb-189">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="a70fb-189">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="a70fb-190">Da intendedpurpose</span><span class="sxs-lookup"><span data-stu-id="a70fb-190">intendedPurpose</span></span>|[<span data-ttu-id="a70fb-191">Da intendedpurpose</span><span class="sxs-lookup"><span data-stu-id="a70fb-191">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="a70fb-192">Ainda não documentado.</span><span class="sxs-lookup"><span data-stu-id="a70fb-192">Not yet documented.</span></span> <span data-ttu-id="a70fb-193">Os valores possíveis são: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span><span class="sxs-lookup"><span data-stu-id="a70fb-193">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="a70fb-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="a70fb-194">Response</span></span>
<span data-ttu-id="a70fb-195">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a70fb-195">If successful, this method returns a `201 Created` response code and a [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a70fb-196">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a70fb-196">Example</span></span>

### <a name="request"></a><span data-ttu-id="a70fb-197">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a70fb-197">Request</span></span>
<span data-ttu-id="a70fb-198">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a70fb-198">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="a70fb-199">Resposta</span><span class="sxs-lookup"><span data-stu-id="a70fb-199">Response</span></span>
<span data-ttu-id="a70fb-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a70fb-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





