---
title: Criar macOSImportedPFXCertificateProfile
description: Criar um novo objeto macOSImportedPFXCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cd22fc9992e3ea44a1dae5de9b9dc87387195181
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32518405"
---
# <a name="create-macosimportedpfxcertificateprofile"></a><span data-ttu-id="5c29c-103">Criar macOSImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="5c29c-103">Create macOSImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="5c29c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5c29c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5c29c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5c29c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c29c-106">Criar um novo objeto [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="5c29c-106">Create a new [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5c29c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5c29c-107">Prerequisites</span></span>
<span data-ttu-id="5c29c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c29c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c29c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5c29c-110">Permission type</span></span>|<span data-ttu-id="5c29c-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5c29c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c29c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5c29c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5c29c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c29c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5c29c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5c29c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c29c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5c29c-115">Not supported.</span></span>|
|<span data-ttu-id="5c29c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5c29c-116">Application</span></span>|<span data-ttu-id="5c29c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5c29c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c29c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5c29c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="5c29c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5c29c-119">Request headers</span></span>
|<span data-ttu-id="5c29c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5c29c-120">Header</span></span>|<span data-ttu-id="5c29c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="5c29c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5c29c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5c29c-122">Authorization</span></span>|<span data-ttu-id="5c29c-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5c29c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5c29c-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5c29c-124">Accept</span></span>|<span data-ttu-id="5c29c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5c29c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c29c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5c29c-126">Request body</span></span>
<span data-ttu-id="5c29c-127">No corpo da solicitação, forneça uma representação JSON do objeto macOSImportedPFXCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="5c29c-127">In the request body, supply a JSON representation for the macOSImportedPFXCertificateProfile object.</span></span>

<span data-ttu-id="5c29c-128">A tabela a seguir mostra as propriedades que são necessárias ao criar macOSImportedPFXCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="5c29c-128">The following table shows the properties that are required when you create the macOSImportedPFXCertificateProfile.</span></span>

