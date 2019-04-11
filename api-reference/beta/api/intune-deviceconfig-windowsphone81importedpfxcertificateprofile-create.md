---
title: Criar windowsPhone81ImportedPFXCertificateProfile
description: Criar um novo objeto windowsPhone81ImportedPFXCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1a42ed28f9c961bb135a4b7cc940fb3e6833980a
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31796140"
---
# <a name="create-windowsphone81importedpfxcertificateprofile"></a><span data-ttu-id="1c881-103">Criar windowsPhone81ImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="1c881-103">Create windowsPhone81ImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="1c881-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1c881-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1c881-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1c881-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1c881-106">Criar um novo objeto [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="1c881-106">Create a new [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1c881-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1c881-107">Prerequisites</span></span>
<span data-ttu-id="1c881-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c881-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c881-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1c881-110">Permission type</span></span>|<span data-ttu-id="1c881-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1c881-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1c881-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1c881-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1c881-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c881-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1c881-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1c881-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1c881-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1c881-115">Not supported.</span></span>|
|<span data-ttu-id="1c881-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1c881-116">Application</span></span>|<span data-ttu-id="1c881-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1c881-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1c881-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1c881-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1c881-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1c881-119">Request headers</span></span>
|<span data-ttu-id="1c881-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1c881-120">Header</span></span>|<span data-ttu-id="1c881-121">Valor</span><span class="sxs-lookup"><span data-stu-id="1c881-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1c881-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1c881-122">Authorization</span></span>|<span data-ttu-id="1c881-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1c881-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1c881-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1c881-124">Accept</span></span>|<span data-ttu-id="1c881-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1c881-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c881-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1c881-126">Request body</span></span>
<span data-ttu-id="1c881-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsPhone81ImportedPFXCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="1c881-127">In the request body, supply a JSON representation for the windowsPhone81ImportedPFXCertificateProfile object.</span></span>

<span data-ttu-id="1c881-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsPhone81ImportedPFXCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="1c881-128">The following table shows the properties that are required when you create the windowsPhone81ImportedPFXCertificateProfile.</span></span>

|<span data-ttu-id="1c881-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1c881-129">Property</span></span>|<span data-ttu-id="1c881-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="1c881-130">Type</span></span>|<span data-ttu-id="1c881-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="1c881-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c881-132">id</span><span class="sxs-lookup"><span data-stu-id="1c881-132">id</span></span>|<span data-ttu-id="1c881-133">String</span><span class="sxs-lookup"><span data-stu-id="1c881-133">String</span></span>|<span data-ttu-id="1c881-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="1c881-134">Key of the entity.</span></span> <span data-ttu-id="1c881-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1c881-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c881-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1c881-136">lastModifiedDateTime</span></span>|<span data-ttu-id="1c881-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c881-137">DateTimeOffset</span></span>|<span data-ttu-id="1c881-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="1c881-138">DateTime the object was last modified.</span></span> <span data-ttu-id="1c881-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1c881-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c881-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1c881-140">roleScopeTagIds</span></span>|<span data-ttu-id="1c881-141">Coleção String</span><span class="sxs-lookup"><span data-stu-id="1c881-141">String collection</span></span>|<span data-ttu-id="1c881-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="1c881-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1c881-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1c881-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c881-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="1c881-144">supportsScopeTags</span></span>|<span data-ttu-id="1c881-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c881-145">Boolean</span></span>|<span data-ttu-id="1c881-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="1c881-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1c881-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="1c881-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1c881-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="1c881-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1c881-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1c881-149">This property is read-only.</span></span> <span data-ttu-id="1c881-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1c881-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c881-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1c881-151">createdDateTime</span></span>|<span data-ttu-id="1c881-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c881-152">DateTimeOffset</span></span>|<span data-ttu-id="1c881-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="1c881-153">DateTime the object was created.</span></span> <span data-ttu-id="1c881-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1c881-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c881-155">description</span><span class="sxs-lookup"><span data-stu-id="1c881-155">description</span></span>|<span data-ttu-id="1c881-156">String</span><span class="sxs-lookup"><span data-stu-id="1c881-156">String</span></span>|<span data-ttu-id="1c881-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1c881-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1c881-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1c881-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c881-159">displayName</span><span class="sxs-lookup"><span data-stu-id="1c881-159">displayName</span></span>|<span data-ttu-id="1c881-160">String</span><span class="sxs-lookup"><span data-stu-id="1c881-160">String</span></span>|<span data-ttu-id="1c881-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1c881-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1c881-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1c881-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c881-163">versão</span><span class="sxs-lookup"><span data-stu-id="1c881-163">version</span></span>|<span data-ttu-id="1c881-164">Int32</span><span class="sxs-lookup"><span data-stu-id="1c881-164">Int32</span></span>|<span data-ttu-id="1c881-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1c881-165">Version of the device configuration.</span></span> <span data-ttu-id="1c881-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1c881-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c881-167">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="1c881-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="1c881-168">Int32</span><span class="sxs-lookup"><span data-stu-id="1c881-168">Int32</span></span>|<span data-ttu-id="1c881-169">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="1c881-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="1c881-170">Valores válidos de 1 a 99 herdados de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="1c881-170">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="1c881-171">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="1c881-171">keyStorageProvider</span></span>|[<span data-ttu-id="1c881-172">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="1c881-172">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="1c881-173">Provedor de armazenamento de chave (KSP) herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="1c881-173">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="1c881-174">Os valores possíveis são: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="1c881-174">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="1c881-175">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="1c881-175">subjectNameFormat</span></span>|[<span data-ttu-id="1c881-176">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="1c881-176">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="1c881-177">Formato do nome de entidade do certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="1c881-177">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="1c881-178">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="1c881-178">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="1c881-179">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="1c881-179">subjectAlternativeNameType</span></span>|[<span data-ttu-id="1c881-180">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="1c881-180">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="1c881-181">Tipo de nome alternativo de entidade do certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="1c881-181">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="1c881-182">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="1c881-182">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="1c881-183">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="1c881-183">certificateValidityPeriodValue</span></span>|<span data-ttu-id="1c881-184">Int32</span><span class="sxs-lookup"><span data-stu-id="1c881-184">Int32</span></span>|<span data-ttu-id="1c881-185">Valor para o período de validade do certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="1c881-185">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="1c881-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="1c881-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="1c881-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="1c881-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="1c881-188">Dimensionar o período de validade do certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="1c881-188">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="1c881-189">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="1c881-189">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="1c881-190">Da intendedpurpose</span><span class="sxs-lookup"><span data-stu-id="1c881-190">intendedPurpose</span></span>|[<span data-ttu-id="1c881-191">Da intendedpurpose</span><span class="sxs-lookup"><span data-stu-id="1c881-191">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="1c881-192">Ainda não documentado.</span><span class="sxs-lookup"><span data-stu-id="1c881-192">Not yet documented.</span></span> <span data-ttu-id="1c881-193">Os valores possíveis são: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span><span class="sxs-lookup"><span data-stu-id="1c881-193">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="1c881-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c881-194">Response</span></span>
<span data-ttu-id="1c881-195">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1c881-195">If successful, this method returns a `201 Created` response code and a [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c881-196">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1c881-196">Example</span></span>

### <a name="request"></a><span data-ttu-id="1c881-197">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1c881-197">Request</span></span>
<span data-ttu-id="1c881-198">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1c881-198">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="1c881-199">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c881-199">Response</span></span>
<span data-ttu-id="1c881-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1c881-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





