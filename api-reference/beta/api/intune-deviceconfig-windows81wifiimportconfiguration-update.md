---
title: Atualizar windows81WifiImportConfiguration
description: Atualiza as propriedades de um objeto windows81WifiImportConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3163018e7f8822dbdf151f19949bf1be626c0f66
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30162864"
---
# <a name="update-windows81wifiimportconfiguration"></a><span data-ttu-id="e4222-103">Atualizar windows81WifiImportConfiguration</span><span class="sxs-lookup"><span data-stu-id="e4222-103">Update windows81WifiImportConfiguration</span></span>

> <span data-ttu-id="e4222-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e4222-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e4222-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e4222-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4222-106">Atualiza as propriedades de um objeto [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="e4222-106">Update the properties of a [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e4222-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e4222-107">Prerequisites</span></span>
<span data-ttu-id="e4222-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e4222-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e4222-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e4222-110">Permission type</span></span>|<span data-ttu-id="e4222-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e4222-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e4222-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e4222-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e4222-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4222-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e4222-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e4222-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4222-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e4222-115">Not supported.</span></span>|
|<span data-ttu-id="e4222-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e4222-116">Application</span></span>|<span data-ttu-id="e4222-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e4222-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e4222-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e4222-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="e4222-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e4222-119">Request headers</span></span>
|<span data-ttu-id="e4222-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e4222-120">Header</span></span>|<span data-ttu-id="e4222-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e4222-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e4222-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e4222-122">Authorization</span></span>|<span data-ttu-id="e4222-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e4222-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e4222-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e4222-124">Accept</span></span>|<span data-ttu-id="e4222-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e4222-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4222-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e4222-126">Request body</span></span>
<span data-ttu-id="e4222-127">No corpo da solicitação, forneça uma representação JSON do objeto [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="e4222-127">In the request body, supply a JSON representation for the [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) object.</span></span>

<span data-ttu-id="e4222-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e4222-128">The following table shows the properties that are required when you create the [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md).</span></span>

|<span data-ttu-id="e4222-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e4222-129">Property</span></span>|<span data-ttu-id="e4222-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="e4222-130">Type</span></span>|<span data-ttu-id="e4222-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4222-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4222-132">id</span><span class="sxs-lookup"><span data-stu-id="e4222-132">id</span></span>|<span data-ttu-id="e4222-133">String</span><span class="sxs-lookup"><span data-stu-id="e4222-133">String</span></span>|<span data-ttu-id="e4222-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e4222-134">Key of the entity.</span></span> <span data-ttu-id="e4222-135">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e4222-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e4222-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e4222-136">lastModifiedDateTime</span></span>|<span data-ttu-id="e4222-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4222-137">DateTimeOffset</span></span>|<span data-ttu-id="e4222-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="e4222-138">DateTime the object was last modified.</span></span> <span data-ttu-id="e4222-139">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e4222-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e4222-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e4222-140">roleScopeTagIds</span></span>|<span data-ttu-id="e4222-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e4222-141">String collection</span></span>|<span data-ttu-id="e4222-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="e4222-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e4222-143">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e4222-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e4222-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="e4222-144">supportsScopeTags</span></span>|<span data-ttu-id="e4222-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="e4222-145">Boolean</span></span>|<span data-ttu-id="e4222-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="e4222-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e4222-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="e4222-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e4222-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="e4222-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e4222-149">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e4222-149">This property is read-only.</span></span> <span data-ttu-id="e4222-150">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e4222-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e4222-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e4222-151">createdDateTime</span></span>|<span data-ttu-id="e4222-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4222-152">DateTimeOffset</span></span>|<span data-ttu-id="e4222-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="e4222-153">DateTime the object was created.</span></span> <span data-ttu-id="e4222-154">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e4222-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e4222-155">description</span><span class="sxs-lookup"><span data-stu-id="e4222-155">description</span></span>|<span data-ttu-id="e4222-156">String</span><span class="sxs-lookup"><span data-stu-id="e4222-156">String</span></span>|<span data-ttu-id="e4222-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e4222-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e4222-158">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e4222-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e4222-159">displayName</span><span class="sxs-lookup"><span data-stu-id="e4222-159">displayName</span></span>|<span data-ttu-id="e4222-160">String</span><span class="sxs-lookup"><span data-stu-id="e4222-160">String</span></span>|<span data-ttu-id="e4222-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e4222-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e4222-162">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e4222-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e4222-163">version</span><span class="sxs-lookup"><span data-stu-id="e4222-163">version</span></span>|<span data-ttu-id="e4222-164">Int32</span><span class="sxs-lookup"><span data-stu-id="e4222-164">Int32</span></span>|<span data-ttu-id="e4222-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e4222-165">Version of the device configuration.</span></span> <span data-ttu-id="e4222-166">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e4222-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e4222-167">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="e4222-167">payloadFileName</span></span>|<span data-ttu-id="e4222-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e4222-168">String</span></span>|<span data-ttu-id="e4222-169">Nome do arquivo de carga (\*. xml).</span><span class="sxs-lookup"><span data-stu-id="e4222-169">Payload file name (\*.xml).</span></span>|
|<span data-ttu-id="e4222-170">ProfileName</span><span class="sxs-lookup"><span data-stu-id="e4222-170">profileName</span></span>|<span data-ttu-id="e4222-171">String</span><span class="sxs-lookup"><span data-stu-id="e4222-171">String</span></span>|<span data-ttu-id="e4222-172">Nome do perfil exibido na interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="e4222-172">Profile name displayed in the UI.</span></span>|
|<span data-ttu-id="e4222-173">payload</span><span class="sxs-lookup"><span data-stu-id="e4222-173">payload</span></span>|<span data-ttu-id="e4222-174">Binária</span><span class="sxs-lookup"><span data-stu-id="e4222-174">Binary</span></span>|<span data-ttu-id="e4222-175">Carga.</span><span class="sxs-lookup"><span data-stu-id="e4222-175">Payload.</span></span> <span data-ttu-id="e4222-176">(Matriz de bytes codificados por UTF8).</span><span class="sxs-lookup"><span data-stu-id="e4222-176">(UTF8 encoded byte array).</span></span> <span data-ttu-id="e4222-177">Este é o arquivo XML salvo no dispositivo que você usou para se conectar ao ponto de extremidade Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="e4222-177">This is the XML file saved on the device you used to connect to the Wi-Fi endpoint.</span></span>|



## <a name="response"></a><span data-ttu-id="e4222-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4222-178">Response</span></span>
<span data-ttu-id="e4222-179">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e4222-179">If successful, this method returns a `200 OK` response code and an updated [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4222-180">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e4222-180">Example</span></span>

### <a name="request"></a><span data-ttu-id="e4222-181">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e4222-181">Request</span></span>
<span data-ttu-id="e4222-182">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e4222-182">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 381

{
  "@odata.type": "#microsoft.graph.windows81WifiImportConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "payloadFileName": "Payload File Name value",
  "profileName": "Profile Name value",
  "payload": "cGF5bG9hZA=="
}
```

### <a name="response"></a><span data-ttu-id="e4222-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4222-183">Response</span></span>
<span data-ttu-id="e4222-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e4222-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 553

{
  "@odata.type": "#microsoft.graph.windows81WifiImportConfiguration",
  "id": "534a2f07-2f07-534a-072f-4a53072f4a53",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "payloadFileName": "Payload File Name value",
  "profileName": "Profile Name value",
  "payload": "cGF5bG9hZA=="
}
```




