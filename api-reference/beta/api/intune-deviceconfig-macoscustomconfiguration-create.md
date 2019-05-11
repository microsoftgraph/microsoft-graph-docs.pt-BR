---
title: Criar macOSCustomConfiguration
description: Cria um novo objeto macOSCustomConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 91a255b6e0b638afa66c33193215e7e8fdd03f27
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33922961"
---
# <a name="create-macoscustomconfiguration"></a><span data-ttu-id="a2245-103">Criar macOSCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="a2245-103">Create macOSCustomConfiguration</span></span>

> <span data-ttu-id="a2245-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a2245-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a2245-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a2245-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2245-106">Cria um novo objeto [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a2245-106">Create a new [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a2245-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a2245-107">Prerequisites</span></span>
<span data-ttu-id="a2245-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2245-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2245-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a2245-110">Permission type</span></span>|<span data-ttu-id="a2245-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a2245-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2245-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a2245-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a2245-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2245-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a2245-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a2245-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2245-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a2245-115">Not supported.</span></span>|
|<span data-ttu-id="a2245-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a2245-116">Application</span></span>|<span data-ttu-id="a2245-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a2245-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2245-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a2245-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a2245-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a2245-119">Request headers</span></span>
|<span data-ttu-id="a2245-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a2245-120">Header</span></span>|<span data-ttu-id="a2245-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a2245-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a2245-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a2245-122">Authorization</span></span>|<span data-ttu-id="a2245-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a2245-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a2245-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a2245-124">Accept</span></span>|<span data-ttu-id="a2245-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a2245-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2245-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a2245-126">Request body</span></span>
<span data-ttu-id="a2245-127">No corpo da solicitação, forneça uma representação JSON do objeto macOSCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="a2245-127">In the request body, supply a JSON representation for the macOSCustomConfiguration object.</span></span>

<span data-ttu-id="a2245-128">A tabela a seguir mostra as propriedades que são necessárias ao criar macOSCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="a2245-128">The following table shows the properties that are required when you create the macOSCustomConfiguration.</span></span>

|<span data-ttu-id="a2245-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a2245-129">Property</span></span>|<span data-ttu-id="a2245-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a2245-130">Type</span></span>|<span data-ttu-id="a2245-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2245-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2245-132">id</span><span class="sxs-lookup"><span data-stu-id="a2245-132">id</span></span>|<span data-ttu-id="a2245-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a2245-133">String</span></span>|<span data-ttu-id="a2245-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a2245-134">Key of the entity.</span></span> <span data-ttu-id="a2245-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a2245-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a2245-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a2245-136">lastModifiedDateTime</span></span>|<span data-ttu-id="a2245-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2245-137">DateTimeOffset</span></span>|<span data-ttu-id="a2245-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="a2245-138">DateTime the object was last modified.</span></span> <span data-ttu-id="a2245-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a2245-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a2245-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a2245-140">roleScopeTagIds</span></span>|<span data-ttu-id="a2245-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a2245-141">String collection</span></span>|<span data-ttu-id="a2245-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="a2245-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a2245-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a2245-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a2245-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a2245-144">supportsScopeTags</span></span>|<span data-ttu-id="a2245-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="a2245-145">Boolean</span></span>|<span data-ttu-id="a2245-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="a2245-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a2245-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="a2245-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a2245-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="a2245-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a2245-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a2245-149">This property is read-only.</span></span> <span data-ttu-id="a2245-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a2245-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a2245-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a2245-151">createdDateTime</span></span>|<span data-ttu-id="a2245-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2245-152">DateTimeOffset</span></span>|<span data-ttu-id="a2245-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="a2245-153">DateTime the object was created.</span></span> <span data-ttu-id="a2245-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a2245-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a2245-155">description</span><span class="sxs-lookup"><span data-stu-id="a2245-155">description</span></span>|<span data-ttu-id="a2245-156">String</span><span class="sxs-lookup"><span data-stu-id="a2245-156">String</span></span>|<span data-ttu-id="a2245-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a2245-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a2245-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a2245-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a2245-159">displayName</span><span class="sxs-lookup"><span data-stu-id="a2245-159">displayName</span></span>|<span data-ttu-id="a2245-160">String</span><span class="sxs-lookup"><span data-stu-id="a2245-160">String</span></span>|<span data-ttu-id="a2245-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a2245-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a2245-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a2245-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a2245-163">versão</span><span class="sxs-lookup"><span data-stu-id="a2245-163">version</span></span>|<span data-ttu-id="a2245-164">Int32</span><span class="sxs-lookup"><span data-stu-id="a2245-164">Int32</span></span>|<span data-ttu-id="a2245-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a2245-165">Version of the device configuration.</span></span> <span data-ttu-id="a2245-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a2245-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a2245-167">payloadName</span><span class="sxs-lookup"><span data-stu-id="a2245-167">payloadName</span></span>|<span data-ttu-id="a2245-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a2245-168">String</span></span>|<span data-ttu-id="a2245-169">Nome que é exibido para o usuário.</span><span class="sxs-lookup"><span data-stu-id="a2245-169">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="a2245-170">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="a2245-170">payloadFileName</span></span>|<span data-ttu-id="a2245-171">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a2245-171">String</span></span>|<span data-ttu-id="a2245-172">O nome do arquivo de carga (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="a2245-172">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="a2245-173">\*.xml).</span><span class="sxs-lookup"><span data-stu-id="a2245-173">\*.xml).</span></span>|
|<span data-ttu-id="a2245-174">payload</span><span class="sxs-lookup"><span data-stu-id="a2245-174">payload</span></span>|<span data-ttu-id="a2245-175">Binária</span><span class="sxs-lookup"><span data-stu-id="a2245-175">Binary</span></span>|<span data-ttu-id="a2245-176">Carga.</span><span class="sxs-lookup"><span data-stu-id="a2245-176">Payload.</span></span> <span data-ttu-id="a2245-177">(Matriz de bytes codificados em UTF8)</span><span class="sxs-lookup"><span data-stu-id="a2245-177">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="a2245-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2245-178">Response</span></span>
<span data-ttu-id="a2245-179">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a2245-179">If successful, this method returns a `201 Created` response code and a [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2245-180">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a2245-180">Example</span></span>

### <a name="request"></a><span data-ttu-id="a2245-181">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a2245-181">Request</span></span>
<span data-ttu-id="a2245-182">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a2245-182">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 373

{
  "@odata.type": "#microsoft.graph.macOSCustomConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "payloadName": "Payload Name value",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA=="
}
```

### <a name="response"></a><span data-ttu-id="a2245-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2245-183">Response</span></span>
<span data-ttu-id="a2245-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a2245-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 545

{
  "@odata.type": "#microsoft.graph.macOSCustomConfiguration",
  "id": "a253835d-835d-a253-5d83-53a25d8353a2",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "payloadName": "Payload Name value",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA=="
}
```




