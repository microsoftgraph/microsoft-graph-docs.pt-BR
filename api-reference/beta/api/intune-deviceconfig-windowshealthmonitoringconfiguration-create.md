---
title: Criar windowsHealthMonitoringConfiguration
description: Criar um novo objeto windowsHealthMonitoringConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 75ace30116ddf2515f99f8bcdd6a2c9c19f45b58
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30972925"
---
# <a name="create-windowshealthmonitoringconfiguration"></a><span data-ttu-id="bf418-103">Criar windowsHealthMonitoringConfiguration</span><span class="sxs-lookup"><span data-stu-id="bf418-103">Create windowsHealthMonitoringConfiguration</span></span>

> <span data-ttu-id="bf418-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bf418-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bf418-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bf418-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bf418-106">Criar um novo objeto [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="bf418-106">Create a new [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bf418-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bf418-107">Prerequisites</span></span>
<span data-ttu-id="bf418-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf418-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf418-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bf418-110">Permission type</span></span>|<span data-ttu-id="bf418-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bf418-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bf418-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bf418-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bf418-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf418-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bf418-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bf418-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bf418-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bf418-115">Not supported.</span></span>|
|<span data-ttu-id="bf418-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bf418-116">Application</span></span>|<span data-ttu-id="bf418-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bf418-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bf418-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bf418-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="bf418-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bf418-119">Request headers</span></span>
|<span data-ttu-id="bf418-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bf418-120">Header</span></span>|<span data-ttu-id="bf418-121">Valor</span><span class="sxs-lookup"><span data-stu-id="bf418-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bf418-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="bf418-122">Authorization</span></span>|<span data-ttu-id="bf418-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bf418-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bf418-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bf418-124">Accept</span></span>|<span data-ttu-id="bf418-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bf418-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bf418-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bf418-126">Request body</span></span>
<span data-ttu-id="bf418-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsHealthMonitoringConfiguration.</span><span class="sxs-lookup"><span data-stu-id="bf418-127">In the request body, supply a JSON representation for the windowsHealthMonitoringConfiguration object.</span></span>

<span data-ttu-id="bf418-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsHealthMonitoringConfiguration.</span><span class="sxs-lookup"><span data-stu-id="bf418-128">The following table shows the properties that are required when you create the windowsHealthMonitoringConfiguration.</span></span>

|<span data-ttu-id="bf418-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bf418-129">Property</span></span>|<span data-ttu-id="bf418-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="bf418-130">Type</span></span>|<span data-ttu-id="bf418-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="bf418-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf418-132">id</span><span class="sxs-lookup"><span data-stu-id="bf418-132">id</span></span>|<span data-ttu-id="bf418-133">String</span><span class="sxs-lookup"><span data-stu-id="bf418-133">String</span></span>|<span data-ttu-id="bf418-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="bf418-134">Key of the entity.</span></span> <span data-ttu-id="bf418-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bf418-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bf418-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bf418-136">lastModifiedDateTime</span></span>|<span data-ttu-id="bf418-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bf418-137">DateTimeOffset</span></span>|<span data-ttu-id="bf418-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="bf418-138">DateTime the object was last modified.</span></span> <span data-ttu-id="bf418-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bf418-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bf418-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="bf418-140">roleScopeTagIds</span></span>|<span data-ttu-id="bf418-141">Coleção String</span><span class="sxs-lookup"><span data-stu-id="bf418-141">String collection</span></span>|<span data-ttu-id="bf418-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="bf418-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="bf418-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bf418-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bf418-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="bf418-144">supportsScopeTags</span></span>|<span data-ttu-id="bf418-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf418-145">Boolean</span></span>|<span data-ttu-id="bf418-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="bf418-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="bf418-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="bf418-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="bf418-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="bf418-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="bf418-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bf418-149">This property is read-only.</span></span> <span data-ttu-id="bf418-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bf418-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bf418-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bf418-151">createdDateTime</span></span>|<span data-ttu-id="bf418-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bf418-152">DateTimeOffset</span></span>|<span data-ttu-id="bf418-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="bf418-153">DateTime the object was created.</span></span> <span data-ttu-id="bf418-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bf418-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bf418-155">descrição</span><span class="sxs-lookup"><span data-stu-id="bf418-155">description</span></span>|<span data-ttu-id="bf418-156">String</span><span class="sxs-lookup"><span data-stu-id="bf418-156">String</span></span>|<span data-ttu-id="bf418-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bf418-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="bf418-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bf418-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bf418-159">displayName</span><span class="sxs-lookup"><span data-stu-id="bf418-159">displayName</span></span>|<span data-ttu-id="bf418-160">String</span><span class="sxs-lookup"><span data-stu-id="bf418-160">String</span></span>|<span data-ttu-id="bf418-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bf418-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="bf418-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bf418-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bf418-163">versão</span><span class="sxs-lookup"><span data-stu-id="bf418-163">version</span></span>|<span data-ttu-id="bf418-164">Int32</span><span class="sxs-lookup"><span data-stu-id="bf418-164">Int32</span></span>|<span data-ttu-id="bf418-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bf418-165">Version of the device configuration.</span></span> <span data-ttu-id="bf418-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bf418-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bf418-167">allowDeviceHealthMonitoring</span><span class="sxs-lookup"><span data-stu-id="bf418-167">allowDeviceHealthMonitoring</span></span>|[<span data-ttu-id="bf418-168">habilitação</span><span class="sxs-lookup"><span data-stu-id="bf418-168">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="bf418-169">Habilita o monitoramento de integridade do dispositivo no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bf418-169">Enables device health monitoring on the device.</span></span> <span data-ttu-id="bf418-170">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="bf418-170">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="bf418-171">configDeviceHealthMonitoringScope</span><span class="sxs-lookup"><span data-stu-id="bf418-171">configDeviceHealthMonitoringScope</span></span>|[<span data-ttu-id="bf418-172">windowsHealthMonitoringScope</span><span class="sxs-lookup"><span data-stu-id="bf418-172">windowsHealthMonitoringScope</span></span>](../resources/intune-deviceconfig-windowshealthmonitoringscope.md)|<span data-ttu-id="bf418-173">Especifica conjunto de eventos coletados do dispositivo onde o monitoramento de integridade está habilitado.</span><span class="sxs-lookup"><span data-stu-id="bf418-173">Sepcifies set of events collected from the device where health monitoring is enabled.</span></span> <span data-ttu-id="bf418-174">Os valores possíveis são: `undefined`, `healthMonitoring`, `bootPerformance`.</span><span class="sxs-lookup"><span data-stu-id="bf418-174">Possible values are: `undefined`, `healthMonitoring`, `bootPerformance`.</span></span>|



## <a name="response"></a><span data-ttu-id="bf418-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="bf418-175">Response</span></span>
<span data-ttu-id="bf418-176">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bf418-176">If successful, this method returns a `201 Created` response code and a [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bf418-177">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bf418-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="bf418-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bf418-178">Request</span></span>
<span data-ttu-id="bf418-179">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bf418-179">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 371

{
  "@odata.type": "#microsoft.graph.windowsHealthMonitoringConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "allowDeviceHealthMonitoring": "enabled",
  "configDeviceHealthMonitoringScope": "healthMonitoring"
}
```

### <a name="response"></a><span data-ttu-id="bf418-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="bf418-180">Response</span></span>
<span data-ttu-id="bf418-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bf418-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 543

{
  "@odata.type": "#microsoft.graph.windowsHealthMonitoringConfiguration",
  "id": "3439bcec-bcec-3439-ecbc-3934ecbc3934",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "allowDeviceHealthMonitoring": "enabled",
  "configDeviceHealthMonitoringScope": "healthMonitoring"
}
```




