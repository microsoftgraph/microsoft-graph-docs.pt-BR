---
title: Criar macOSCustomConfiguration
description: Cria um novo objeto macOSCustomConfiguration.
author: tfitzmac
ms.openlocfilehash: 0169ba83335be2202ca3034df7205a407021d0c0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340247"
---
# <a name="create-macoscustomconfiguration"></a><span data-ttu-id="18ad6-103">Criar macOSCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="18ad6-103">Create macOSCustomConfiguration</span></span>

> <span data-ttu-id="18ad6-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="18ad6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="18ad6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="18ad6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="18ad6-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="18ad6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="18ad6-107">Cria um novo objeto [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="18ad6-107">Create a new [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="18ad6-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="18ad6-108">Prerequisites</span></span>
<span data-ttu-id="18ad6-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18ad6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18ad6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="18ad6-111">Permission type</span></span>|<span data-ttu-id="18ad6-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="18ad6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="18ad6-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="18ad6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="18ad6-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18ad6-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="18ad6-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="18ad6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18ad6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="18ad6-116">Not supported.</span></span>|
|<span data-ttu-id="18ad6-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="18ad6-117">Application</span></span>|<span data-ttu-id="18ad6-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="18ad6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="18ad6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="18ad6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="18ad6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="18ad6-120">Request headers</span></span>
|<span data-ttu-id="18ad6-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="18ad6-121">Header</span></span>|<span data-ttu-id="18ad6-122">Valor</span><span class="sxs-lookup"><span data-stu-id="18ad6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="18ad6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="18ad6-123">Authorization</span></span>|<span data-ttu-id="18ad6-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="18ad6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="18ad6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="18ad6-125">Accept</span></span>|<span data-ttu-id="18ad6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="18ad6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="18ad6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="18ad6-127">Request body</span></span>
<span data-ttu-id="18ad6-128">No corpo da solicitação, forneça uma representação JSON do objeto macOSCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="18ad6-128">In the request body, supply a JSON representation for the macOSCustomConfiguration object.</span></span>

<span data-ttu-id="18ad6-129">A tabela a seguir mostra as propriedades que são necessárias ao criar macOSCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="18ad6-129">The following table shows the properties that are required when you create the macOSCustomConfiguration.</span></span>

|<span data-ttu-id="18ad6-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="18ad6-130">Property</span></span>|<span data-ttu-id="18ad6-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="18ad6-131">Type</span></span>|<span data-ttu-id="18ad6-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="18ad6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18ad6-133">id</span><span class="sxs-lookup"><span data-stu-id="18ad6-133">id</span></span>|<span data-ttu-id="18ad6-134">String</span><span class="sxs-lookup"><span data-stu-id="18ad6-134">String</span></span>|<span data-ttu-id="18ad6-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="18ad6-135">Key of the entity.</span></span> <span data-ttu-id="18ad6-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18ad6-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18ad6-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="18ad6-137">lastModifiedDateTime</span></span>|<span data-ttu-id="18ad6-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18ad6-138">DateTimeOffset</span></span>|<span data-ttu-id="18ad6-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="18ad6-139">DateTime the object was last modified.</span></span> <span data-ttu-id="18ad6-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18ad6-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18ad6-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="18ad6-141">roleScopeTagIds</span></span>|<span data-ttu-id="18ad6-142">String collection</span><span class="sxs-lookup"><span data-stu-id="18ad6-142">String collection</span></span>|<span data-ttu-id="18ad6-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="18ad6-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="18ad6-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18ad6-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18ad6-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="18ad6-145">supportsScopeTags</span></span>|<span data-ttu-id="18ad6-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="18ad6-146">Boolean</span></span>|<span data-ttu-id="18ad6-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="18ad6-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="18ad6-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="18ad6-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="18ad6-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="18ad6-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="18ad6-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="18ad6-150">This property is read-only.</span></span> <span data-ttu-id="18ad6-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18ad6-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18ad6-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="18ad6-152">createdDateTime</span></span>|<span data-ttu-id="18ad6-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18ad6-153">DateTimeOffset</span></span>|<span data-ttu-id="18ad6-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="18ad6-154">DateTime the object was created.</span></span> <span data-ttu-id="18ad6-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18ad6-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18ad6-156">description</span><span class="sxs-lookup"><span data-stu-id="18ad6-156">description</span></span>|<span data-ttu-id="18ad6-157">String</span><span class="sxs-lookup"><span data-stu-id="18ad6-157">String</span></span>|<span data-ttu-id="18ad6-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="18ad6-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="18ad6-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18ad6-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18ad6-160">displayName</span><span class="sxs-lookup"><span data-stu-id="18ad6-160">displayName</span></span>|<span data-ttu-id="18ad6-161">String</span><span class="sxs-lookup"><span data-stu-id="18ad6-161">String</span></span>|<span data-ttu-id="18ad6-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="18ad6-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="18ad6-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18ad6-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18ad6-164">version</span><span class="sxs-lookup"><span data-stu-id="18ad6-164">version</span></span>|<span data-ttu-id="18ad6-165">Int32</span><span class="sxs-lookup"><span data-stu-id="18ad6-165">Int32</span></span>|<span data-ttu-id="18ad6-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="18ad6-166">Version of the device configuration.</span></span> <span data-ttu-id="18ad6-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18ad6-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18ad6-168">payloadName</span><span class="sxs-lookup"><span data-stu-id="18ad6-168">payloadName</span></span>|<span data-ttu-id="18ad6-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="18ad6-169">String</span></span>|<span data-ttu-id="18ad6-170">Nome que é exibido para o usuário.</span><span class="sxs-lookup"><span data-stu-id="18ad6-170">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="18ad6-171">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="18ad6-171">payloadFileName</span></span>|<span data-ttu-id="18ad6-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="18ad6-172">String</span></span>|<span data-ttu-id="18ad6-173">O nome do arquivo de carga (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="18ad6-173">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="18ad6-174">\*.xml).</span><span class="sxs-lookup"><span data-stu-id="18ad6-174">\*.xml).</span></span>|
|<span data-ttu-id="18ad6-175">payload</span><span class="sxs-lookup"><span data-stu-id="18ad6-175">payload</span></span>|<span data-ttu-id="18ad6-176">Binária</span><span class="sxs-lookup"><span data-stu-id="18ad6-176">Binary</span></span>|<span data-ttu-id="18ad6-177">Carga.</span><span class="sxs-lookup"><span data-stu-id="18ad6-177">Payload.</span></span> <span data-ttu-id="18ad6-178">(Matriz de bytes codificados em UTF8)</span><span class="sxs-lookup"><span data-stu-id="18ad6-178">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="18ad6-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="18ad6-179">Response</span></span>
<span data-ttu-id="18ad6-180">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="18ad6-180">If successful, this method returns a `201 Created` response code and a [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18ad6-181">Exemplo</span><span class="sxs-lookup"><span data-stu-id="18ad6-181">Example</span></span>
### <a name="request"></a><span data-ttu-id="18ad6-182">Solicitação</span><span class="sxs-lookup"><span data-stu-id="18ad6-182">Request</span></span>
<span data-ttu-id="18ad6-183">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="18ad6-183">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 437

{
  "@odata.type": "#microsoft.graph.macOSCustomConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="18ad6-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="18ad6-184">Response</span></span>
<span data-ttu-id="18ad6-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="18ad6-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





