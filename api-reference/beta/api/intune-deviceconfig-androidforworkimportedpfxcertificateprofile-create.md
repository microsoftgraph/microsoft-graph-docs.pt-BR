---
title: Criar androidForWorkImportedPFXCertificateProfile
description: Criar um novo objeto androidForWorkImportedPFXCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0b4c2ffde1683ab2a7100604405d4b35a85d6931
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166896"
---
# <a name="create-androidforworkimportedpfxcertificateprofile"></a><span data-ttu-id="d7bdd-103">Criar androidForWorkImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="d7bdd-103">Create androidForWorkImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="d7bdd-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d7bdd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d7bdd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d7bdd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d7bdd-106">Criar um novo objeto [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="d7bdd-106">Create a new [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d7bdd-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d7bdd-107">Prerequisites</span></span>
<span data-ttu-id="d7bdd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d7bdd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d7bdd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d7bdd-110">Permission type</span></span>|<span data-ttu-id="d7bdd-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d7bdd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d7bdd-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d7bdd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d7bdd-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7bdd-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d7bdd-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d7bdd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d7bdd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d7bdd-115">Not supported.</span></span>|
|<span data-ttu-id="d7bdd-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d7bdd-116">Application</span></span>|<span data-ttu-id="d7bdd-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d7bdd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d7bdd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d7bdd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d7bdd-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d7bdd-119">Request headers</span></span>
|<span data-ttu-id="d7bdd-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d7bdd-120">Header</span></span>|<span data-ttu-id="d7bdd-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d7bdd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d7bdd-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d7bdd-122">Authorization</span></span>|<span data-ttu-id="d7bdd-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d7bdd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d7bdd-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d7bdd-124">Accept</span></span>|<span data-ttu-id="d7bdd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d7bdd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7bdd-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d7bdd-126">Request body</span></span>
<span data-ttu-id="d7bdd-127">No corpo da solicitação, forneça uma representação JSON do objeto androidForWorkImportedPFXCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="d7bdd-127">In the request body, supply a JSON representation for the androidForWorkImportedPFXCertificateProfile object.</span></span>

<span data-ttu-id="d7bdd-128">A tabela a seguir mostra as propriedades que são necessárias ao criar androidForWorkImportedPFXCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="d7bdd-128">The following table shows the properties that are required when you create the androidForWorkImportedPFXCertificateProfile.</span></span>

