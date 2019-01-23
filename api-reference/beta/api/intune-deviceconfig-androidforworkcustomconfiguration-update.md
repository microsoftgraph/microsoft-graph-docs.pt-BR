---
title: Atualizar androidForWorkCustomConfiguration
description: Atualize as propriedades de um objeto androidForWorkCustomConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f5226e1113f28f09f2e1ebb6a2fb0e660d1fa4cf
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414260"
---
# <a name="update-androidforworkcustomconfiguration"></a><span data-ttu-id="a7355-103">Atualizar androidForWorkCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="a7355-103">Update androidForWorkCustomConfiguration</span></span>

> <span data-ttu-id="a7355-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="a7355-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a7355-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a7355-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a7355-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="a7355-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7355-107">Atualize as propriedades de um objeto [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="a7355-107">Update the properties of a [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a7355-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a7355-108">Prerequisites</span></span>
<span data-ttu-id="a7355-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a7355-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a7355-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a7355-111">Permission type</span></span>|<span data-ttu-id="a7355-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a7355-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a7355-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a7355-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a7355-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7355-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a7355-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a7355-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a7355-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a7355-116">Not supported.</span></span>|
|<span data-ttu-id="a7355-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a7355-117">Application</span></span>|<span data-ttu-id="a7355-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a7355-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a7355-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a7355-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a7355-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a7355-120">Request headers</span></span>
|<span data-ttu-id="a7355-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a7355-121">Header</span></span>|<span data-ttu-id="a7355-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a7355-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a7355-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a7355-123">Authorization</span></span>|<span data-ttu-id="a7355-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a7355-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a7355-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a7355-125">Accept</span></span>|<span data-ttu-id="a7355-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a7355-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a7355-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a7355-127">Request body</span></span>
<span data-ttu-id="a7355-128">No corpo da solicitação, fornece uma representação JSON para o objeto [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="a7355-128">In the request body, supply a JSON representation for the [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) object.</span></span>

<span data-ttu-id="a7355-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a7355-129">The following table shows the properties that are required when you create the [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md).</span></span>

|<span data-ttu-id="a7355-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a7355-130">Property</span></span>|<span data-ttu-id="a7355-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a7355-131">Type</span></span>|<span data-ttu-id="a7355-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a7355-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7355-133">id</span><span class="sxs-lookup"><span data-stu-id="a7355-133">id</span></span>|<span data-ttu-id="a7355-134">String</span><span class="sxs-lookup"><span data-stu-id="a7355-134">String</span></span>|<span data-ttu-id="a7355-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a7355-135">Key of the entity.</span></span> <span data-ttu-id="a7355-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7355-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7355-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a7355-137">lastModifiedDateTime</span></span>|<span data-ttu-id="a7355-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7355-138">DateTimeOffset</span></span>|<span data-ttu-id="a7355-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="a7355-139">DateTime the object was last modified.</span></span> <span data-ttu-id="a7355-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7355-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7355-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a7355-141">roleScopeTagIds</span></span>|<span data-ttu-id="a7355-142">String collection</span><span class="sxs-lookup"><span data-stu-id="a7355-142">String collection</span></span>|<span data-ttu-id="a7355-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="a7355-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a7355-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7355-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7355-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a7355-145">supportsScopeTags</span></span>|<span data-ttu-id="a7355-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7355-146">Boolean</span></span>|<span data-ttu-id="a7355-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="a7355-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a7355-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="a7355-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a7355-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="a7355-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a7355-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a7355-150">This property is read-only.</span></span> <span data-ttu-id="a7355-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7355-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7355-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a7355-152">createdDateTime</span></span>|<span data-ttu-id="a7355-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7355-153">DateTimeOffset</span></span>|<span data-ttu-id="a7355-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="a7355-154">DateTime the object was created.</span></span> <span data-ttu-id="a7355-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7355-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7355-156">description</span><span class="sxs-lookup"><span data-stu-id="a7355-156">description</span></span>|<span data-ttu-id="a7355-157">String</span><span class="sxs-lookup"><span data-stu-id="a7355-157">String</span></span>|<span data-ttu-id="a7355-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a7355-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a7355-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7355-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7355-160">displayName</span><span class="sxs-lookup"><span data-stu-id="a7355-160">displayName</span></span>|<span data-ttu-id="a7355-161">String</span><span class="sxs-lookup"><span data-stu-id="a7355-161">String</span></span>|<span data-ttu-id="a7355-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a7355-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a7355-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7355-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7355-164">version</span><span class="sxs-lookup"><span data-stu-id="a7355-164">version</span></span>|<span data-ttu-id="a7355-165">Int32</span><span class="sxs-lookup"><span data-stu-id="a7355-165">Int32</span></span>|<span data-ttu-id="a7355-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a7355-166">Version of the device configuration.</span></span> <span data-ttu-id="a7355-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7355-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7355-168">omaSettings</span><span class="sxs-lookup"><span data-stu-id="a7355-168">omaSettings</span></span>|<span data-ttu-id="a7355-169">Coleção [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="a7355-169">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="a7355-170">Configurações OMA.</span><span class="sxs-lookup"><span data-stu-id="a7355-170">OMA settings.</span></span> <span data-ttu-id="a7355-171">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="a7355-171">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="a7355-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="a7355-172">Response</span></span>
<span data-ttu-id="a7355-173">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a7355-173">If successful, this method returns a `200 OK` response code and an updated [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7355-174">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a7355-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="a7355-175">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a7355-175">Request</span></span>
<span data-ttu-id="a7355-176">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a7355-176">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 501

{
  "@odata.type": "#microsoft.graph.androidForWorkCustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="a7355-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="a7355-177">Response</span></span>
<span data-ttu-id="a7355-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a7355-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 673

{
  "@odata.type": "#microsoft.graph.androidForWorkCustomConfiguration",
  "id": "cca8b2bb-b2bb-cca8-bbb2-a8ccbbb2a8cc",
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