|<span data-ttu-id="5c29c-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5c29c-129">Property</span></span>|<span data-ttu-id="5c29c-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="5c29c-130">Type</span></span>|<span data-ttu-id="5c29c-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c29c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c29c-132">id</span><span class="sxs-lookup"><span data-stu-id="5c29c-132">id</span></span>|<span data-ttu-id="5c29c-133">String</span><span class="sxs-lookup"><span data-stu-id="5c29c-133">String</span></span>|<span data-ttu-id="5c29c-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="5c29c-134">Key of the entity.</span></span> <span data-ttu-id="5c29c-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c29c-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c29c-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5c29c-136">lastModifiedDateTime</span></span>|<span data-ttu-id="5c29c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c29c-137">DateTimeOffset</span></span>|<span data-ttu-id="5c29c-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="5c29c-138">DateTime the object was last modified.</span></span> <span data-ttu-id="5c29c-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c29c-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c29c-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5c29c-140">roleScopeTagIds</span></span>|<span data-ttu-id="5c29c-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="5c29c-141">String collection</span></span>|<span data-ttu-id="5c29c-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="5c29c-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="5c29c-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c29c-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c29c-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="5c29c-144">supportsScopeTags</span></span>|<span data-ttu-id="5c29c-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="5c29c-145">Boolean</span></span>|<span data-ttu-id="5c29c-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="5c29c-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="5c29c-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="5c29c-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="5c29c-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="5c29c-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="5c29c-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5c29c-149">This property is read-only.</span></span> <span data-ttu-id="5c29c-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c29c-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c29c-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5c29c-151">createdDateTime</span></span>|<span data-ttu-id="5c29c-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c29c-152">DateTimeOffset</span></span>|<span data-ttu-id="5c29c-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="5c29c-153">DateTime the object was created.</span></span> <span data-ttu-id="5c29c-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c29c-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c29c-155">description</span><span class="sxs-lookup"><span data-stu-id="5c29c-155">description</span></span>|<span data-ttu-id="5c29c-156">String</span><span class="sxs-lookup"><span data-stu-id="5c29c-156">String</span></span>|<span data-ttu-id="5c29c-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5c29c-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5c29c-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c29c-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c29c-159">displayName</span><span class="sxs-lookup"><span data-stu-id="5c29c-159">displayName</span></span>|<span data-ttu-id="5c29c-160">String</span><span class="sxs-lookup"><span data-stu-id="5c29c-160">String</span></span>|<span data-ttu-id="5c29c-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5c29c-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5c29c-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c29c-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c29c-163">versão</span><span class="sxs-lookup"><span data-stu-id="5c29c-163">version</span></span>|<span data-ttu-id="5c29c-164">Int32</span><span class="sxs-lookup"><span data-stu-id="5c29c-164">Int32</span></span>|<span data-ttu-id="5c29c-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5c29c-165">Version of the device configuration.</span></span> <span data-ttu-id="5c29c-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5c29c-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c29c-167">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="5c29c-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="5c29c-168">Int32</span><span class="sxs-lookup"><span data-stu-id="5c29c-168">Int32</span></span>|<span data-ttu-id="5c29c-169">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="5c29c-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="5c29c-170">Herdado de [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="5c29c-170">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="5c29c-171">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="5c29c-171">subjectNameFormat</span></span>|[<span data-ttu-id="5c29c-172">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="5c29c-172">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="5c29c-173">Formato do nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="5c29c-173">Certificate Subject Name Format.</span></span> <span data-ttu-id="5c29c-174">Herdado de [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="5c29c-174">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="5c29c-175">Os valores possíveis são: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="5c29c-175">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="5c29c-176">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="5c29c-176">subjectAlternativeNameType</span></span>|[<span data-ttu-id="5c29c-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="5c29c-177">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="5c29c-178">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="5c29c-178">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="5c29c-179">Herdado de [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="5c29c-179">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="5c29c-180">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="5c29c-180">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="5c29c-181">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="5c29c-181">certificateValidityPeriodValue</span></span>|<span data-ttu-id="5c29c-182">Int32</span><span class="sxs-lookup"><span data-stu-id="5c29c-182">Int32</span></span>|<span data-ttu-id="5c29c-183">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="5c29c-183">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="5c29c-184">Herdado de [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="5c29c-184">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="5c29c-185">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="5c29c-185">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="5c29c-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="5c29c-186">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="5c29c-187">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="5c29c-187">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="5c29c-188">Herdado de [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="5c29c-188">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="5c29c-189">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="5c29c-189">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="5c29c-190">Da intendedpurpose</span><span class="sxs-lookup"><span data-stu-id="5c29c-190">intendedPurpose</span></span>|[<span data-ttu-id="5c29c-191">Da intendedpurpose</span><span class="sxs-lookup"><span data-stu-id="5c29c-191">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="5c29c-192">Ainda não documentado.</span><span class="sxs-lookup"><span data-stu-id="5c29c-192">Not yet documented.</span></span> <span data-ttu-id="5c29c-193">Os valores possíveis são: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span><span class="sxs-lookup"><span data-stu-id="5c29c-193">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="5c29c-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c29c-194">Response</span></span>
<span data-ttu-id="5c29c-195">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5c29c-195">If successful, this method returns a `201 Created` response code and a [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c29c-196">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5c29c-196">Example</span></span>

### <a name="request"></a><span data-ttu-id="5c29c-197">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5c29c-197">Request</span></span>
<span data-ttu-id="5c29c-198">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5c29c-198">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 524

{
  "@odata.type": "#microsoft.graph.macOSImportedPFXCertificateProfile",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "renewalThresholdPercentage": 10,
  "subjectNameFormat": "commonNameAsEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "intendedPurpose": "smimeEncryption"
}
```

### <a name="response"></a><span data-ttu-id="5c29c-199">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c29c-199">Response</span></span>
<span data-ttu-id="5c29c-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5c29c-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 696

{
  "@odata.type": "#microsoft.graph.macOSImportedPFXCertificateProfile",
  "id": "4175bd8c-bd8c-4175-8cbd-75418cbd7541",
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
  "subjectNameFormat": "commonNameAsEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "intendedPurpose": "smimeEncryption"
}
```





