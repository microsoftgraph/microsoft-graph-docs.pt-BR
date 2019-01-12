---
title: Atualizar iosImportedPFXCertificateProfile
description: Atualize as propriedades de um objeto iosImportedPFXCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 19c8eaabd05bcafa545bdfa93677c68df9f28dfb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27929680"
---
# <a name="update-iosimportedpfxcertificateprofile"></a><span data-ttu-id="efefd-103">Atualizar iosImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="efefd-103">Update iosImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="efefd-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="efefd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="efefd-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="efefd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="efefd-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="efefd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="efefd-107">Atualize as propriedades de um objeto [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="efefd-107">Update the properties of a [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="efefd-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="efefd-108">Prerequisites</span></span>
<span data-ttu-id="efefd-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="efefd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="efefd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="efefd-111">Permission type</span></span>|<span data-ttu-id="efefd-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="efefd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="efefd-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="efefd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="efefd-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efefd-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="efefd-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="efefd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="efefd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="efefd-116">Not supported.</span></span>|
|<span data-ttu-id="efefd-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="efefd-117">Application</span></span>|<span data-ttu-id="efefd-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="efefd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="efefd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="efefd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="efefd-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="efefd-120">Request headers</span></span>
|<span data-ttu-id="efefd-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="efefd-121">Header</span></span>|<span data-ttu-id="efefd-122">Valor</span><span class="sxs-lookup"><span data-stu-id="efefd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="efefd-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="efefd-123">Authorization</span></span>|<span data-ttu-id="efefd-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="efefd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="efefd-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="efefd-125">Accept</span></span>|<span data-ttu-id="efefd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="efefd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="efefd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="efefd-127">Request body</span></span>
<span data-ttu-id="efefd-128">No corpo da solicitação, fornece uma representação JSON para o objeto [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="efefd-128">In the request body, supply a JSON representation for the [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) object.</span></span>

<span data-ttu-id="efefd-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="efefd-129">The following table shows the properties that are required when you create the [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md).</span></span>

|<span data-ttu-id="efefd-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="efefd-130">Property</span></span>|<span data-ttu-id="efefd-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="efefd-131">Type</span></span>|<span data-ttu-id="efefd-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="efefd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="efefd-133">id</span><span class="sxs-lookup"><span data-stu-id="efefd-133">id</span></span>|<span data-ttu-id="efefd-134">String</span><span class="sxs-lookup"><span data-stu-id="efefd-134">String</span></span>|<span data-ttu-id="efefd-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="efefd-135">Key of the entity.</span></span> <span data-ttu-id="efefd-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="efefd-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="efefd-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="efefd-137">lastModifiedDateTime</span></span>|<span data-ttu-id="efefd-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="efefd-138">DateTimeOffset</span></span>|<span data-ttu-id="efefd-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="efefd-139">DateTime the object was last modified.</span></span> <span data-ttu-id="efefd-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="efefd-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="efefd-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="efefd-141">roleScopeTagIds</span></span>|<span data-ttu-id="efefd-142">String collection</span><span class="sxs-lookup"><span data-stu-id="efefd-142">String collection</span></span>|<span data-ttu-id="efefd-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="efefd-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="efefd-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="efefd-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="efefd-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="efefd-145">supportsScopeTags</span></span>|<span data-ttu-id="efefd-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="efefd-146">Boolean</span></span>|<span data-ttu-id="efefd-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="efefd-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="efefd-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="efefd-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="efefd-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="efefd-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="efefd-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efefd-150">This property is read-only.</span></span> <span data-ttu-id="efefd-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="efefd-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="efefd-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="efefd-152">createdDateTime</span></span>|<span data-ttu-id="efefd-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="efefd-153">DateTimeOffset</span></span>|<span data-ttu-id="efefd-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="efefd-154">DateTime the object was created.</span></span> <span data-ttu-id="efefd-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="efefd-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="efefd-156">description</span><span class="sxs-lookup"><span data-stu-id="efefd-156">description</span></span>|<span data-ttu-id="efefd-157">String</span><span class="sxs-lookup"><span data-stu-id="efefd-157">String</span></span>|<span data-ttu-id="efefd-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="efefd-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="efefd-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="efefd-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="efefd-160">displayName</span><span class="sxs-lookup"><span data-stu-id="efefd-160">displayName</span></span>|<span data-ttu-id="efefd-161">String</span><span class="sxs-lookup"><span data-stu-id="efefd-161">String</span></span>|<span data-ttu-id="efefd-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="efefd-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="efefd-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="efefd-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="efefd-164">version</span><span class="sxs-lookup"><span data-stu-id="efefd-164">version</span></span>|<span data-ttu-id="efefd-165">Int32</span><span class="sxs-lookup"><span data-stu-id="efefd-165">Int32</span></span>|<span data-ttu-id="efefd-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="efefd-166">Version of the device configuration.</span></span> <span data-ttu-id="efefd-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="efefd-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="efefd-168">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="efefd-168">intendedPurpose</span></span>|[<span data-ttu-id="efefd-169">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="efefd-169">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="efefd-170">Ainda não documentado.</span><span class="sxs-lookup"><span data-stu-id="efefd-170">Not yet documented.</span></span> <span data-ttu-id="efefd-171">Os valores possíveis são: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span><span class="sxs-lookup"><span data-stu-id="efefd-171">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="efefd-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="efefd-172">Response</span></span>
<span data-ttu-id="efefd-173">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="efefd-173">If successful, this method returns a `200 OK` response code and an updated [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="efefd-174">Exemplo</span><span class="sxs-lookup"><span data-stu-id="efefd-174">Example</span></span>
### <a name="request"></a><span data-ttu-id="efefd-175">Solicitação</span><span class="sxs-lookup"><span data-stu-id="efefd-175">Request</span></span>
<span data-ttu-id="efefd-176">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="efefd-176">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 296

{
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

### <a name="response"></a><span data-ttu-id="efefd-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="efefd-177">Response</span></span>
<span data-ttu-id="efefd-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="efefd-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





