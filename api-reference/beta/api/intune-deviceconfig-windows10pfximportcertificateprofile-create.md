---
title: Criar windows10PFXImportCertificateProfile
description: Criar um novo objeto windows10PFXImportCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 005b7640ec189fe47a76411a47158c1de1a33d69
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32516076"
---
# <a name="create-windows10pfximportcertificateprofile"></a><span data-ttu-id="4e822-103">Criar windows10PFXImportCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="4e822-103">Create windows10PFXImportCertificateProfile</span></span>

> <span data-ttu-id="4e822-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4e822-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4e822-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4e822-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e822-106">Criar um novo objeto [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="4e822-106">Create a new [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4e822-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4e822-107">Prerequisites</span></span>
<span data-ttu-id="4e822-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e822-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e822-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4e822-110">Permission type</span></span>|<span data-ttu-id="4e822-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4e822-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4e822-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4e822-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4e822-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e822-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4e822-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4e822-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4e822-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4e822-115">Not supported.</span></span>|
|<span data-ttu-id="4e822-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4e822-116">Application</span></span>|<span data-ttu-id="4e822-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4e822-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e822-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4e822-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4e822-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4e822-119">Request headers</span></span>
|<span data-ttu-id="4e822-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4e822-120">Header</span></span>|<span data-ttu-id="4e822-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4e822-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4e822-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4e822-122">Authorization</span></span>|<span data-ttu-id="4e822-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4e822-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4e822-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4e822-124">Accept</span></span>|<span data-ttu-id="4e822-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4e822-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e822-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4e822-126">Request body</span></span>
<span data-ttu-id="4e822-127">No corpo da solicitação, forneça uma representação JSON do objeto windows10PFXImportCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="4e822-127">In the request body, supply a JSON representation for the windows10PFXImportCertificateProfile object.</span></span>

<span data-ttu-id="4e822-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windows10PFXImportCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="4e822-128">The following table shows the properties that are required when you create the windows10PFXImportCertificateProfile.</span></span>

|<span data-ttu-id="4e822-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4e822-129">Property</span></span>|<span data-ttu-id="4e822-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="4e822-130">Type</span></span>|<span data-ttu-id="4e822-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="4e822-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e822-132">id</span><span class="sxs-lookup"><span data-stu-id="4e822-132">id</span></span>|<span data-ttu-id="4e822-133">String</span><span class="sxs-lookup"><span data-stu-id="4e822-133">String</span></span>|<span data-ttu-id="4e822-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4e822-134">Key of the entity.</span></span> <span data-ttu-id="4e822-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4e822-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4e822-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4e822-136">lastModifiedDateTime</span></span>|<span data-ttu-id="4e822-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e822-137">DateTimeOffset</span></span>|<span data-ttu-id="4e822-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="4e822-138">DateTime the object was last modified.</span></span> <span data-ttu-id="4e822-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4e822-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4e822-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4e822-140">roleScopeTagIds</span></span>|<span data-ttu-id="4e822-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="4e822-141">String collection</span></span>|<span data-ttu-id="4e822-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="4e822-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4e822-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4e822-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4e822-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="4e822-144">supportsScopeTags</span></span>|<span data-ttu-id="4e822-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="4e822-145">Boolean</span></span>|<span data-ttu-id="4e822-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="4e822-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4e822-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="4e822-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4e822-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="4e822-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4e822-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4e822-149">This property is read-only.</span></span> <span data-ttu-id="4e822-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4e822-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4e822-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4e822-151">createdDateTime</span></span>|<span data-ttu-id="4e822-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e822-152">DateTimeOffset</span></span>|<span data-ttu-id="4e822-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="4e822-153">DateTime the object was created.</span></span> <span data-ttu-id="4e822-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4e822-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4e822-155">description</span><span class="sxs-lookup"><span data-stu-id="4e822-155">description</span></span>|<span data-ttu-id="4e822-156">String</span><span class="sxs-lookup"><span data-stu-id="4e822-156">String</span></span>|<span data-ttu-id="4e822-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4e822-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4e822-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4e822-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4e822-159">displayName</span><span class="sxs-lookup"><span data-stu-id="4e822-159">displayName</span></span>|<span data-ttu-id="4e822-160">String</span><span class="sxs-lookup"><span data-stu-id="4e822-160">String</span></span>|<span data-ttu-id="4e822-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4e822-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4e822-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4e822-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4e822-163">versão</span><span class="sxs-lookup"><span data-stu-id="4e822-163">version</span></span>|<span data-ttu-id="4e822-164">Int32</span><span class="sxs-lookup"><span data-stu-id="4e822-164">Int32</span></span>|<span data-ttu-id="4e822-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4e822-165">Version of the device configuration.</span></span> <span data-ttu-id="4e822-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4e822-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4e822-167">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="4e822-167">keyStorageProvider</span></span>|[<span data-ttu-id="4e822-168">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="4e822-168">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="4e822-169">Ainda não documentado.</span><span class="sxs-lookup"><span data-stu-id="4e822-169">Not yet documented.</span></span> <span data-ttu-id="4e822-170">Os valores possíveis são: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="4e822-170">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|



## <a name="response"></a><span data-ttu-id="4e822-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="4e822-171">Response</span></span>
<span data-ttu-id="4e822-172">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4e822-172">If successful, this method returns a `201 Created` response code and a [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e822-173">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4e822-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="4e822-174">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4e822-174">Request</span></span>
<span data-ttu-id="4e822-175">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4e822-175">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 317

{
  "@odata.type": "#microsoft.graph.windows10PFXImportCertificateProfile",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "keyStorageProvider": "useTpmKspOtherwiseFail"
}
```

### <a name="response"></a><span data-ttu-id="4e822-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="4e822-176">Response</span></span>
<span data-ttu-id="4e822-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4e822-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 489

{
  "@odata.type": "#microsoft.graph.windows10PFXImportCertificateProfile",
  "id": "4244277a-277a-4244-7a27-44427a274442",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "keyStorageProvider": "useTpmKspOtherwiseFail"
}
```





