---
title: Criar androidImportedPFXCertificateProfile
description: Criar um novo objeto androidImportedPFXCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5046088d0792d15695bb9d580089d1ffec88a2a8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32476037"
---
# <a name="create-androidimportedpfxcertificateprofile"></a><span data-ttu-id="71ef2-103">Criar androidImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="71ef2-103">Create androidImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="71ef2-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="71ef2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="71ef2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="71ef2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71ef2-106">Criar um novo objeto [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="71ef2-106">Create a new [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="71ef2-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="71ef2-107">Prerequisites</span></span>
<span data-ttu-id="71ef2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71ef2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71ef2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="71ef2-110">Permission type</span></span>|<span data-ttu-id="71ef2-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="71ef2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71ef2-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="71ef2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="71ef2-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71ef2-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="71ef2-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="71ef2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71ef2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="71ef2-115">Not supported.</span></span>|
|<span data-ttu-id="71ef2-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="71ef2-116">Application</span></span>|<span data-ttu-id="71ef2-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="71ef2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="71ef2-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="71ef2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="71ef2-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="71ef2-119">Request headers</span></span>
|<span data-ttu-id="71ef2-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="71ef2-120">Header</span></span>|<span data-ttu-id="71ef2-121">Valor</span><span class="sxs-lookup"><span data-stu-id="71ef2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="71ef2-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="71ef2-122">Authorization</span></span>|<span data-ttu-id="71ef2-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="71ef2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="71ef2-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="71ef2-124">Accept</span></span>|<span data-ttu-id="71ef2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="71ef2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="71ef2-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="71ef2-126">Request body</span></span>
<span data-ttu-id="71ef2-127">No corpo da solicitação, forneça uma representação JSON do objeto androidImportedPFXCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="71ef2-127">In the request body, supply a JSON representation for the androidImportedPFXCertificateProfile object.</span></span>

<span data-ttu-id="71ef2-128">A tabela a seguir mostra as propriedades que são necessárias ao criar androidImportedPFXCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="71ef2-128">The following table shows the properties that are required when you create the androidImportedPFXCertificateProfile.</span></span>

