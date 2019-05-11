---
title: Atualizar windows81WifiImportConfiguration
description: Atualiza as propriedades de um objeto windows81WifiImportConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 501168a6e4c98846091164012f5ed33756935d83
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33918091"
---
# <a name="update-windows81wifiimportconfiguration"></a><span data-ttu-id="ff949-103">Atualizar windows81WifiImportConfiguration</span><span class="sxs-lookup"><span data-stu-id="ff949-103">Update windows81WifiImportConfiguration</span></span>

> <span data-ttu-id="ff949-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ff949-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ff949-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ff949-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff949-106">Atualiza as propriedades de um objeto [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="ff949-106">Update the properties of a [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ff949-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ff949-107">Prerequisites</span></span>
<span data-ttu-id="ff949-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff949-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff949-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ff949-110">Permission type</span></span>|<span data-ttu-id="ff949-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ff949-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff949-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ff949-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ff949-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff949-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ff949-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ff949-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff949-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ff949-115">Not supported.</span></span>|
|<span data-ttu-id="ff949-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ff949-116">Application</span></span>|<span data-ttu-id="ff949-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ff949-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff949-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ff949-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ff949-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ff949-119">Request headers</span></span>
|<span data-ttu-id="ff949-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ff949-120">Header</span></span>|<span data-ttu-id="ff949-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ff949-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ff949-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ff949-122">Authorization</span></span>|<span data-ttu-id="ff949-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ff949-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ff949-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ff949-124">Accept</span></span>|<span data-ttu-id="ff949-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ff949-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff949-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ff949-126">Request body</span></span>
<span data-ttu-id="ff949-127">No corpo da solicitação, forneça uma representação JSON do objeto [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="ff949-127">In the request body, supply a JSON representation for the [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) object.</span></span>

<span data-ttu-id="ff949-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ff949-128">The following table shows the properties that are required when you create the [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md).</span></span>

|<span data-ttu-id="ff949-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ff949-129">Property</span></span>|<span data-ttu-id="ff949-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="ff949-130">Type</span></span>|<span data-ttu-id="ff949-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff949-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff949-132">id</span><span class="sxs-lookup"><span data-stu-id="ff949-132">id</span></span>|<span data-ttu-id="ff949-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ff949-133">String</span></span>|<span data-ttu-id="ff949-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ff949-134">Key of the entity.</span></span> <span data-ttu-id="ff949-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff949-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff949-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ff949-136">lastModifiedDateTime</span></span>|<span data-ttu-id="ff949-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff949-137">DateTimeOffset</span></span>|<span data-ttu-id="ff949-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="ff949-138">DateTime the object was last modified.</span></span> <span data-ttu-id="ff949-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff949-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff949-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ff949-140">roleScopeTagIds</span></span>|<span data-ttu-id="ff949-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ff949-141">String collection</span></span>|<span data-ttu-id="ff949-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="ff949-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ff949-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff949-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff949-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ff949-144">supportsScopeTags</span></span>|<span data-ttu-id="ff949-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="ff949-145">Boolean</span></span>|<span data-ttu-id="ff949-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="ff949-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ff949-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="ff949-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ff949-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="ff949-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ff949-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ff949-149">This property is read-only.</span></span> <span data-ttu-id="ff949-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff949-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff949-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ff949-151">createdDateTime</span></span>|<span data-ttu-id="ff949-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff949-152">DateTimeOffset</span></span>|<span data-ttu-id="ff949-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="ff949-153">DateTime the object was created.</span></span> <span data-ttu-id="ff949-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff949-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff949-155">description</span><span class="sxs-lookup"><span data-stu-id="ff949-155">description</span></span>|<span data-ttu-id="ff949-156">String</span><span class="sxs-lookup"><span data-stu-id="ff949-156">String</span></span>|<span data-ttu-id="ff949-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ff949-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ff949-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff949-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff949-159">displayName</span><span class="sxs-lookup"><span data-stu-id="ff949-159">displayName</span></span>|<span data-ttu-id="ff949-160">String</span><span class="sxs-lookup"><span data-stu-id="ff949-160">String</span></span>|<span data-ttu-id="ff949-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ff949-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ff949-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff949-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff949-163">versão</span><span class="sxs-lookup"><span data-stu-id="ff949-163">version</span></span>|<span data-ttu-id="ff949-164">Int32</span><span class="sxs-lookup"><span data-stu-id="ff949-164">Int32</span></span>|<span data-ttu-id="ff949-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ff949-165">Version of the device configuration.</span></span> <span data-ttu-id="ff949-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff949-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff949-167">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="ff949-167">payloadFileName</span></span>|<span data-ttu-id="ff949-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ff949-168">String</span></span>|<span data-ttu-id="ff949-169">Nome do arquivo de carga (\*. xml).</span><span class="sxs-lookup"><span data-stu-id="ff949-169">Payload file name (\*.xml).</span></span>|
|<span data-ttu-id="ff949-170">ProfileName</span><span class="sxs-lookup"><span data-stu-id="ff949-170">profileName</span></span>|<span data-ttu-id="ff949-171">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ff949-171">String</span></span>|<span data-ttu-id="ff949-172">Nome do perfil exibido na interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="ff949-172">Profile name displayed in the UI.</span></span>|
|<span data-ttu-id="ff949-173">payload</span><span class="sxs-lookup"><span data-stu-id="ff949-173">payload</span></span>|<span data-ttu-id="ff949-174">Binária</span><span class="sxs-lookup"><span data-stu-id="ff949-174">Binary</span></span>|<span data-ttu-id="ff949-175">Carga.</span><span class="sxs-lookup"><span data-stu-id="ff949-175">Payload.</span></span> <span data-ttu-id="ff949-176">(Matriz de bytes codificados por UTF8).</span><span class="sxs-lookup"><span data-stu-id="ff949-176">(UTF8 encoded byte array).</span></span> <span data-ttu-id="ff949-177">Este é o arquivo XML salvo no dispositivo que você usou para se conectar ao ponto de extremidade Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="ff949-177">This is the XML file saved on the device you used to connect to the Wi-Fi endpoint.</span></span>|



## <a name="response"></a><span data-ttu-id="ff949-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff949-178">Response</span></span>
<span data-ttu-id="ff949-179">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ff949-179">If successful, this method returns a `200 OK` response code and an updated [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff949-180">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ff949-180">Example</span></span>

### <a name="request"></a><span data-ttu-id="ff949-181">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ff949-181">Request</span></span>
<span data-ttu-id="ff949-182">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ff949-182">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ff949-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff949-183">Response</span></span>
<span data-ttu-id="ff949-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ff949-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




