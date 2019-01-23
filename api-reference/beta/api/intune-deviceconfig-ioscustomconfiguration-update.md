---
title: Atualizar iosCustomConfiguration
description: Atualizar as propriedades de um objeto iosCustomConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6c6a5d4e96aa05271d0cc6968df70bf8035b09c4
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415996"
---
# <a name="update-ioscustomconfiguration"></a><span data-ttu-id="6ba32-103">Atualizar iosCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="6ba32-103">Update iosCustomConfiguration</span></span>

> <span data-ttu-id="6ba32-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="6ba32-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6ba32-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6ba32-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6ba32-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="6ba32-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ba32-107">Atualizar as propriedades de um objeto [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6ba32-107">Update the properties of a [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6ba32-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6ba32-108">Prerequisites</span></span>
<span data-ttu-id="6ba32-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="6ba32-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6ba32-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6ba32-111">Permission type</span></span>|<span data-ttu-id="6ba32-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6ba32-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6ba32-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6ba32-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6ba32-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ba32-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6ba32-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6ba32-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6ba32-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6ba32-116">Not supported.</span></span>|
|<span data-ttu-id="6ba32-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6ba32-117">Application</span></span>|<span data-ttu-id="6ba32-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6ba32-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6ba32-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6ba32-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="6ba32-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6ba32-120">Request headers</span></span>
|<span data-ttu-id="6ba32-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6ba32-121">Header</span></span>|<span data-ttu-id="6ba32-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6ba32-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6ba32-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6ba32-123">Authorization</span></span>|<span data-ttu-id="6ba32-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6ba32-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6ba32-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6ba32-125">Accept</span></span>|<span data-ttu-id="6ba32-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6ba32-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ba32-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6ba32-127">Request body</span></span>
<span data-ttu-id="6ba32-128">No corpo da solicitação, forneça uma representação JSON do objeto [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6ba32-128">In the request body, supply a JSON representation for the [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object.</span></span>

<span data-ttu-id="6ba32-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6ba32-129">The following table shows the properties that are required when you create the [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).</span></span>

|<span data-ttu-id="6ba32-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6ba32-130">Property</span></span>|<span data-ttu-id="6ba32-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6ba32-131">Type</span></span>|<span data-ttu-id="6ba32-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6ba32-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ba32-133">id</span><span class="sxs-lookup"><span data-stu-id="6ba32-133">id</span></span>|<span data-ttu-id="6ba32-134">String</span><span class="sxs-lookup"><span data-stu-id="6ba32-134">String</span></span>|<span data-ttu-id="6ba32-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6ba32-135">Key of the entity.</span></span> <span data-ttu-id="6ba32-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ba32-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ba32-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6ba32-137">lastModifiedDateTime</span></span>|<span data-ttu-id="6ba32-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6ba32-138">DateTimeOffset</span></span>|<span data-ttu-id="6ba32-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="6ba32-139">DateTime the object was last modified.</span></span> <span data-ttu-id="6ba32-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ba32-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ba32-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6ba32-141">roleScopeTagIds</span></span>|<span data-ttu-id="6ba32-142">String collection</span><span class="sxs-lookup"><span data-stu-id="6ba32-142">String collection</span></span>|<span data-ttu-id="6ba32-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="6ba32-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6ba32-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ba32-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ba32-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6ba32-145">supportsScopeTags</span></span>|<span data-ttu-id="6ba32-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ba32-146">Boolean</span></span>|<span data-ttu-id="6ba32-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="6ba32-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6ba32-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="6ba32-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6ba32-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="6ba32-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6ba32-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6ba32-150">This property is read-only.</span></span> <span data-ttu-id="6ba32-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ba32-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ba32-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6ba32-152">createdDateTime</span></span>|<span data-ttu-id="6ba32-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6ba32-153">DateTimeOffset</span></span>|<span data-ttu-id="6ba32-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="6ba32-154">DateTime the object was created.</span></span> <span data-ttu-id="6ba32-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ba32-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ba32-156">description</span><span class="sxs-lookup"><span data-stu-id="6ba32-156">description</span></span>|<span data-ttu-id="6ba32-157">String</span><span class="sxs-lookup"><span data-stu-id="6ba32-157">String</span></span>|<span data-ttu-id="6ba32-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6ba32-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6ba32-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ba32-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ba32-160">displayName</span><span class="sxs-lookup"><span data-stu-id="6ba32-160">displayName</span></span>|<span data-ttu-id="6ba32-161">String</span><span class="sxs-lookup"><span data-stu-id="6ba32-161">String</span></span>|<span data-ttu-id="6ba32-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6ba32-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6ba32-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ba32-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ba32-164">version</span><span class="sxs-lookup"><span data-stu-id="6ba32-164">version</span></span>|<span data-ttu-id="6ba32-165">Int32</span><span class="sxs-lookup"><span data-stu-id="6ba32-165">Int32</span></span>|<span data-ttu-id="6ba32-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6ba32-166">Version of the device configuration.</span></span> <span data-ttu-id="6ba32-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ba32-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ba32-168">payloadName</span><span class="sxs-lookup"><span data-stu-id="6ba32-168">payloadName</span></span>|<span data-ttu-id="6ba32-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6ba32-169">String</span></span>|<span data-ttu-id="6ba32-170">Nome que é exibido para o usuário.</span><span class="sxs-lookup"><span data-stu-id="6ba32-170">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="6ba32-171">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="6ba32-171">payloadFileName</span></span>|<span data-ttu-id="6ba32-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6ba32-172">String</span></span>|<span data-ttu-id="6ba32-173">O nome do arquivo de carga (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="6ba32-173">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="6ba32-174">\*.xml).</span><span class="sxs-lookup"><span data-stu-id="6ba32-174">\*.xml).</span></span>|
|<span data-ttu-id="6ba32-175">payload</span><span class="sxs-lookup"><span data-stu-id="6ba32-175">payload</span></span>|<span data-ttu-id="6ba32-176">Binária</span><span class="sxs-lookup"><span data-stu-id="6ba32-176">Binary</span></span>|<span data-ttu-id="6ba32-177">Carga.</span><span class="sxs-lookup"><span data-stu-id="6ba32-177">Payload.</span></span> <span data-ttu-id="6ba32-178">(Matriz de bytes codificados em UTF8)</span><span class="sxs-lookup"><span data-stu-id="6ba32-178">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="6ba32-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="6ba32-179">Response</span></span>
<span data-ttu-id="6ba32-180">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6ba32-180">If successful, this method returns a `200 OK` response code and an updated [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ba32-181">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6ba32-181">Example</span></span>

### <a name="request"></a><span data-ttu-id="6ba32-182">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6ba32-182">Request</span></span>
<span data-ttu-id="6ba32-183">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6ba32-183">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 371

{
  "@odata.type": "#microsoft.graph.iosCustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="6ba32-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="6ba32-184">Response</span></span>
<span data-ttu-id="6ba32-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6ba32-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 543

{
  "@odata.type": "#microsoft.graph.iosCustomConfiguration",
  "id": "f34428e3-28e3-f344-e328-44f3e32844f3",
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




