---
title: Criar windows10ImportedPFXCertificateProfile
description: Crie um novo objeto de windows10ImportedPFXCertificateProfile.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 666a849b1713c7009af7473438ed546e7639165d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29408128"
---
# <a name="create-windows10importedpfxcertificateprofile"></a><span data-ttu-id="62404-103">Criar windows10ImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="62404-103">Create windows10ImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="62404-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="62404-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="62404-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="62404-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="62404-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="62404-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62404-107">Crie um novo objeto de [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="62404-107">Create a new [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="62404-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="62404-108">Prerequisites</span></span>
<span data-ttu-id="62404-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="62404-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="62404-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="62404-111">Permission type</span></span>|<span data-ttu-id="62404-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="62404-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="62404-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="62404-113">Delegated (work or school account)</span></span>|<span data-ttu-id="62404-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62404-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="62404-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="62404-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="62404-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="62404-116">Not supported.</span></span>|
|<span data-ttu-id="62404-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="62404-117">Application</span></span>|<span data-ttu-id="62404-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="62404-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="62404-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="62404-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="62404-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="62404-120">Request headers</span></span>
|<span data-ttu-id="62404-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="62404-121">Header</span></span>|<span data-ttu-id="62404-122">Valor</span><span class="sxs-lookup"><span data-stu-id="62404-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="62404-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="62404-123">Authorization</span></span>|<span data-ttu-id="62404-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="62404-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="62404-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="62404-125">Accept</span></span>|<span data-ttu-id="62404-126">application/json</span><span class="sxs-lookup"><span data-stu-id="62404-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="62404-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="62404-127">Request body</span></span>
<span data-ttu-id="62404-128">No corpo da solicitação, fornece uma representação JSON para o objeto windows10ImportedPFXCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="62404-128">In the request body, supply a JSON representation for the windows10ImportedPFXCertificateProfile object.</span></span>

<span data-ttu-id="62404-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o windows10ImportedPFXCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="62404-129">The following table shows the properties that are required when you create the windows10ImportedPFXCertificateProfile.</span></span>

|<span data-ttu-id="62404-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="62404-130">Property</span></span>|<span data-ttu-id="62404-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="62404-131">Type</span></span>|<span data-ttu-id="62404-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="62404-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62404-133">id</span><span class="sxs-lookup"><span data-stu-id="62404-133">id</span></span>|<span data-ttu-id="62404-134">String</span><span class="sxs-lookup"><span data-stu-id="62404-134">String</span></span>|<span data-ttu-id="62404-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="62404-135">Key of the entity.</span></span> <span data-ttu-id="62404-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="62404-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62404-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="62404-137">lastModifiedDateTime</span></span>|<span data-ttu-id="62404-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62404-138">DateTimeOffset</span></span>|<span data-ttu-id="62404-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="62404-139">DateTime the object was last modified.</span></span> <span data-ttu-id="62404-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="62404-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62404-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="62404-141">roleScopeTagIds</span></span>|<span data-ttu-id="62404-142">String collection</span><span class="sxs-lookup"><span data-stu-id="62404-142">String collection</span></span>|<span data-ttu-id="62404-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="62404-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="62404-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="62404-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62404-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="62404-145">supportsScopeTags</span></span>|<span data-ttu-id="62404-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="62404-146">Boolean</span></span>|<span data-ttu-id="62404-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="62404-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="62404-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="62404-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="62404-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="62404-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="62404-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="62404-150">This property is read-only.</span></span> <span data-ttu-id="62404-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="62404-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62404-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="62404-152">createdDateTime</span></span>|<span data-ttu-id="62404-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62404-153">DateTimeOffset</span></span>|<span data-ttu-id="62404-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="62404-154">DateTime the object was created.</span></span> <span data-ttu-id="62404-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="62404-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62404-156">description</span><span class="sxs-lookup"><span data-stu-id="62404-156">description</span></span>|<span data-ttu-id="62404-157">String</span><span class="sxs-lookup"><span data-stu-id="62404-157">String</span></span>|<span data-ttu-id="62404-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="62404-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="62404-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="62404-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62404-160">displayName</span><span class="sxs-lookup"><span data-stu-id="62404-160">displayName</span></span>|<span data-ttu-id="62404-161">String</span><span class="sxs-lookup"><span data-stu-id="62404-161">String</span></span>|<span data-ttu-id="62404-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="62404-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="62404-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="62404-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62404-164">version</span><span class="sxs-lookup"><span data-stu-id="62404-164">version</span></span>|<span data-ttu-id="62404-165">Int32</span><span class="sxs-lookup"><span data-stu-id="62404-165">Int32</span></span>|<span data-ttu-id="62404-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="62404-166">Version of the device configuration.</span></span> <span data-ttu-id="62404-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="62404-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62404-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="62404-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="62404-169">Int32</span><span class="sxs-lookup"><span data-stu-id="62404-169">Int32</span></span>|<span data-ttu-id="62404-170">Porcentagem de limite de renovação de certificados.</span><span class="sxs-lookup"><span data-stu-id="62404-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="62404-171">Válido valores de 1 a 99 Inherited de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="62404-171">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="62404-172">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="62404-172">keyStorageProvider</span></span>|[<span data-ttu-id="62404-173">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="62404-173">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="62404-174">Provedor de armazenamento de chave (KSP) Inherited de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="62404-174">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="62404-175">Os valores possíveis são: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="62404-175">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="62404-176">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="62404-176">subjectNameFormat</span></span>|[<span data-ttu-id="62404-177">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="62404-177">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="62404-178">Certificado assunto nome formato herdado do [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="62404-178">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="62404-179">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="62404-179">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="62404-180">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="62404-180">subjectAlternativeNameType</span></span>|[<span data-ttu-id="62404-181">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="62404-181">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="62404-182">Certificado Subject Alternative nome tipo herdada do [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="62404-182">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="62404-183">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="62404-183">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="62404-184">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="62404-184">certificateValidityPeriodValue</span></span>|<span data-ttu-id="62404-185">Int32</span><span class="sxs-lookup"><span data-stu-id="62404-185">Int32</span></span>|<span data-ttu-id="62404-186">Valor para o período de validade de certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="62404-186">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="62404-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="62404-187">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="62404-188">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="62404-188">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="62404-189">Escala para o período de validade de certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="62404-189">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="62404-190">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="62404-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="62404-191">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="62404-191">intendedPurpose</span></span>|[<span data-ttu-id="62404-192">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="62404-192">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="62404-193">Ainda não documentado.</span><span class="sxs-lookup"><span data-stu-id="62404-193">Not yet documented.</span></span> <span data-ttu-id="62404-194">Os valores possíveis são: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span><span class="sxs-lookup"><span data-stu-id="62404-194">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="62404-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="62404-195">Response</span></span>
<span data-ttu-id="62404-196">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="62404-196">If successful, this method returns a `201 Created` response code and a [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62404-197">Exemplo</span><span class="sxs-lookup"><span data-stu-id="62404-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="62404-198">Solicitação</span><span class="sxs-lookup"><span data-stu-id="62404-198">Request</span></span>
<span data-ttu-id="62404-199">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="62404-199">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="62404-200">Resposta</span><span class="sxs-lookup"><span data-stu-id="62404-200">Response</span></span>
<span data-ttu-id="62404-p117">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="62404-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




