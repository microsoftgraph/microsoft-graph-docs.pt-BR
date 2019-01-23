---
title: Criar macOSImportedPFXCertificateProfile
description: Crie um novo objeto de macOSImportedPFXCertificateProfile.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: fa14580bd62d42e3706d7a7f422f46832e78cf02
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29408261"
---
# <a name="create-macosimportedpfxcertificateprofile"></a><span data-ttu-id="bef0a-103">Criar macOSImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="bef0a-103">Create macOSImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="bef0a-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="bef0a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bef0a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="bef0a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bef0a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="bef0a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bef0a-107">Crie um novo objeto de [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="bef0a-107">Create a new [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bef0a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bef0a-108">Prerequisites</span></span>
<span data-ttu-id="bef0a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="bef0a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="bef0a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bef0a-111">Permission type</span></span>|<span data-ttu-id="bef0a-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bef0a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bef0a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bef0a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bef0a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bef0a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bef0a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bef0a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bef0a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bef0a-116">Not supported.</span></span>|
|<span data-ttu-id="bef0a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bef0a-117">Application</span></span>|<span data-ttu-id="bef0a-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bef0a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bef0a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bef0a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="bef0a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bef0a-120">Request headers</span></span>
|<span data-ttu-id="bef0a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bef0a-121">Header</span></span>|<span data-ttu-id="bef0a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="bef0a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bef0a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="bef0a-123">Authorization</span></span>|<span data-ttu-id="bef0a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bef0a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bef0a-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bef0a-125">Accept</span></span>|<span data-ttu-id="bef0a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bef0a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bef0a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bef0a-127">Request body</span></span>
<span data-ttu-id="bef0a-128">No corpo da solicitação, fornece uma representação JSON para o objeto macOSImportedPFXCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="bef0a-128">In the request body, supply a JSON representation for the macOSImportedPFXCertificateProfile object.</span></span>

<span data-ttu-id="bef0a-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o macOSImportedPFXCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="bef0a-129">The following table shows the properties that are required when you create the macOSImportedPFXCertificateProfile.</span></span>

|<span data-ttu-id="bef0a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bef0a-130">Property</span></span>|<span data-ttu-id="bef0a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="bef0a-131">Type</span></span>|<span data-ttu-id="bef0a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="bef0a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bef0a-133">id</span><span class="sxs-lookup"><span data-stu-id="bef0a-133">id</span></span>|<span data-ttu-id="bef0a-134">String</span><span class="sxs-lookup"><span data-stu-id="bef0a-134">String</span></span>|<span data-ttu-id="bef0a-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="bef0a-135">Key of the entity.</span></span> <span data-ttu-id="bef0a-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bef0a-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bef0a-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bef0a-137">lastModifiedDateTime</span></span>|<span data-ttu-id="bef0a-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bef0a-138">DateTimeOffset</span></span>|<span data-ttu-id="bef0a-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="bef0a-139">DateTime the object was last modified.</span></span> <span data-ttu-id="bef0a-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bef0a-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bef0a-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="bef0a-141">roleScopeTagIds</span></span>|<span data-ttu-id="bef0a-142">String collection</span><span class="sxs-lookup"><span data-stu-id="bef0a-142">String collection</span></span>|<span data-ttu-id="bef0a-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="bef0a-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="bef0a-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bef0a-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bef0a-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="bef0a-145">supportsScopeTags</span></span>|<span data-ttu-id="bef0a-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="bef0a-146">Boolean</span></span>|<span data-ttu-id="bef0a-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="bef0a-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="bef0a-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="bef0a-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="bef0a-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="bef0a-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="bef0a-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bef0a-150">This property is read-only.</span></span> <span data-ttu-id="bef0a-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bef0a-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bef0a-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bef0a-152">createdDateTime</span></span>|<span data-ttu-id="bef0a-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bef0a-153">DateTimeOffset</span></span>|<span data-ttu-id="bef0a-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="bef0a-154">DateTime the object was created.</span></span> <span data-ttu-id="bef0a-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bef0a-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bef0a-156">description</span><span class="sxs-lookup"><span data-stu-id="bef0a-156">description</span></span>|<span data-ttu-id="bef0a-157">String</span><span class="sxs-lookup"><span data-stu-id="bef0a-157">String</span></span>|<span data-ttu-id="bef0a-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bef0a-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="bef0a-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bef0a-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bef0a-160">displayName</span><span class="sxs-lookup"><span data-stu-id="bef0a-160">displayName</span></span>|<span data-ttu-id="bef0a-161">String</span><span class="sxs-lookup"><span data-stu-id="bef0a-161">String</span></span>|<span data-ttu-id="bef0a-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bef0a-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="bef0a-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bef0a-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bef0a-164">version</span><span class="sxs-lookup"><span data-stu-id="bef0a-164">version</span></span>|<span data-ttu-id="bef0a-165">Int32</span><span class="sxs-lookup"><span data-stu-id="bef0a-165">Int32</span></span>|<span data-ttu-id="bef0a-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bef0a-166">Version of the device configuration.</span></span> <span data-ttu-id="bef0a-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bef0a-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bef0a-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="bef0a-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="bef0a-169">Int32</span><span class="sxs-lookup"><span data-stu-id="bef0a-169">Int32</span></span>|<span data-ttu-id="bef0a-170">Porcentagem de limite de renovação de certificados.</span><span class="sxs-lookup"><span data-stu-id="bef0a-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="bef0a-171">Herdado de [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="bef0a-171">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="bef0a-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="bef0a-172">subjectNameFormat</span></span>|[<span data-ttu-id="bef0a-173">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="bef0a-173">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="bef0a-174">Formato de nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="bef0a-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="bef0a-175">Herdada do [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="bef0a-175">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="bef0a-176">Os possíveis valores são: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="bef0a-176">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="bef0a-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="bef0a-177">subjectAlternativeNameType</span></span>|[<span data-ttu-id="bef0a-178">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="bef0a-178">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="bef0a-179">Tipo de nome alternativo de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="bef0a-179">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="bef0a-180">Herdada do [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="bef0a-180">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="bef0a-181">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="bef0a-181">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="bef0a-182">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="bef0a-182">certificateValidityPeriodValue</span></span>|<span data-ttu-id="bef0a-183">Int32</span><span class="sxs-lookup"><span data-stu-id="bef0a-183">Int32</span></span>|<span data-ttu-id="bef0a-184">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="bef0a-184">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="bef0a-185">Herdado de [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="bef0a-185">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="bef0a-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="bef0a-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="bef0a-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="bef0a-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="bef0a-188">Escala para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="bef0a-188">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="bef0a-189">Herdada do [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="bef0a-189">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="bef0a-190">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="bef0a-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="bef0a-191">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="bef0a-191">intendedPurpose</span></span>|[<span data-ttu-id="bef0a-192">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="bef0a-192">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="bef0a-193">Ainda não documentado.</span><span class="sxs-lookup"><span data-stu-id="bef0a-193">Not yet documented.</span></span> <span data-ttu-id="bef0a-194">Os valores possíveis são: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span><span class="sxs-lookup"><span data-stu-id="bef0a-194">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="bef0a-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="bef0a-195">Response</span></span>
<span data-ttu-id="bef0a-196">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bef0a-196">If successful, this method returns a `201 Created` response code and a [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bef0a-197">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bef0a-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="bef0a-198">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bef0a-198">Request</span></span>
<span data-ttu-id="bef0a-199">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bef0a-199">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bef0a-200">Resposta</span><span class="sxs-lookup"><span data-stu-id="bef0a-200">Response</span></span>
<span data-ttu-id="bef0a-p117">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bef0a-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