|<span data-ttu-id="d7bdd-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d7bdd-129">Property</span></span>|<span data-ttu-id="d7bdd-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="d7bdd-130">Type</span></span>|<span data-ttu-id="d7bdd-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7bdd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7bdd-132">id</span><span class="sxs-lookup"><span data-stu-id="d7bdd-132">id</span></span>|<span data-ttu-id="d7bdd-133">String</span><span class="sxs-lookup"><span data-stu-id="d7bdd-133">String</span></span>|<span data-ttu-id="d7bdd-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d7bdd-134">Key of the entity.</span></span> <span data-ttu-id="d7bdd-135">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d7bdd-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7bdd-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d7bdd-136">lastModifiedDateTime</span></span>|<span data-ttu-id="d7bdd-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7bdd-137">DateTimeOffset</span></span>|<span data-ttu-id="d7bdd-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="d7bdd-138">DateTime the object was last modified.</span></span> <span data-ttu-id="d7bdd-139">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d7bdd-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7bdd-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d7bdd-140">roleScopeTagIds</span></span>|<span data-ttu-id="d7bdd-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d7bdd-141">String collection</span></span>|<span data-ttu-id="d7bdd-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="d7bdd-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d7bdd-143">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d7bdd-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7bdd-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d7bdd-144">supportsScopeTags</span></span>|<span data-ttu-id="d7bdd-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="d7bdd-145">Boolean</span></span>|<span data-ttu-id="d7bdd-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="d7bdd-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d7bdd-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="d7bdd-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d7bdd-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="d7bdd-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d7bdd-149">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d7bdd-149">This property is read-only.</span></span> <span data-ttu-id="d7bdd-150">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d7bdd-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7bdd-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d7bdd-151">createdDateTime</span></span>|<span data-ttu-id="d7bdd-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7bdd-152">DateTimeOffset</span></span>|<span data-ttu-id="d7bdd-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="d7bdd-153">DateTime the object was created.</span></span> <span data-ttu-id="d7bdd-154">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d7bdd-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7bdd-155">description</span><span class="sxs-lookup"><span data-stu-id="d7bdd-155">description</span></span>|<span data-ttu-id="d7bdd-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d7bdd-156">String</span></span>|<span data-ttu-id="d7bdd-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d7bdd-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d7bdd-158">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d7bdd-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7bdd-159">displayName</span><span class="sxs-lookup"><span data-stu-id="d7bdd-159">displayName</span></span>|<span data-ttu-id="d7bdd-160">String</span><span class="sxs-lookup"><span data-stu-id="d7bdd-160">String</span></span>|<span data-ttu-id="d7bdd-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d7bdd-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d7bdd-162">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d7bdd-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7bdd-163">version</span><span class="sxs-lookup"><span data-stu-id="d7bdd-163">version</span></span>|<span data-ttu-id="d7bdd-164">Int32</span><span class="sxs-lookup"><span data-stu-id="d7bdd-164">Int32</span></span>|<span data-ttu-id="d7bdd-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d7bdd-165">Version of the device configuration.</span></span> <span data-ttu-id="d7bdd-166">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d7bdd-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7bdd-167">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="d7bdd-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="d7bdd-168">Int32</span><span class="sxs-lookup"><span data-stu-id="d7bdd-168">Int32</span></span>|<span data-ttu-id="d7bdd-169">Porcentagem de limite de renovação de certificado.</span><span class="sxs-lookup"><span data-stu-id="d7bdd-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="d7bdd-170">Valores válidos de 1 a 99 herdados de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="d7bdd-170">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="d7bdd-171">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="d7bdd-171">subjectNameFormat</span></span>|[<span data-ttu-id="d7bdd-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="d7bdd-172">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="d7bdd-173">Formato do nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="d7bdd-173">Certificate Subject Name Format.</span></span> <span data-ttu-id="d7bdd-174">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="d7bdd-174">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="d7bdd-175">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="d7bdd-175">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="d7bdd-176">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="d7bdd-176">subjectAlternativeNameType</span></span>|[<span data-ttu-id="d7bdd-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="d7bdd-177">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="d7bdd-178">Tipo de nome alternativo da entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="d7bdd-178">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="d7bdd-179">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="d7bdd-179">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="d7bdd-180">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="d7bdd-180">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="d7bdd-181">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="d7bdd-181">certificateValidityPeriodValue</span></span>|<span data-ttu-id="d7bdd-182">Int32</span><span class="sxs-lookup"><span data-stu-id="d7bdd-182">Int32</span></span>|<span data-ttu-id="d7bdd-183">Valor para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="d7bdd-183">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="d7bdd-184">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="d7bdd-184">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="d7bdd-185">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="d7bdd-185">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="d7bdd-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="d7bdd-186">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="d7bdd-187">Dimensionar o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="d7bdd-187">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="d7bdd-188">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="d7bdd-188">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="d7bdd-189">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="d7bdd-189">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="d7bdd-190">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="d7bdd-190">extendedKeyUsages</span></span>|<span data-ttu-id="d7bdd-191">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="d7bdd-191">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="d7bdd-192">Configurações de EKU (uso estendido de chave).</span><span class="sxs-lookup"><span data-stu-id="d7bdd-192">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="d7bdd-193">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="d7bdd-193">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="d7bdd-194">Herdado de [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="d7bdd-194">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="d7bdd-195">Da intendedpurpose</span><span class="sxs-lookup"><span data-stu-id="d7bdd-195">intendedPurpose</span></span>|[<span data-ttu-id="d7bdd-196">Da intendedpurpose</span><span class="sxs-lookup"><span data-stu-id="d7bdd-196">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="d7bdd-197">Ainda não documentado.</span><span class="sxs-lookup"><span data-stu-id="d7bdd-197">Not yet documented.</span></span> <span data-ttu-id="d7bdd-198">Os valores possíveis são: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span><span class="sxs-lookup"><span data-stu-id="d7bdd-198">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="d7bdd-199">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7bdd-199">Response</span></span>
<span data-ttu-id="d7bdd-200">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d7bdd-200">If successful, this method returns a `201 Created` response code and a [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7bdd-201">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d7bdd-201">Example</span></span>

### <a name="request"></a><span data-ttu-id="d7bdd-202">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d7bdd-202">Request</span></span>
<span data-ttu-id="d7bdd-203">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d7bdd-203">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 726

{
  "@odata.type": "#microsoft.graph.androidForWorkImportedPFXCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="d7bdd-204">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7bdd-204">Response</span></span>
<span data-ttu-id="d7bdd-p117">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d7bdd-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 898

{
  "@odata.type": "#microsoft.graph.androidForWorkImportedPFXCertificateProfile",
  "id": "a0bfd7bc-d7bc-a0bf-bcd7-bfa0bcd7bfa0",
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




