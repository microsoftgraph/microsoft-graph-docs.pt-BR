---
title: Criar windowsPhone81SCEPCertificateProfile
description: Crie um novo objeto de windowsPhone81SCEPCertificateProfile.
author: tfitzmac
ms.openlocfilehash: b7c274f6e15578863d88f71900f815599ae420b6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314088"
---
# <a name="create-windowsphone81scepcertificateprofile"></a><span data-ttu-id="8f4de-103">Criar windowsPhone81SCEPCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="8f4de-103">Create windowsPhone81SCEPCertificateProfile</span></span>

> <span data-ttu-id="8f4de-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8f4de-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8f4de-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8f4de-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8f4de-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8f4de-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8f4de-107">Crie um novo objeto de [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="8f4de-107">Create a new [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8f4de-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8f4de-108">Prerequisites</span></span>
<span data-ttu-id="8f4de-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f4de-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f4de-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8f4de-111">Permission type</span></span>|<span data-ttu-id="8f4de-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8f4de-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8f4de-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8f4de-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8f4de-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f4de-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8f4de-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8f4de-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8f4de-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8f4de-116">Not supported.</span></span>|
|<span data-ttu-id="8f4de-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8f4de-117">Application</span></span>|<span data-ttu-id="8f4de-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8f4de-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8f4de-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8f4de-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="8f4de-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8f4de-120">Request headers</span></span>
|<span data-ttu-id="8f4de-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8f4de-121">Header</span></span>|<span data-ttu-id="8f4de-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8f4de-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8f4de-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8f4de-123">Authorization</span></span>|<span data-ttu-id="8f4de-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8f4de-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8f4de-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8f4de-125">Accept</span></span>|<span data-ttu-id="8f4de-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8f4de-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f4de-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8f4de-127">Request body</span></span>
<span data-ttu-id="8f4de-128">No corpo da solicitação, fornece uma representação JSON para o objeto windowsPhone81SCEPCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="8f4de-128">In the request body, supply a JSON representation for the windowsPhone81SCEPCertificateProfile object.</span></span>

<span data-ttu-id="8f4de-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o windowsPhone81SCEPCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="8f4de-129">The following table shows the properties that are required when you create the windowsPhone81SCEPCertificateProfile.</span></span>

|<span data-ttu-id="8f4de-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8f4de-130">Property</span></span>|<span data-ttu-id="8f4de-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="8f4de-131">Type</span></span>|<span data-ttu-id="8f4de-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f4de-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f4de-133">id</span><span class="sxs-lookup"><span data-stu-id="8f4de-133">id</span></span>|<span data-ttu-id="8f4de-134">String</span><span class="sxs-lookup"><span data-stu-id="8f4de-134">String</span></span>|<span data-ttu-id="8f4de-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="8f4de-135">Key of the entity.</span></span> <span data-ttu-id="8f4de-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8f4de-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f4de-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8f4de-137">lastModifiedDateTime</span></span>|<span data-ttu-id="8f4de-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f4de-138">DateTimeOffset</span></span>|<span data-ttu-id="8f4de-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="8f4de-139">DateTime the object was last modified.</span></span> <span data-ttu-id="8f4de-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8f4de-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f4de-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8f4de-141">roleScopeTagIds</span></span>|<span data-ttu-id="8f4de-142">String collection</span><span class="sxs-lookup"><span data-stu-id="8f4de-142">String collection</span></span>|<span data-ttu-id="8f4de-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="8f4de-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8f4de-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8f4de-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f4de-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="8f4de-145">supportsScopeTags</span></span>|<span data-ttu-id="8f4de-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f4de-146">Boolean</span></span>|<span data-ttu-id="8f4de-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="8f4de-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="8f4de-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="8f4de-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="8f4de-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="8f4de-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="8f4de-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8f4de-150">This property is read-only.</span></span> <span data-ttu-id="8f4de-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8f4de-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f4de-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8f4de-152">createdDateTime</span></span>|<span data-ttu-id="8f4de-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f4de-153">DateTimeOffset</span></span>|<span data-ttu-id="8f4de-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="8f4de-154">DateTime the object was created.</span></span> <span data-ttu-id="8f4de-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8f4de-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f4de-156">description</span><span class="sxs-lookup"><span data-stu-id="8f4de-156">description</span></span>|<span data-ttu-id="8f4de-157">String</span><span class="sxs-lookup"><span data-stu-id="8f4de-157">String</span></span>|<span data-ttu-id="8f4de-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8f4de-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8f4de-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8f4de-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f4de-160">displayName</span><span class="sxs-lookup"><span data-stu-id="8f4de-160">displayName</span></span>|<span data-ttu-id="8f4de-161">String</span><span class="sxs-lookup"><span data-stu-id="8f4de-161">String</span></span>|<span data-ttu-id="8f4de-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8f4de-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8f4de-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8f4de-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f4de-164">version</span><span class="sxs-lookup"><span data-stu-id="8f4de-164">version</span></span>|<span data-ttu-id="8f4de-165">Int32</span><span class="sxs-lookup"><span data-stu-id="8f4de-165">Int32</span></span>|<span data-ttu-id="8f4de-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8f4de-166">Version of the device configuration.</span></span> <span data-ttu-id="8f4de-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8f4de-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f4de-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="8f4de-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="8f4de-169">Int32</span><span class="sxs-lookup"><span data-stu-id="8f4de-169">Int32</span></span>|<span data-ttu-id="8f4de-170">Porcentagem de limite de renovação de certificados.</span><span class="sxs-lookup"><span data-stu-id="8f4de-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="8f4de-171">Herdado de [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="8f4de-171">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="8f4de-172">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="8f4de-172">keyStorageProvider</span></span>|[<span data-ttu-id="8f4de-173">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="8f4de-173">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="8f4de-174">Provedor de armazenamento de chave (KSP).</span><span class="sxs-lookup"><span data-stu-id="8f4de-174">Key Storage Provider (KSP).</span></span> <span data-ttu-id="8f4de-175">Herdada do [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="8f4de-175">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="8f4de-176">Os valores possíveis são: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="8f4de-176">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="8f4de-177">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="8f4de-177">subjectNameFormat</span></span>|[<span data-ttu-id="8f4de-178">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="8f4de-178">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="8f4de-179">Formato de nome de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="8f4de-179">Certificate Subject Name Format.</span></span> <span data-ttu-id="8f4de-180">Herdada do [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="8f4de-180">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="8f4de-181">Os valores possíveis são: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="8f4de-181">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="8f4de-182">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="8f4de-182">subjectAlternativeNameType</span></span>|[<span data-ttu-id="8f4de-183">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="8f4de-183">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="8f4de-184">Tipo de nome alternativo de entidade do certificado.</span><span class="sxs-lookup"><span data-stu-id="8f4de-184">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="8f4de-185">Herdada do [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="8f4de-185">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="8f4de-186">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="8f4de-186">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="8f4de-187">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="8f4de-187">certificateValidityPeriodValue</span></span>|<span data-ttu-id="8f4de-188">Int32</span><span class="sxs-lookup"><span data-stu-id="8f4de-188">Int32</span></span>|<span data-ttu-id="8f4de-189">Valor para o período de Validtiy do certificado.</span><span class="sxs-lookup"><span data-stu-id="8f4de-189">Value for the Certificate Validtiy Period.</span></span> <span data-ttu-id="8f4de-190">Herdado de [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="8f4de-190">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="8f4de-191">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="8f4de-191">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="8f4de-192">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="8f4de-192">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="8f4de-193">Escala para o período de validade do certificado.</span><span class="sxs-lookup"><span data-stu-id="8f4de-193">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="8f4de-194">Herdada do [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="8f4de-194">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="8f4de-195">Os valores possíveis são: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="8f4de-195">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="8f4de-196">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="8f4de-196">extendedKeyUsages</span></span>|<span data-ttu-id="8f4de-197">coleção [extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="8f4de-197">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="8f4de-198">Configurações de uso de chave (EKU) estendido.</span><span class="sxs-lookup"><span data-stu-id="8f4de-198">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="8f4de-199">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="8f4de-199">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="8f4de-200">Herdado de [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="8f4de-200">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="8f4de-201">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="8f4de-201">scepServerUrls</span></span>|<span data-ttu-id="8f4de-202">String collection</span><span class="sxs-lookup"><span data-stu-id="8f4de-202">String collection</span></span>|<span data-ttu-id="8f4de-203">URLs de servidor SCEP.</span><span class="sxs-lookup"><span data-stu-id="8f4de-203">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="8f4de-204">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="8f4de-204">subjectNameFormatString</span></span>|<span data-ttu-id="8f4de-205">String</span><span class="sxs-lookup"><span data-stu-id="8f4de-205">String</span></span>|<span data-ttu-id="8f4de-206">Um formato personalizado a ser usada com SubjectNameFormat = personalizado.</span><span class="sxs-lookup"><span data-stu-id="8f4de-206">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="8f4de-207">Exemplo: CN = {{EmailAddress}}, F = {{EmailAddress}}, OU = usuários do Enterprise, O = Contoso Corporation, L = Redmond, ST = WA, C = US</span><span class="sxs-lookup"><span data-stu-id="8f4de-207">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="8f4de-208">keyUsage</span><span class="sxs-lookup"><span data-stu-id="8f4de-208">keyUsage</span></span>|[<span data-ttu-id="8f4de-209">keyUsages</span><span class="sxs-lookup"><span data-stu-id="8f4de-209">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="8f4de-210">Uso de chave SCEP.</span><span class="sxs-lookup"><span data-stu-id="8f4de-210">SCEP Key Usage.</span></span> <span data-ttu-id="8f4de-211">Os valores possíveis são: `keyEncipherment` e `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="8f4de-211">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="8f4de-212">keySize</span><span class="sxs-lookup"><span data-stu-id="8f4de-212">keySize</span></span>|[<span data-ttu-id="8f4de-213">keySize</span><span class="sxs-lookup"><span data-stu-id="8f4de-213">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="8f4de-214">Tamanho da chave SCEP.</span><span class="sxs-lookup"><span data-stu-id="8f4de-214">SCEP Key Size.</span></span> <span data-ttu-id="8f4de-215">Os valores possíveis são: `size1024` e `size2048`.</span><span class="sxs-lookup"><span data-stu-id="8f4de-215">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="8f4de-216">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="8f4de-216">hashAlgorithm</span></span>|[<span data-ttu-id="8f4de-217">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="8f4de-217">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="8f4de-218">Algoritmo de Hash SCEP.</span><span class="sxs-lookup"><span data-stu-id="8f4de-218">SCEP Hash Algorithm.</span></span> <span data-ttu-id="8f4de-219">Os valores possíveis são: `sha1` e `sha2`.</span><span class="sxs-lookup"><span data-stu-id="8f4de-219">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="8f4de-220">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="8f4de-220">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="8f4de-221">String</span><span class="sxs-lookup"><span data-stu-id="8f4de-221">String</span></span>|<span data-ttu-id="8f4de-222">Cadeia de caracteres personalizada que define o atributo AAD.</span><span class="sxs-lookup"><span data-stu-id="8f4de-222">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="8f4de-223">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f4de-223">Response</span></span>
<span data-ttu-id="8f4de-224">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8f4de-224">If successful, this method returns a `201 Created` response code and a [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f4de-225">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8f4de-225">Example</span></span>
### <a name="request"></a><span data-ttu-id="8f4de-226">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8f4de-226">Request</span></span>
<span data-ttu-id="8f4de-227">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8f4de-227">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1096

{
  "@odata.type": "#microsoft.graph.windowsPhone81SCEPCertificateProfile",
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
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```

### <a name="response"></a><span data-ttu-id="8f4de-228">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f4de-228">Response</span></span>
<span data-ttu-id="8f4de-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8f4de-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1204

{
  "@odata.type": "#microsoft.graph.windowsPhone81SCEPCertificateProfile",
  "id": "f070e30e-e30e-f070-0ee3-70f00ee370f0",
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
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```





