---
title: Criar macOSImportedPFXCertificateProfile
description: Crie um novo objeto de macOSImportedPFXCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 11a3dfca4979e7211b2faf5feb9f29d4f9a5f2f9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983090"
---
# <a name="create-macosimportedpfxcertificateprofile"></a><span data-ttu-id="61124-103">Criar macOSImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="61124-103">Create macOSImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="61124-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="61124-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="61124-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="61124-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="61124-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="61124-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="61124-107">Crie um novo objeto de [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="61124-107">Create a new [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="61124-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="61124-108">Prerequisites</span></span>
<span data-ttu-id="61124-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61124-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61124-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="61124-111">Permission type</span></span>|<span data-ttu-id="61124-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="61124-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="61124-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="61124-113">Delegated (work or school account)</span></span>|<span data-ttu-id="61124-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61124-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="61124-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="61124-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="61124-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="61124-116">Not supported.</span></span>|
|<span data-ttu-id="61124-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="61124-117">Application</span></span>|<span data-ttu-id="61124-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="61124-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="61124-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="61124-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="61124-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="61124-120">Request headers</span></span>
|<span data-ttu-id="61124-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="61124-121">Header</span></span>|<span data-ttu-id="61124-122">Valor</span><span class="sxs-lookup"><span data-stu-id="61124-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="61124-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="61124-123">Authorization</span></span>|<span data-ttu-id="61124-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="61124-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="61124-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="61124-125">Accept</span></span>|<span data-ttu-id="61124-126">application/json</span><span class="sxs-lookup"><span data-stu-id="61124-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="61124-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="61124-127">Request body</span></span>
<span data-ttu-id="61124-128">No corpo da solicitação, fornece uma representação JSON para o objeto macOSImportedPFXCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="61124-128">In the request body, supply a JSON representation for the macOSImportedPFXCertificateProfile object.</span></span>

<span data-ttu-id="61124-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o macOSImportedPFXCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="61124-129">The following table shows the properties that are required when you create the macOSImportedPFXCertificateProfile.</span></span>

|<span data-ttu-id="61124-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="61124-130">Property</span></span>|<span data-ttu-id="61124-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="61124-131">Type</span></span>|<span data-ttu-id="61124-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="61124-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61124-133">id</span><span class="sxs-lookup"><span data-stu-id="61124-133">id</span></span>|<span data-ttu-id="61124-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="61124-134">String</span></span>|<span data-ttu-id="61124-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="61124-135">Key of the entity.</span></span> <span data-ttu-id="61124-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="61124-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="61124-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="61124-137">lastModifiedDateTime</span></span>|<span data-ttu-id="61124-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61124-138">DateTimeOffset</span></span>|<span data-ttu-id="61124-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="61124-139">DateTime the object was last modified.</span></span> <span data-ttu-id="61124-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="61124-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="61124-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="61124-141">roleScopeTagIds</span></span>|<span data-ttu-id="61124-142">String collection</span><span class="sxs-lookup"><span data-stu-id="61124-142">String collection</span></span>|<span data-ttu-id="61124-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="61124-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="61124-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="61124-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="61124-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="61124-145">supportsScopeTags</span></span>|<span data-ttu-id="61124-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="61124-146">Boolean</span></span>|<span data-ttu-id="61124-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="61124-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="61124-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="61124-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="61124-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="61124-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="61124-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="61124-150">This property is read-only.</span></span> <span data-ttu-id="61124-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="61124-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="61124-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="61124-152">createdDateTime</span></span>|<span data-ttu-id="61124-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61124-153">DateTimeOffset</span></span>|<span data-ttu-id="61124-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="61124-154">DateTime the object was created.</span></span> <span data-ttu-id="61124-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="61124-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="61124-156">description</span><span class="sxs-lookup"><span data-stu-id="61124-156">description</span></span>|<span data-ttu-id="61124-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="61124-157">String</span></span>|<span data-ttu-id="61124-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="61124-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="61124-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="61124-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="61124-160">displayName</span><span class="sxs-lookup"><span data-stu-id="61124-160">displayName</span></span>|<span data-ttu-id="61124-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="61124-161">String</span></span>|<span data-ttu-id="61124-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="61124-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="61124-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="61124-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="61124-164">version</span><span class="sxs-lookup"><span data-stu-id="61124-164">version</span></span>|<span data-ttu-id="61124-165">Int32</span><span class="sxs-lookup"><span data-stu-id="61124-165">Int32</span></span>|<span data-ttu-id="61124-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="61124-166">Version of the device configuration.</span></span> <span data-ttu-id="61124-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="61124-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="61124-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="61124-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="61124-169">Int32</span><span class="sxs-lookup"><span data-stu-id="61124-169">Int32</span></span>|<span data-ttu-id="61124-170">Porcentagem de limite de renovação de certificados.</span><span class="sxs-lookup"><span data-stu-id="61124-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="61124-171">Herdado de [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="61124-171">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="61124-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="61124-172">subjectNameFormat</span></span>|[<span data-ttu-id="61124-173">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="61124-173">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="61124-174">Formato de nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="61124-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="61124-175">Herdada do [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="61124-175">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="61124-176">Os possíveis valores são: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="61124-176">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="61124-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="61124-177">subjectAlternativeNameType</span></span>|[<span data-ttu-id="61124-178">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="61124-178">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="61124-179">Tipo de nome alternativo de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="61124-179">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="61124-180">Herdada do [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="61124-180">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="61124-181">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="61124-181">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="61124-182">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="61124-182">certificateValidityPeriodValue</span></span>|<span data-ttu-id="61124-183">Int32</span><span class="sxs-lookup"><span data-stu-id="61124-183">Int32</span></span>|<span data-ttu-id="61124-184">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="61124-184">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="61124-185">Herdado de [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="61124-185">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="61124-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="61124-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="61124-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="61124-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="61124-188">Escala para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="61124-188">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="61124-189">Herdada do [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="61124-189">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="61124-190">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="61124-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="61124-191">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="61124-191">intendedPurpose</span></span>|[<span data-ttu-id="61124-192">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="61124-192">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="61124-193">Ainda não documentado.</span><span class="sxs-lookup"><span data-stu-id="61124-193">Not yet documented.</span></span> <span data-ttu-id="61124-194">Os valores possíveis são: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span><span class="sxs-lookup"><span data-stu-id="61124-194">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="61124-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="61124-195">Response</span></span>
<span data-ttu-id="61124-196">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="61124-196">If successful, this method returns a `201 Created` response code and a [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="61124-197">Exemplo</span><span class="sxs-lookup"><span data-stu-id="61124-197">Example</span></span>
### <a name="request"></a><span data-ttu-id="61124-198">Solicitação</span><span class="sxs-lookup"><span data-stu-id="61124-198">Request</span></span>
<span data-ttu-id="61124-199">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="61124-199">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 588

{
  "@odata.type": "#microsoft.graph.macOSImportedPFXCertificateProfile",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="61124-200">Resposta</span><span class="sxs-lookup"><span data-stu-id="61124-200">Response</span></span>
<span data-ttu-id="61124-p117">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="61124-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





