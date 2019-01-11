---
title: Criar windowsPhone81ImportedPFXCertificateProfile
description: Crie um novo objeto de windowsPhone81ImportedPFXCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 23e5b52e69e15dc37f94048a2b9b309d09ec0d32
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27852043"
---
# <a name="create-windowsphone81importedpfxcertificateprofile"></a><span data-ttu-id="3fbef-103">Criar windowsPhone81ImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="3fbef-103">Create windowsPhone81ImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="3fbef-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3fbef-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3fbef-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3fbef-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3fbef-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="3fbef-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3fbef-107">Crie um novo objeto de [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="3fbef-107">Create a new [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3fbef-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3fbef-108">Prerequisites</span></span>
<span data-ttu-id="3fbef-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3fbef-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3fbef-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3fbef-111">Permission type</span></span>|<span data-ttu-id="3fbef-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3fbef-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3fbef-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3fbef-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3fbef-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3fbef-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3fbef-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3fbef-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3fbef-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3fbef-116">Not supported.</span></span>|
|<span data-ttu-id="3fbef-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3fbef-117">Application</span></span>|<span data-ttu-id="3fbef-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3fbef-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3fbef-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3fbef-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3fbef-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3fbef-120">Request headers</span></span>
|<span data-ttu-id="3fbef-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3fbef-121">Header</span></span>|<span data-ttu-id="3fbef-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3fbef-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3fbef-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3fbef-123">Authorization</span></span>|<span data-ttu-id="3fbef-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3fbef-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3fbef-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3fbef-125">Accept</span></span>|<span data-ttu-id="3fbef-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3fbef-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3fbef-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3fbef-127">Request body</span></span>
<span data-ttu-id="3fbef-128">No corpo da solicitação, fornece uma representação JSON para o objeto windowsPhone81ImportedPFXCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="3fbef-128">In the request body, supply a JSON representation for the windowsPhone81ImportedPFXCertificateProfile object.</span></span>

<span data-ttu-id="3fbef-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o windowsPhone81ImportedPFXCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="3fbef-129">The following table shows the properties that are required when you create the windowsPhone81ImportedPFXCertificateProfile.</span></span>

