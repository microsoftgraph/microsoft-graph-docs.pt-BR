---
title: Criar iosImportedPFXCertificateProfile
description: Crie um novo objeto de iosImportedPFXCertificateProfile.
ms.openlocfilehash: 1d5b73a3c3548b0e94dcf7e0675662a1ed8ca611
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039514"
---
# <a name="create-iosimportedpfxcertificateprofile"></a><span data-ttu-id="44f08-103">Criar iosImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="44f08-103">Create iosImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="44f08-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="44f08-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="44f08-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="44f08-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="44f08-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="44f08-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="44f08-107">Crie um novo objeto de [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="44f08-107">Create a new [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="44f08-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="44f08-108">Prerequisites</span></span>
<span data-ttu-id="44f08-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44f08-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44f08-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="44f08-111">Permission type</span></span>|<span data-ttu-id="44f08-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="44f08-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="44f08-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="44f08-113">Delegated (work or school account)</span></span>|<span data-ttu-id="44f08-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44f08-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="44f08-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="44f08-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="44f08-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="44f08-116">Not supported.</span></span>|
|<span data-ttu-id="44f08-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="44f08-117">Application</span></span>|<span data-ttu-id="44f08-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="44f08-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="44f08-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="44f08-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="44f08-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="44f08-120">Request headers</span></span>
|<span data-ttu-id="44f08-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="44f08-121">Header</span></span>|<span data-ttu-id="44f08-122">Valor</span><span class="sxs-lookup"><span data-stu-id="44f08-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="44f08-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="44f08-123">Authorization</span></span>|<span data-ttu-id="44f08-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="44f08-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="44f08-125">Accept</span><span class="sxs-lookup"><span data-stu-id="44f08-125">Accept</span></span>|<span data-ttu-id="44f08-126">application/json</span><span class="sxs-lookup"><span data-stu-id="44f08-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="44f08-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="44f08-127">Request body</span></span>
<span data-ttu-id="44f08-128">No corpo da solicitação, fornece uma representação JSON para o objeto iosImportedPFXCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="44f08-128">In the request body, supply a JSON representation for the iosImportedPFXCertificateProfile object.</span></span>

<span data-ttu-id="44f08-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o iosImportedPFXCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="44f08-129">The following table shows the properties that are required when you create the iosImportedPFXCertificateProfile.</span></span>

|<span data-ttu-id="44f08-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="44f08-130">Property</span></span>|<span data-ttu-id="44f08-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="44f08-131">Type</span></span>|<span data-ttu-id="44f08-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="44f08-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44f08-133">id</span><span class="sxs-lookup"><span data-stu-id="44f08-133">id</span></span>|<span data-ttu-id="44f08-134">String</span><span class="sxs-lookup"><span data-stu-id="44f08-134">String</span></span>|<span data-ttu-id="44f08-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="44f08-135">Key of the entity.</span></span> <span data-ttu-id="44f08-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44f08-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44f08-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="44f08-137">lastModifiedDateTime</span></span>|<span data-ttu-id="44f08-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44f08-138">DateTimeOffset</span></span>|<span data-ttu-id="44f08-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="44f08-139">DateTime the object was last modified.</span></span> <span data-ttu-id="44f08-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44f08-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44f08-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="44f08-141">roleScopeTagIds</span></span>|<span data-ttu-id="44f08-142">String collection</span><span class="sxs-lookup"><span data-stu-id="44f08-142">String collection</span></span>|<span data-ttu-id="44f08-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="44f08-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="44f08-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44f08-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44f08-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="44f08-145">supportsScopeTags</span></span>|<span data-ttu-id="44f08-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="44f08-146">Boolean</span></span>|<span data-ttu-id="44f08-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="44f08-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="44f08-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="44f08-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="44f08-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="44f08-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="44f08-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="44f08-150">This property is read-only.</span></span> <span data-ttu-id="44f08-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44f08-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44f08-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="44f08-152">createdDateTime</span></span>|<span data-ttu-id="44f08-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44f08-153">DateTimeOffset</span></span>|<span data-ttu-id="44f08-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="44f08-154">DateTime the object was created.</span></span> <span data-ttu-id="44f08-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44f08-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44f08-156">description</span><span class="sxs-lookup"><span data-stu-id="44f08-156">description</span></span>|<span data-ttu-id="44f08-157">String</span><span class="sxs-lookup"><span data-stu-id="44f08-157">String</span></span>|<span data-ttu-id="44f08-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="44f08-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="44f08-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44f08-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44f08-160">displayName</span><span class="sxs-lookup"><span data-stu-id="44f08-160">displayName</span></span>|<span data-ttu-id="44f08-161">String</span><span class="sxs-lookup"><span data-stu-id="44f08-161">String</span></span>|<span data-ttu-id="44f08-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="44f08-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="44f08-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44f08-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44f08-164">version</span><span class="sxs-lookup"><span data-stu-id="44f08-164">version</span></span>|<span data-ttu-id="44f08-165">Int32</span><span class="sxs-lookup"><span data-stu-id="44f08-165">Int32</span></span>|<span data-ttu-id="44f08-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="44f08-166">Version of the device configuration.</span></span> <span data-ttu-id="44f08-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44f08-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44f08-168">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="44f08-168">intendedPurpose</span></span>|[<span data-ttu-id="44f08-169">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="44f08-169">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="44f08-170">Ainda não documentado.</span><span class="sxs-lookup"><span data-stu-id="44f08-170">Not yet documented.</span></span> <span data-ttu-id="44f08-171">Os valores possíveis são: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span><span class="sxs-lookup"><span data-stu-id="44f08-171">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="44f08-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="44f08-172">Response</span></span>
<span data-ttu-id="44f08-173">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="44f08-173">If successful, this method returns a `201 Created` response code and a [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44f08-174">Exemplo</span><span class="sxs-lookup"><span data-stu-id="44f08-174">Example</span></span>
### <a name="request"></a><span data-ttu-id="44f08-175">Solicitação</span><span class="sxs-lookup"><span data-stu-id="44f08-175">Request</span></span>
<span data-ttu-id="44f08-176">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="44f08-176">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 367

{
  "@odata.type": "#microsoft.graph.iosImportedPFXCertificateProfile",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "intendedPurpose": "smimeEncryption"
}
```

### <a name="response"></a><span data-ttu-id="44f08-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="44f08-177">Response</span></span>
<span data-ttu-id="44f08-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="44f08-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 475

{
  "@odata.type": "#microsoft.graph.iosImportedPFXCertificateProfile",
  "id": "583b9d8c-9d8c-583b-8c9d-3b588c9d3b58",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "intendedPurpose": "smimeEncryption"
}
```





