---
title: Criar androidCustomConfiguration
description: Criar um novo objeto androidCustomConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: dc000c2fa4e0f47bbc8b37dd1b69886be3142e5a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409710"
---
# <a name="create-androidcustomconfiguration"></a><span data-ttu-id="efd95-103">Criar androidCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="efd95-103">Create androidCustomConfiguration</span></span>

> <span data-ttu-id="efd95-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="efd95-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="efd95-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="efd95-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="efd95-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="efd95-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="efd95-107">Criar um novo objeto [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="efd95-107">Create a new [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="efd95-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="efd95-108">Prerequisites</span></span>
<span data-ttu-id="efd95-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="efd95-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="efd95-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="efd95-111">Permission type</span></span>|<span data-ttu-id="efd95-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="efd95-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="efd95-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="efd95-113">Delegated (work or school account)</span></span>|<span data-ttu-id="efd95-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efd95-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="efd95-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="efd95-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="efd95-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="efd95-116">Not supported.</span></span>|
|<span data-ttu-id="efd95-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="efd95-117">Application</span></span>|<span data-ttu-id="efd95-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="efd95-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="efd95-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="efd95-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="efd95-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="efd95-120">Request headers</span></span>
|<span data-ttu-id="efd95-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="efd95-121">Header</span></span>|<span data-ttu-id="efd95-122">Valor</span><span class="sxs-lookup"><span data-stu-id="efd95-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="efd95-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="efd95-123">Authorization</span></span>|<span data-ttu-id="efd95-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="efd95-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="efd95-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="efd95-125">Accept</span></span>|<span data-ttu-id="efd95-126">application/json</span><span class="sxs-lookup"><span data-stu-id="efd95-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="efd95-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="efd95-127">Request body</span></span>
<span data-ttu-id="efd95-128">No corpo da solicitação, forneça uma representação JSON do objeto androidCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="efd95-128">In the request body, supply a JSON representation for the androidCustomConfiguration object.</span></span>

<span data-ttu-id="efd95-129">A tabela a seguir mostra as propriedades que são necessárias ao criar androidCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="efd95-129">The following table shows the properties that are required when you create the androidCustomConfiguration.</span></span>

|<span data-ttu-id="efd95-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="efd95-130">Property</span></span>|<span data-ttu-id="efd95-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="efd95-131">Type</span></span>|<span data-ttu-id="efd95-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="efd95-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="efd95-133">id</span><span class="sxs-lookup"><span data-stu-id="efd95-133">id</span></span>|<span data-ttu-id="efd95-134">String</span><span class="sxs-lookup"><span data-stu-id="efd95-134">String</span></span>|<span data-ttu-id="efd95-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="efd95-135">Key of the entity.</span></span> <span data-ttu-id="efd95-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="efd95-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="efd95-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="efd95-137">lastModifiedDateTime</span></span>|<span data-ttu-id="efd95-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="efd95-138">DateTimeOffset</span></span>|<span data-ttu-id="efd95-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="efd95-139">DateTime the object was last modified.</span></span> <span data-ttu-id="efd95-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="efd95-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="efd95-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="efd95-141">roleScopeTagIds</span></span>|<span data-ttu-id="efd95-142">String collection</span><span class="sxs-lookup"><span data-stu-id="efd95-142">String collection</span></span>|<span data-ttu-id="efd95-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="efd95-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="efd95-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="efd95-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="efd95-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="efd95-145">supportsScopeTags</span></span>|<span data-ttu-id="efd95-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="efd95-146">Boolean</span></span>|<span data-ttu-id="efd95-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="efd95-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="efd95-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="efd95-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="efd95-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="efd95-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="efd95-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efd95-150">This property is read-only.</span></span> <span data-ttu-id="efd95-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="efd95-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="efd95-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="efd95-152">createdDateTime</span></span>|<span data-ttu-id="efd95-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="efd95-153">DateTimeOffset</span></span>|<span data-ttu-id="efd95-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="efd95-154">DateTime the object was created.</span></span> <span data-ttu-id="efd95-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="efd95-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="efd95-156">description</span><span class="sxs-lookup"><span data-stu-id="efd95-156">description</span></span>|<span data-ttu-id="efd95-157">String</span><span class="sxs-lookup"><span data-stu-id="efd95-157">String</span></span>|<span data-ttu-id="efd95-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="efd95-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="efd95-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="efd95-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="efd95-160">displayName</span><span class="sxs-lookup"><span data-stu-id="efd95-160">displayName</span></span>|<span data-ttu-id="efd95-161">String</span><span class="sxs-lookup"><span data-stu-id="efd95-161">String</span></span>|<span data-ttu-id="efd95-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="efd95-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="efd95-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="efd95-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="efd95-164">version</span><span class="sxs-lookup"><span data-stu-id="efd95-164">version</span></span>|<span data-ttu-id="efd95-165">Int32</span><span class="sxs-lookup"><span data-stu-id="efd95-165">Int32</span></span>|<span data-ttu-id="efd95-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="efd95-166">Version of the device configuration.</span></span> <span data-ttu-id="efd95-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="efd95-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="efd95-168">omaSettings</span><span class="sxs-lookup"><span data-stu-id="efd95-168">omaSettings</span></span>|<span data-ttu-id="efd95-169">Coleção [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="efd95-169">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="efd95-170">Configurações OMA.</span><span class="sxs-lookup"><span data-stu-id="efd95-170">OMA settings.</span></span> <span data-ttu-id="efd95-171">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="efd95-171">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="efd95-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="efd95-172">Response</span></span>
<span data-ttu-id="efd95-173">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="efd95-173">If successful, this method returns a `201 Created` response code and a [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="efd95-174">Exemplo</span><span class="sxs-lookup"><span data-stu-id="efd95-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="efd95-175">Solicitação</span><span class="sxs-lookup"><span data-stu-id="efd95-175">Request</span></span>
<span data-ttu-id="efd95-176">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="efd95-176">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 494

{
  "@odata.type": "#microsoft.graph.androidCustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="efd95-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="efd95-177">Response</span></span>
<span data-ttu-id="efd95-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="efd95-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 666

{
  "@odata.type": "#microsoft.graph.androidCustomConfiguration",
  "id": "619b5e6d-5e6d-619b-6d5e-9b616d5e9b61",
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