|<span data-ttu-id="3fbef-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3fbef-130">Property</span></span>|<span data-ttu-id="3fbef-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="3fbef-131">Type</span></span>|<span data-ttu-id="3fbef-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3fbef-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3fbef-133">id</span><span class="sxs-lookup"><span data-stu-id="3fbef-133">id</span></span>|<span data-ttu-id="3fbef-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3fbef-134">String</span></span>|<span data-ttu-id="3fbef-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="3fbef-135">Key of the entity.</span></span> <span data-ttu-id="3fbef-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3fbef-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3fbef-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3fbef-137">lastModifiedDateTime</span></span>|<span data-ttu-id="3fbef-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3fbef-138">DateTimeOffset</span></span>|<span data-ttu-id="3fbef-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="3fbef-139">DateTime the object was last modified.</span></span> <span data-ttu-id="3fbef-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3fbef-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3fbef-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3fbef-141">roleScopeTagIds</span></span>|<span data-ttu-id="3fbef-142">String collection</span><span class="sxs-lookup"><span data-stu-id="3fbef-142">String collection</span></span>|<span data-ttu-id="3fbef-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="3fbef-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3fbef-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3fbef-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3fbef-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="3fbef-145">supportsScopeTags</span></span>|<span data-ttu-id="3fbef-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="3fbef-146">Boolean</span></span>|<span data-ttu-id="3fbef-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="3fbef-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="3fbef-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="3fbef-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="3fbef-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="3fbef-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="3fbef-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3fbef-150">This property is read-only.</span></span> <span data-ttu-id="3fbef-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3fbef-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3fbef-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3fbef-152">createdDateTime</span></span>|<span data-ttu-id="3fbef-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3fbef-153">DateTimeOffset</span></span>|<span data-ttu-id="3fbef-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="3fbef-154">DateTime the object was created.</span></span> <span data-ttu-id="3fbef-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3fbef-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3fbef-156">description</span><span class="sxs-lookup"><span data-stu-id="3fbef-156">description</span></span>|<span data-ttu-id="3fbef-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3fbef-157">String</span></span>|<span data-ttu-id="3fbef-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3fbef-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3fbef-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3fbef-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3fbef-160">displayName</span><span class="sxs-lookup"><span data-stu-id="3fbef-160">displayName</span></span>|<span data-ttu-id="3fbef-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3fbef-161">String</span></span>|<span data-ttu-id="3fbef-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3fbef-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3fbef-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3fbef-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3fbef-164">version</span><span class="sxs-lookup"><span data-stu-id="3fbef-164">version</span></span>|<span data-ttu-id="3fbef-165">Int32</span><span class="sxs-lookup"><span data-stu-id="3fbef-165">Int32</span></span>|<span data-ttu-id="3fbef-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3fbef-166">Version of the device configuration.</span></span> <span data-ttu-id="3fbef-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3fbef-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3fbef-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="3fbef-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="3fbef-169">Int32</span><span class="sxs-lookup"><span data-stu-id="3fbef-169">Int32</span></span>|<span data-ttu-id="3fbef-170">Porcentagem de limite de renovação de certificados.</span><span class="sxs-lookup"><span data-stu-id="3fbef-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="3fbef-171">Válido valores de 1 a 99 Inherited de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="3fbef-171">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="3fbef-172">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="3fbef-172">keyStorageProvider</span></span>|[<span data-ttu-id="3fbef-173">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="3fbef-173">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="3fbef-174">Provedor de armazenamento de chave (KSP) Inherited de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="3fbef-174">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="3fbef-175">Os valores possíveis são: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="3fbef-175">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="3fbef-176">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="3fbef-176">subjectNameFormat</span></span>|[<span data-ttu-id="3fbef-177">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="3fbef-177">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="3fbef-178">Certificado assunto nome formato herdado do [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="3fbef-178">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="3fbef-179">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="3fbef-179">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="3fbef-180">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="3fbef-180">subjectAlternativeNameType</span></span>|[<span data-ttu-id="3fbef-181">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="3fbef-181">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="3fbef-182">Certificado Subject Alternative nome tipo herdada do [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="3fbef-182">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="3fbef-183">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="3fbef-183">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="3fbef-184">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="3fbef-184">certificateValidityPeriodValue</span></span>|<span data-ttu-id="3fbef-185">Int32</span><span class="sxs-lookup"><span data-stu-id="3fbef-185">Int32</span></span>|<span data-ttu-id="3fbef-186">Valor para o período de validade de certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="3fbef-186">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="3fbef-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="3fbef-187">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="3fbef-188">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="3fbef-188">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="3fbef-189">Escala para o período de validade de certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="3fbef-189">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="3fbef-190">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="3fbef-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="3fbef-191">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="3fbef-191">intendedPurpose</span></span>|[<span data-ttu-id="3fbef-192">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="3fbef-192">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="3fbef-193">Ainda não documentado.</span><span class="sxs-lookup"><span data-stu-id="3fbef-193">Not yet documented.</span></span> <span data-ttu-id="3fbef-194">Os valores possíveis são: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span><span class="sxs-lookup"><span data-stu-id="3fbef-194">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="3fbef-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="3fbef-195">Response</span></span>
<span data-ttu-id="3fbef-196">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3fbef-196">If successful, this method returns a `201 Created` response code and a [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3fbef-197">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3fbef-197">Example</span></span>
### <a name="request"></a><span data-ttu-id="3fbef-198">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3fbef-198">Request</span></span>
<span data-ttu-id="3fbef-199">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3fbef-199">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 655

{
  "@odata.type": "#microsoft.graph.windowsPhone81ImportedPFXCertificateProfile",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="3fbef-200">Resposta</span><span class="sxs-lookup"><span data-stu-id="3fbef-200">Response</span></span>
<span data-ttu-id="3fbef-p117">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3fbef-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





