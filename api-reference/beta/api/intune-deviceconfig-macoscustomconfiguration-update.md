---
title: Atualizar macOSCustomConfiguration
description: Atualizar as propriedades de um objeto macOSCustomConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 22d7ebd743a9cd90ce5fdfd408de5113b1bb4e88
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30171250"
---
# <a name="update-macoscustomconfiguration"></a><span data-ttu-id="8133d-103">Atualizar macOSCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="8133d-103">Update macOSCustomConfiguration</span></span>

> <span data-ttu-id="8133d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8133d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8133d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8133d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8133d-106">Atualizar as propriedades de um objeto [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8133d-106">Update the properties of a [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8133d-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8133d-107">Prerequisites</span></span>
<span data-ttu-id="8133d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="8133d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="8133d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8133d-110">Permission type</span></span>|<span data-ttu-id="8133d-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8133d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8133d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8133d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8133d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8133d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8133d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8133d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8133d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8133d-115">Not supported.</span></span>|
|<span data-ttu-id="8133d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8133d-116">Application</span></span>|<span data-ttu-id="8133d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8133d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8133d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8133d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="8133d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8133d-119">Request headers</span></span>
|<span data-ttu-id="8133d-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8133d-120">Header</span></span>|<span data-ttu-id="8133d-121">Valor</span><span class="sxs-lookup"><span data-stu-id="8133d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8133d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8133d-122">Authorization</span></span>|<span data-ttu-id="8133d-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8133d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8133d-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8133d-124">Accept</span></span>|<span data-ttu-id="8133d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8133d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8133d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8133d-126">Request body</span></span>
<span data-ttu-id="8133d-127">No corpo da solicitação, forneça uma representação JSON do objeto [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8133d-127">In the request body, supply a JSON representation for the [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object.</span></span>

<span data-ttu-id="8133d-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8133d-128">The following table shows the properties that are required when you create the [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md).</span></span>

|<span data-ttu-id="8133d-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8133d-129">Property</span></span>|<span data-ttu-id="8133d-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="8133d-130">Type</span></span>|<span data-ttu-id="8133d-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="8133d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8133d-132">id</span><span class="sxs-lookup"><span data-stu-id="8133d-132">id</span></span>|<span data-ttu-id="8133d-133">String</span><span class="sxs-lookup"><span data-stu-id="8133d-133">String</span></span>|<span data-ttu-id="8133d-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="8133d-134">Key of the entity.</span></span> <span data-ttu-id="8133d-135">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8133d-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8133d-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8133d-136">lastModifiedDateTime</span></span>|<span data-ttu-id="8133d-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8133d-137">DateTimeOffset</span></span>|<span data-ttu-id="8133d-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="8133d-138">DateTime the object was last modified.</span></span> <span data-ttu-id="8133d-139">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8133d-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8133d-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8133d-140">roleScopeTagIds</span></span>|<span data-ttu-id="8133d-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="8133d-141">String collection</span></span>|<span data-ttu-id="8133d-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="8133d-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8133d-143">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8133d-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8133d-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="8133d-144">supportsScopeTags</span></span>|<span data-ttu-id="8133d-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="8133d-145">Boolean</span></span>|<span data-ttu-id="8133d-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="8133d-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="8133d-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="8133d-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="8133d-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="8133d-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="8133d-149">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8133d-149">This property is read-only.</span></span> <span data-ttu-id="8133d-150">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8133d-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8133d-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8133d-151">createdDateTime</span></span>|<span data-ttu-id="8133d-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8133d-152">DateTimeOffset</span></span>|<span data-ttu-id="8133d-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="8133d-153">DateTime the object was created.</span></span> <span data-ttu-id="8133d-154">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8133d-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8133d-155">description</span><span class="sxs-lookup"><span data-stu-id="8133d-155">description</span></span>|<span data-ttu-id="8133d-156">String</span><span class="sxs-lookup"><span data-stu-id="8133d-156">String</span></span>|<span data-ttu-id="8133d-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8133d-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8133d-158">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8133d-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8133d-159">displayName</span><span class="sxs-lookup"><span data-stu-id="8133d-159">displayName</span></span>|<span data-ttu-id="8133d-160">String</span><span class="sxs-lookup"><span data-stu-id="8133d-160">String</span></span>|<span data-ttu-id="8133d-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8133d-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8133d-162">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8133d-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8133d-163">version</span><span class="sxs-lookup"><span data-stu-id="8133d-163">version</span></span>|<span data-ttu-id="8133d-164">Int32</span><span class="sxs-lookup"><span data-stu-id="8133d-164">Int32</span></span>|<span data-ttu-id="8133d-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8133d-165">Version of the device configuration.</span></span> <span data-ttu-id="8133d-166">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8133d-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8133d-167">payloadName</span><span class="sxs-lookup"><span data-stu-id="8133d-167">payloadName</span></span>|<span data-ttu-id="8133d-168">String</span><span class="sxs-lookup"><span data-stu-id="8133d-168">String</span></span>|<span data-ttu-id="8133d-169">Nome que é exibido para o usuário.</span><span class="sxs-lookup"><span data-stu-id="8133d-169">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="8133d-170">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="8133d-170">payloadFileName</span></span>|<span data-ttu-id="8133d-171">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8133d-171">String</span></span>|<span data-ttu-id="8133d-172">O nome do arquivo de carga (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="8133d-172">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="8133d-173">\*.xml).</span><span class="sxs-lookup"><span data-stu-id="8133d-173">\*.xml).</span></span>|
|<span data-ttu-id="8133d-174">payload</span><span class="sxs-lookup"><span data-stu-id="8133d-174">payload</span></span>|<span data-ttu-id="8133d-175">Binária</span><span class="sxs-lookup"><span data-stu-id="8133d-175">Binary</span></span>|<span data-ttu-id="8133d-176">Carga.</span><span class="sxs-lookup"><span data-stu-id="8133d-176">Payload.</span></span> <span data-ttu-id="8133d-177">(Matriz de bytes codificados em UTF8)</span><span class="sxs-lookup"><span data-stu-id="8133d-177">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="8133d-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="8133d-178">Response</span></span>
<span data-ttu-id="8133d-179">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8133d-179">If successful, this method returns a `200 OK` response code and an updated [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8133d-180">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8133d-180">Example</span></span>

### <a name="request"></a><span data-ttu-id="8133d-181">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8133d-181">Request</span></span>
<span data-ttu-id="8133d-182">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8133d-182">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="8133d-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="8133d-183">Response</span></span>
<span data-ttu-id="8133d-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8133d-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