|<span data-ttu-id="71ef2-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="71ef2-129">Property</span></span>|<span data-ttu-id="71ef2-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="71ef2-130">Type</span></span>|<span data-ttu-id="71ef2-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="71ef2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71ef2-132">id</span><span class="sxs-lookup"><span data-stu-id="71ef2-132">id</span></span>|<span data-ttu-id="71ef2-133">String</span><span class="sxs-lookup"><span data-stu-id="71ef2-133">String</span></span>|<span data-ttu-id="71ef2-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="71ef2-134">Key of the entity.</span></span> <span data-ttu-id="71ef2-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71ef2-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71ef2-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="71ef2-136">lastModifiedDateTime</span></span>|<span data-ttu-id="71ef2-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71ef2-137">DateTimeOffset</span></span>|<span data-ttu-id="71ef2-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="71ef2-138">DateTime the object was last modified.</span></span> <span data-ttu-id="71ef2-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71ef2-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71ef2-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="71ef2-140">roleScopeTagIds</span></span>|<span data-ttu-id="71ef2-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="71ef2-141">String collection</span></span>|<span data-ttu-id="71ef2-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="71ef2-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="71ef2-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71ef2-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71ef2-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="71ef2-144">supportsScopeTags</span></span>|<span data-ttu-id="71ef2-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="71ef2-145">Boolean</span></span>|<span data-ttu-id="71ef2-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="71ef2-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="71ef2-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="71ef2-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="71ef2-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="71ef2-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="71ef2-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="71ef2-149">This property is read-only.</span></span> <span data-ttu-id="71ef2-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71ef2-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71ef2-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="71ef2-151">createdDateTime</span></span>|<span data-ttu-id="71ef2-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71ef2-152">DateTimeOffset</span></span>|<span data-ttu-id="71ef2-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="71ef2-153">DateTime the object was created.</span></span> <span data-ttu-id="71ef2-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71ef2-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71ef2-155">description</span><span class="sxs-lookup"><span data-stu-id="71ef2-155">description</span></span>|<span data-ttu-id="71ef2-156">String</span><span class="sxs-lookup"><span data-stu-id="71ef2-156">String</span></span>|<span data-ttu-id="71ef2-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="71ef2-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="71ef2-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71ef2-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71ef2-159">displayName</span><span class="sxs-lookup"><span data-stu-id="71ef2-159">displayName</span></span>|<span data-ttu-id="71ef2-160">String</span><span class="sxs-lookup"><span data-stu-id="71ef2-160">String</span></span>|<span data-ttu-id="71ef2-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="71ef2-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="71ef2-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71ef2-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71ef2-163">versão</span><span class="sxs-lookup"><span data-stu-id="71ef2-163">version</span></span>|<span data-ttu-id="71ef2-164">Int32</span><span class="sxs-lookup"><span data-stu-id="71ef2-164">Int32</span></span>|<span data-ttu-id="71ef2-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="71ef2-165">Version of the device configuration.</span></span> <span data-ttu-id="71ef2-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71ef2-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71ef2-167">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="71ef2-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="71ef2-168">Int32</span><span class="sxs-lookup"><span data-stu-id="71ef2-168">Int32</span></span>|<span data-ttu-id="71ef2-169">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="71ef2-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="71ef2-170">Valores válidos de 1 a 99 herdados de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="71ef2-170">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="71ef2-171">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="71ef2-171">subjectNameFormat</span></span>|[<span data-ttu-id="71ef2-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="71ef2-172">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="71ef2-173">Formato do nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="71ef2-173">Certificate Subject Name Format.</span></span> <span data-ttu-id="71ef2-174">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="71ef2-174">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="71ef2-175">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="71ef2-175">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="71ef2-176">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="71ef2-176">subjectAlternativeNameType</span></span>|[<span data-ttu-id="71ef2-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="71ef2-177">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="71ef2-178">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="71ef2-178">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="71ef2-179">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="71ef2-179">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="71ef2-180">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="71ef2-180">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="71ef2-181">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="71ef2-181">certificateValidityPeriodValue</span></span>|<span data-ttu-id="71ef2-182">Int32</span><span class="sxs-lookup"><span data-stu-id="71ef2-182">Int32</span></span>|<span data-ttu-id="71ef2-183">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="71ef2-183">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="71ef2-184">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="71ef2-184">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="71ef2-185">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="71ef2-185">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="71ef2-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="71ef2-186">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="71ef2-187">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="71ef2-187">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="71ef2-188">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="71ef2-188">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="71ef2-189">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="71ef2-189">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="71ef2-190">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="71ef2-190">extendedKeyUsages</span></span>|<span data-ttu-id="71ef2-191">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="71ef2-191">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="71ef2-192">Configurações de EKU (uso estendido de chave).</span><span class="sxs-lookup"><span data-stu-id="71ef2-192">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="71ef2-193">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="71ef2-193">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="71ef2-194">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="71ef2-194">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="71ef2-195">Da intendedpurpose</span><span class="sxs-lookup"><span data-stu-id="71ef2-195">intendedPurpose</span></span>|[<span data-ttu-id="71ef2-196">Da intendedpurpose</span><span class="sxs-lookup"><span data-stu-id="71ef2-196">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="71ef2-197">Ainda não documentado.</span><span class="sxs-lookup"><span data-stu-id="71ef2-197">Not yet documented.</span></span> <span data-ttu-id="71ef2-198">Os valores possíveis são: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span><span class="sxs-lookup"><span data-stu-id="71ef2-198">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="71ef2-199">Resposta</span><span class="sxs-lookup"><span data-stu-id="71ef2-199">Response</span></span>
<span data-ttu-id="71ef2-200">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="71ef2-200">If successful, this method returns a `201 Created` response code and a [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71ef2-201">Exemplo</span><span class="sxs-lookup"><span data-stu-id="71ef2-201">Example</span></span>

### <a name="request"></a><span data-ttu-id="71ef2-202">Solicitação</span><span class="sxs-lookup"><span data-stu-id="71ef2-202">Request</span></span>
<span data-ttu-id="71ef2-203">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="71ef2-203">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 719

{
  "@odata.type": "#microsoft.graph.androidImportedPFXCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="71ef2-204">Resposta</span><span class="sxs-lookup"><span data-stu-id="71ef2-204">Response</span></span>
<span data-ttu-id="71ef2-p117">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="71ef2-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 891

{
  "@odata.type": "#microsoft.graph.androidImportedPFXCertificateProfile",
  "id": "1cd3b0a6-b0a6-1cd3-a6b0-d31ca6b0d31c",
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





