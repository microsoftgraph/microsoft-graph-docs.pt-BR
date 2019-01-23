---
title: Atualizar windows10CustomConfiguration
description: Atualizar as propriedades de um objeto windows10CustomConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bb0cf97455c40811be97e29cd420bc355ca493f2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29392973"
---
# <a name="update-windows10customconfiguration"></a><span data-ttu-id="521f4-103">Atualizar windows10CustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="521f4-103">Update windows10CustomConfiguration</span></span>

> <span data-ttu-id="521f4-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="521f4-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="521f4-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="521f4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="521f4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="521f4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="521f4-107">Atualizar as propriedades de um objeto [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="521f4-107">Update the properties of a [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="521f4-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="521f4-108">Prerequisites</span></span>
<span data-ttu-id="521f4-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="521f4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="521f4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="521f4-111">Permission type</span></span>|<span data-ttu-id="521f4-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="521f4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="521f4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="521f4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="521f4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="521f4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="521f4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="521f4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="521f4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="521f4-116">Not supported.</span></span>|
|<span data-ttu-id="521f4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="521f4-117">Application</span></span>|<span data-ttu-id="521f4-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="521f4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="521f4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="521f4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="521f4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="521f4-120">Request headers</span></span>
|<span data-ttu-id="521f4-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="521f4-121">Header</span></span>|<span data-ttu-id="521f4-122">Valor</span><span class="sxs-lookup"><span data-stu-id="521f4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="521f4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="521f4-123">Authorization</span></span>|<span data-ttu-id="521f4-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="521f4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="521f4-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="521f4-125">Accept</span></span>|<span data-ttu-id="521f4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="521f4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="521f4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="521f4-127">Request body</span></span>
<span data-ttu-id="521f4-128">No corpo da solicitação, forneça uma representação JSON do objeto [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="521f4-128">In the request body, supply a JSON representation for the [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) object.</span></span>

<span data-ttu-id="521f4-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="521f4-129">The following table shows the properties that are required when you create the [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md).</span></span>

|<span data-ttu-id="521f4-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="521f4-130">Property</span></span>|<span data-ttu-id="521f4-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="521f4-131">Type</span></span>|<span data-ttu-id="521f4-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="521f4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="521f4-133">id</span><span class="sxs-lookup"><span data-stu-id="521f4-133">id</span></span>|<span data-ttu-id="521f4-134">String</span><span class="sxs-lookup"><span data-stu-id="521f4-134">String</span></span>|<span data-ttu-id="521f4-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="521f4-135">Key of the entity.</span></span> <span data-ttu-id="521f4-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="521f4-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="521f4-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="521f4-137">lastModifiedDateTime</span></span>|<span data-ttu-id="521f4-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="521f4-138">DateTimeOffset</span></span>|<span data-ttu-id="521f4-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="521f4-139">DateTime the object was last modified.</span></span> <span data-ttu-id="521f4-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="521f4-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="521f4-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="521f4-141">roleScopeTagIds</span></span>|<span data-ttu-id="521f4-142">String collection</span><span class="sxs-lookup"><span data-stu-id="521f4-142">String collection</span></span>|<span data-ttu-id="521f4-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="521f4-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="521f4-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="521f4-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="521f4-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="521f4-145">supportsScopeTags</span></span>|<span data-ttu-id="521f4-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="521f4-146">Boolean</span></span>|<span data-ttu-id="521f4-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="521f4-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="521f4-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="521f4-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="521f4-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="521f4-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="521f4-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="521f4-150">This property is read-only.</span></span> <span data-ttu-id="521f4-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="521f4-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="521f4-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="521f4-152">createdDateTime</span></span>|<span data-ttu-id="521f4-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="521f4-153">DateTimeOffset</span></span>|<span data-ttu-id="521f4-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="521f4-154">DateTime the object was created.</span></span> <span data-ttu-id="521f4-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="521f4-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="521f4-156">description</span><span class="sxs-lookup"><span data-stu-id="521f4-156">description</span></span>|<span data-ttu-id="521f4-157">String</span><span class="sxs-lookup"><span data-stu-id="521f4-157">String</span></span>|<span data-ttu-id="521f4-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="521f4-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="521f4-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="521f4-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="521f4-160">displayName</span><span class="sxs-lookup"><span data-stu-id="521f4-160">displayName</span></span>|<span data-ttu-id="521f4-161">String</span><span class="sxs-lookup"><span data-stu-id="521f4-161">String</span></span>|<span data-ttu-id="521f4-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="521f4-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="521f4-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="521f4-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="521f4-164">version</span><span class="sxs-lookup"><span data-stu-id="521f4-164">version</span></span>|<span data-ttu-id="521f4-165">Int32</span><span class="sxs-lookup"><span data-stu-id="521f4-165">Int32</span></span>|<span data-ttu-id="521f4-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="521f4-166">Version of the device configuration.</span></span> <span data-ttu-id="521f4-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="521f4-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="521f4-168">omaSettings</span><span class="sxs-lookup"><span data-stu-id="521f4-168">omaSettings</span></span>|<span data-ttu-id="521f4-169">Coleção [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="521f4-169">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="521f4-170">Configurações OMA.</span><span class="sxs-lookup"><span data-stu-id="521f4-170">OMA settings.</span></span> <span data-ttu-id="521f4-171">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="521f4-171">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="521f4-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="521f4-172">Response</span></span>
<span data-ttu-id="521f4-173">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="521f4-173">If successful, this method returns a `200 OK` response code and an updated [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="521f4-174">Exemplo</span><span class="sxs-lookup"><span data-stu-id="521f4-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="521f4-175">Solicitação</span><span class="sxs-lookup"><span data-stu-id="521f4-175">Request</span></span>
<span data-ttu-id="521f4-176">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="521f4-176">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 496

{
  "@odata.type": "#microsoft.graph.windows10CustomConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSettingInteger",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "value": 5
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="521f4-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="521f4-177">Response</span></span>
<span data-ttu-id="521f4-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="521f4-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 668

{
  "@odata.type": "#microsoft.graph.windows10CustomConfiguration",
  "id": "d8ae266e-266e-d8ae-6e26-aed86e26aed8",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSettingInteger",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "value": 5
    }
  ]
}
```




