---
title: Atualizar windowsHealthMonitoringConfiguration
description: Atualiza as propriedades de um objeto windowsHealthMonitoringConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8e409ce95a90cf71fa7998a307f25f7a09db8f0d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32514922"
---
# <a name="update-windowshealthmonitoringconfiguration"></a><span data-ttu-id="57b17-103">Atualizar windowsHealthMonitoringConfiguration</span><span class="sxs-lookup"><span data-stu-id="57b17-103">Update windowsHealthMonitoringConfiguration</span></span>

> <span data-ttu-id="57b17-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="57b17-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="57b17-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="57b17-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57b17-106">Atualiza as propriedades de um objeto [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="57b17-106">Update the properties of a [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="57b17-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="57b17-107">Prerequisites</span></span>
<span data-ttu-id="57b17-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57b17-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57b17-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="57b17-110">Permission type</span></span>|<span data-ttu-id="57b17-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="57b17-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="57b17-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="57b17-112">Delegated (work or school account)</span></span>|<span data-ttu-id="57b17-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57b17-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="57b17-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="57b17-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="57b17-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="57b17-115">Not supported.</span></span>|
|<span data-ttu-id="57b17-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="57b17-116">Application</span></span>|<span data-ttu-id="57b17-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="57b17-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="57b17-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="57b17-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="57b17-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="57b17-119">Request headers</span></span>
|<span data-ttu-id="57b17-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="57b17-120">Header</span></span>|<span data-ttu-id="57b17-121">Valor</span><span class="sxs-lookup"><span data-stu-id="57b17-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="57b17-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="57b17-122">Authorization</span></span>|<span data-ttu-id="57b17-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="57b17-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="57b17-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="57b17-124">Accept</span></span>|<span data-ttu-id="57b17-125">application/json</span><span class="sxs-lookup"><span data-stu-id="57b17-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="57b17-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="57b17-126">Request body</span></span>
<span data-ttu-id="57b17-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="57b17-127">In the request body, supply a JSON representation for the [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) object.</span></span>

<span data-ttu-id="57b17-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="57b17-128">The following table shows the properties that are required when you create the [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md).</span></span>

|<span data-ttu-id="57b17-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="57b17-129">Property</span></span>|<span data-ttu-id="57b17-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="57b17-130">Type</span></span>|<span data-ttu-id="57b17-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="57b17-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57b17-132">id</span><span class="sxs-lookup"><span data-stu-id="57b17-132">id</span></span>|<span data-ttu-id="57b17-133">String</span><span class="sxs-lookup"><span data-stu-id="57b17-133">String</span></span>|<span data-ttu-id="57b17-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="57b17-134">Key of the entity.</span></span> <span data-ttu-id="57b17-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="57b17-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="57b17-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="57b17-136">lastModifiedDateTime</span></span>|<span data-ttu-id="57b17-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="57b17-137">DateTimeOffset</span></span>|<span data-ttu-id="57b17-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="57b17-138">DateTime the object was last modified.</span></span> <span data-ttu-id="57b17-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="57b17-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="57b17-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="57b17-140">roleScopeTagIds</span></span>|<span data-ttu-id="57b17-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="57b17-141">String collection</span></span>|<span data-ttu-id="57b17-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="57b17-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="57b17-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="57b17-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="57b17-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="57b17-144">supportsScopeTags</span></span>|<span data-ttu-id="57b17-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="57b17-145">Boolean</span></span>|<span data-ttu-id="57b17-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="57b17-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="57b17-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="57b17-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="57b17-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="57b17-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="57b17-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="57b17-149">This property is read-only.</span></span> <span data-ttu-id="57b17-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="57b17-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="57b17-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="57b17-151">createdDateTime</span></span>|<span data-ttu-id="57b17-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="57b17-152">DateTimeOffset</span></span>|<span data-ttu-id="57b17-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="57b17-153">DateTime the object was created.</span></span> <span data-ttu-id="57b17-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="57b17-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="57b17-155">description</span><span class="sxs-lookup"><span data-stu-id="57b17-155">description</span></span>|<span data-ttu-id="57b17-156">String</span><span class="sxs-lookup"><span data-stu-id="57b17-156">String</span></span>|<span data-ttu-id="57b17-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="57b17-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="57b17-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="57b17-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="57b17-159">displayName</span><span class="sxs-lookup"><span data-stu-id="57b17-159">displayName</span></span>|<span data-ttu-id="57b17-160">String</span><span class="sxs-lookup"><span data-stu-id="57b17-160">String</span></span>|<span data-ttu-id="57b17-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="57b17-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="57b17-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="57b17-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="57b17-163">versão</span><span class="sxs-lookup"><span data-stu-id="57b17-163">version</span></span>|<span data-ttu-id="57b17-164">Int32</span><span class="sxs-lookup"><span data-stu-id="57b17-164">Int32</span></span>|<span data-ttu-id="57b17-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="57b17-165">Version of the device configuration.</span></span> <span data-ttu-id="57b17-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="57b17-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="57b17-167">allowDeviceHealthMonitoring</span><span class="sxs-lookup"><span data-stu-id="57b17-167">allowDeviceHealthMonitoring</span></span>|[<span data-ttu-id="57b17-168">habilitação</span><span class="sxs-lookup"><span data-stu-id="57b17-168">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="57b17-169">Habilita o monitoramento de integridade do dispositivo no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="57b17-169">Enables device health monitoring on the device.</span></span> <span data-ttu-id="57b17-170">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="57b17-170">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="57b17-171">configDeviceHealthMonitoringScope</span><span class="sxs-lookup"><span data-stu-id="57b17-171">configDeviceHealthMonitoringScope</span></span>|[<span data-ttu-id="57b17-172">windowsHealthMonitoringScope</span><span class="sxs-lookup"><span data-stu-id="57b17-172">windowsHealthMonitoringScope</span></span>](../resources/intune-deviceconfig-windowshealthmonitoringscope.md)|<span data-ttu-id="57b17-173">Especifica conjunto de eventos coletados do dispositivo onde o monitoramento de integridade está habilitado.</span><span class="sxs-lookup"><span data-stu-id="57b17-173">Sepcifies set of events collected from the device where health monitoring is enabled.</span></span> <span data-ttu-id="57b17-174">Os valores possíveis são: `undefined`, `healthMonitoring`, `bootPerformance`.</span><span class="sxs-lookup"><span data-stu-id="57b17-174">Possible values are: `undefined`, `healthMonitoring`, `bootPerformance`.</span></span>|



## <a name="response"></a><span data-ttu-id="57b17-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="57b17-175">Response</span></span>
<span data-ttu-id="57b17-176">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="57b17-176">If successful, this method returns a `200 OK` response code and an updated [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57b17-177">Exemplo</span><span class="sxs-lookup"><span data-stu-id="57b17-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="57b17-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="57b17-178">Request</span></span>
<span data-ttu-id="57b17-179">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="57b17-179">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="57b17-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="57b17-180">Response</span></span>
<span data-ttu-id="57b17-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="57b17-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





