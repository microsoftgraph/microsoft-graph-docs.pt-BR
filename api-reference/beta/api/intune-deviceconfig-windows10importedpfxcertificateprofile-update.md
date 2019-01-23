---
title: Atualizar windows10ImportedPFXCertificateProfile
description: Atualize as propriedades de um objeto windows10ImportedPFXCertificateProfile.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0a525c64bbf2e0210acb200488d7426b08b23052
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411817"
---
# <a name="update-windows10importedpfxcertificateprofile"></a><span data-ttu-id="77b79-103">Atualizar windows10ImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="77b79-103">Update windows10ImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="77b79-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="77b79-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="77b79-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="77b79-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="77b79-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="77b79-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77b79-107">Atualize as propriedades de um objeto [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="77b79-107">Update the properties of a [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="77b79-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="77b79-108">Prerequisites</span></span>
<span data-ttu-id="77b79-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="77b79-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="77b79-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="77b79-111">Permission type</span></span>|<span data-ttu-id="77b79-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="77b79-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77b79-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="77b79-113">Delegated (work or school account)</span></span>|<span data-ttu-id="77b79-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77b79-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="77b79-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="77b79-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77b79-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="77b79-116">Not supported.</span></span>|
|<span data-ttu-id="77b79-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="77b79-117">Application</span></span>|<span data-ttu-id="77b79-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="77b79-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="77b79-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="77b79-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="77b79-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="77b79-120">Request headers</span></span>
|<span data-ttu-id="77b79-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="77b79-121">Header</span></span>|<span data-ttu-id="77b79-122">Valor</span><span class="sxs-lookup"><span data-stu-id="77b79-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="77b79-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="77b79-123">Authorization</span></span>|<span data-ttu-id="77b79-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="77b79-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="77b79-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="77b79-125">Accept</span></span>|<span data-ttu-id="77b79-126">application/json</span><span class="sxs-lookup"><span data-stu-id="77b79-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="77b79-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="77b79-127">Request body</span></span>
<span data-ttu-id="77b79-128">No corpo da solicitação, fornece uma representação JSON para o objeto [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="77b79-128">In the request body, supply a JSON representation for the [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) object.</span></span>

<span data-ttu-id="77b79-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="77b79-129">The following table shows the properties that are required when you create the [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md).</span></span>

|<span data-ttu-id="77b79-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="77b79-130">Property</span></span>|<span data-ttu-id="77b79-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="77b79-131">Type</span></span>|<span data-ttu-id="77b79-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="77b79-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77b79-133">id</span><span class="sxs-lookup"><span data-stu-id="77b79-133">id</span></span>|<span data-ttu-id="77b79-134">String</span><span class="sxs-lookup"><span data-stu-id="77b79-134">String</span></span>|<span data-ttu-id="77b79-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="77b79-135">Key of the entity.</span></span> <span data-ttu-id="77b79-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77b79-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77b79-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="77b79-137">lastModifiedDateTime</span></span>|<span data-ttu-id="77b79-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77b79-138">DateTimeOffset</span></span>|<span data-ttu-id="77b79-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="77b79-139">DateTime the object was last modified.</span></span> <span data-ttu-id="77b79-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77b79-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77b79-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="77b79-141">roleScopeTagIds</span></span>|<span data-ttu-id="77b79-142">String collection</span><span class="sxs-lookup"><span data-stu-id="77b79-142">String collection</span></span>|<span data-ttu-id="77b79-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="77b79-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="77b79-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77b79-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77b79-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="77b79-145">supportsScopeTags</span></span>|<span data-ttu-id="77b79-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="77b79-146">Boolean</span></span>|<span data-ttu-id="77b79-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="77b79-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="77b79-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="77b79-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="77b79-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="77b79-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="77b79-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="77b79-150">This property is read-only.</span></span> <span data-ttu-id="77b79-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77b79-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77b79-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="77b79-152">createdDateTime</span></span>|<span data-ttu-id="77b79-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77b79-153">DateTimeOffset</span></span>|<span data-ttu-id="77b79-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="77b79-154">DateTime the object was created.</span></span> <span data-ttu-id="77b79-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77b79-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77b79-156">description</span><span class="sxs-lookup"><span data-stu-id="77b79-156">description</span></span>|<span data-ttu-id="77b79-157">String</span><span class="sxs-lookup"><span data-stu-id="77b79-157">String</span></span>|<span data-ttu-id="77b79-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="77b79-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="77b79-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77b79-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77b79-160">displayName</span><span class="sxs-lookup"><span data-stu-id="77b79-160">displayName</span></span>|<span data-ttu-id="77b79-161">String</span><span class="sxs-lookup"><span data-stu-id="77b79-161">String</span></span>|<span data-ttu-id="77b79-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="77b79-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="77b79-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77b79-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77b79-164">version</span><span class="sxs-lookup"><span data-stu-id="77b79-164">version</span></span>|<span data-ttu-id="77b79-165">Int32</span><span class="sxs-lookup"><span data-stu-id="77b79-165">Int32</span></span>|<span data-ttu-id="77b79-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="77b79-166">Version of the device configuration.</span></span> <span data-ttu-id="77b79-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77b79-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77b79-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="77b79-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="77b79-169">Int32</span><span class="sxs-lookup"><span data-stu-id="77b79-169">Int32</span></span>|<span data-ttu-id="77b79-170">Porcentagem de limite de renovação de certificados.</span><span class="sxs-lookup"><span data-stu-id="77b79-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="77b79-171">Válido valores de 1 a 99 Inherited de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="77b79-171">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="77b79-172">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="77b79-172">keyStorageProvider</span></span>|[<span data-ttu-id="77b79-173">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="77b79-173">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="77b79-174">Provedor de armazenamento de chave (KSP) Inherited de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="77b79-174">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="77b79-175">Os valores possíveis são: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="77b79-175">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="77b79-176">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="77b79-176">subjectNameFormat</span></span>|[<span data-ttu-id="77b79-177">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="77b79-177">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="77b79-178">Certificado assunto nome formato herdado do [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="77b79-178">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="77b79-179">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="77b79-179">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="77b79-180">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="77b79-180">subjectAlternativeNameType</span></span>|[<span data-ttu-id="77b79-181">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="77b79-181">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="77b79-182">Certificado Subject Alternative nome tipo herdada do [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="77b79-182">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="77b79-183">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="77b79-183">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="77b79-184">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="77b79-184">certificateValidityPeriodValue</span></span>|<span data-ttu-id="77b79-185">Int32</span><span class="sxs-lookup"><span data-stu-id="77b79-185">Int32</span></span>|<span data-ttu-id="77b79-186">Valor para o período de validade de certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="77b79-186">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="77b79-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="77b79-187">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="77b79-188">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="77b79-188">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="77b79-189">Escala para o período de validade de certificado herdado de [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="77b79-189">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="77b79-190">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="77b79-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="77b79-191">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="77b79-191">intendedPurpose</span></span>|[<span data-ttu-id="77b79-192">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="77b79-192">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="77b79-193">Ainda não documentado.</span><span class="sxs-lookup"><span data-stu-id="77b79-193">Not yet documented.</span></span> <span data-ttu-id="77b79-194">Os valores possíveis são: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span><span class="sxs-lookup"><span data-stu-id="77b79-194">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="77b79-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="77b79-195">Response</span></span>
<span data-ttu-id="77b79-196">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="77b79-196">If successful, this method returns a `200 OK` response code and an updated [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77b79-197">Exemplo</span><span class="sxs-lookup"><span data-stu-id="77b79-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="77b79-198">Solicitação</span><span class="sxs-lookup"><span data-stu-id="77b79-198">Request</span></span>
<span data-ttu-id="77b79-199">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="77b79-199">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="77b79-200">Resposta</span><span class="sxs-lookup"><span data-stu-id="77b79-200">Response</span></span>
<span data-ttu-id="77b79-p117">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="77b79-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




