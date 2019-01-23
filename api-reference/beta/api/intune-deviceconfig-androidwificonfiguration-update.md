---
title: Atualizar androidWiFiConfiguration
description: Atualize as propriedades de um objeto androidWiFiConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 33abae4905e2d8a83254dedb679143e242e3ed67
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424844"
---
# <a name="update-androidwificonfiguration"></a><span data-ttu-id="e4ee8-103">Atualizar androidWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="e4ee8-103">Update androidWiFiConfiguration</span></span>

> <span data-ttu-id="e4ee8-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="e4ee8-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e4ee8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e4ee8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e4ee8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="e4ee8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4ee8-107">Atualize as propriedades de um objeto [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="e4ee8-107">Update the properties of a [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e4ee8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e4ee8-108">Prerequisites</span></span>
<span data-ttu-id="e4ee8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e4ee8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e4ee8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e4ee8-111">Permission type</span></span>|<span data-ttu-id="e4ee8-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e4ee8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e4ee8-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e4ee8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e4ee8-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4ee8-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e4ee8-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e4ee8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4ee8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e4ee8-116">Not supported.</span></span>|
|<span data-ttu-id="e4ee8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e4ee8-117">Application</span></span>|<span data-ttu-id="e4ee8-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e4ee8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e4ee8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e4ee8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="e4ee8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e4ee8-120">Request headers</span></span>
|<span data-ttu-id="e4ee8-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e4ee8-121">Header</span></span>|<span data-ttu-id="e4ee8-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e4ee8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e4ee8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e4ee8-123">Authorization</span></span>|<span data-ttu-id="e4ee8-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e4ee8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e4ee8-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e4ee8-125">Accept</span></span>|<span data-ttu-id="e4ee8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e4ee8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4ee8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e4ee8-127">Request body</span></span>
<span data-ttu-id="e4ee8-128">No corpo da solicitação, fornece uma representação JSON para o objeto [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="e4ee8-128">In the request body, supply a JSON representation for the [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) object.</span></span>

<span data-ttu-id="e4ee8-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e4ee8-129">The following table shows the properties that are required when you create the [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md).</span></span>

|<span data-ttu-id="e4ee8-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e4ee8-130">Property</span></span>|<span data-ttu-id="e4ee8-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e4ee8-131">Type</span></span>|<span data-ttu-id="e4ee8-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4ee8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4ee8-133">id</span><span class="sxs-lookup"><span data-stu-id="e4ee8-133">id</span></span>|<span data-ttu-id="e4ee8-134">String</span><span class="sxs-lookup"><span data-stu-id="e4ee8-134">String</span></span>|<span data-ttu-id="e4ee8-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e4ee8-135">Key of the entity.</span></span> <span data-ttu-id="e4ee8-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e4ee8-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e4ee8-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e4ee8-137">lastModifiedDateTime</span></span>|<span data-ttu-id="e4ee8-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4ee8-138">DateTimeOffset</span></span>|<span data-ttu-id="e4ee8-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="e4ee8-139">DateTime the object was last modified.</span></span> <span data-ttu-id="e4ee8-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e4ee8-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e4ee8-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e4ee8-141">roleScopeTagIds</span></span>|<span data-ttu-id="e4ee8-142">String collection</span><span class="sxs-lookup"><span data-stu-id="e4ee8-142">String collection</span></span>|<span data-ttu-id="e4ee8-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="e4ee8-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e4ee8-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e4ee8-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e4ee8-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="e4ee8-145">supportsScopeTags</span></span>|<span data-ttu-id="e4ee8-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4ee8-146">Boolean</span></span>|<span data-ttu-id="e4ee8-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="e4ee8-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e4ee8-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="e4ee8-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e4ee8-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="e4ee8-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e4ee8-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e4ee8-150">This property is read-only.</span></span> <span data-ttu-id="e4ee8-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e4ee8-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e4ee8-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e4ee8-152">createdDateTime</span></span>|<span data-ttu-id="e4ee8-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4ee8-153">DateTimeOffset</span></span>|<span data-ttu-id="e4ee8-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="e4ee8-154">DateTime the object was created.</span></span> <span data-ttu-id="e4ee8-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e4ee8-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e4ee8-156">description</span><span class="sxs-lookup"><span data-stu-id="e4ee8-156">description</span></span>|<span data-ttu-id="e4ee8-157">String</span><span class="sxs-lookup"><span data-stu-id="e4ee8-157">String</span></span>|<span data-ttu-id="e4ee8-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e4ee8-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e4ee8-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e4ee8-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e4ee8-160">displayName</span><span class="sxs-lookup"><span data-stu-id="e4ee8-160">displayName</span></span>|<span data-ttu-id="e4ee8-161">String</span><span class="sxs-lookup"><span data-stu-id="e4ee8-161">String</span></span>|<span data-ttu-id="e4ee8-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e4ee8-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e4ee8-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e4ee8-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e4ee8-164">version</span><span class="sxs-lookup"><span data-stu-id="e4ee8-164">version</span></span>|<span data-ttu-id="e4ee8-165">Int32</span><span class="sxs-lookup"><span data-stu-id="e4ee8-165">Int32</span></span>|<span data-ttu-id="e4ee8-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e4ee8-166">Version of the device configuration.</span></span> <span data-ttu-id="e4ee8-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e4ee8-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e4ee8-168">networkName</span><span class="sxs-lookup"><span data-stu-id="e4ee8-168">networkName</span></span>|<span data-ttu-id="e4ee8-169">String</span><span class="sxs-lookup"><span data-stu-id="e4ee8-169">String</span></span>|<span data-ttu-id="e4ee8-170">Nome da rede</span><span class="sxs-lookup"><span data-stu-id="e4ee8-170">Network Name</span></span>|
|<span data-ttu-id="e4ee8-171">SSID</span><span class="sxs-lookup"><span data-stu-id="e4ee8-171">ssid</span></span>|<span data-ttu-id="e4ee8-172">String</span><span class="sxs-lookup"><span data-stu-id="e4ee8-172">String</span></span>|<span data-ttu-id="e4ee8-173">Este é o nome da rede Wi-Fi que é difundido para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="e4ee8-173">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="e4ee8-174">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="e4ee8-174">connectAutomatically</span></span>|<span data-ttu-id="e4ee8-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4ee8-175">Boolean</span></span>|<span data-ttu-id="e4ee8-176">Conecte automaticamente quando esta rede estiver no intervalo.</span><span class="sxs-lookup"><span data-stu-id="e4ee8-176">Connect automatically when this network is in range.</span></span> <span data-ttu-id="e4ee8-177">Essa configuração como true ignorar o prompt do usuário e se conecte automaticamente o dispositivo à rede Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="e4ee8-177">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="e4ee8-178">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="e4ee8-178">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="e4ee8-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4ee8-179">Boolean</span></span>|<span data-ttu-id="e4ee8-180">Quando definido como true, esse perfil força o dispositivo para se conectar a uma rede que não transmite seu SSID para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="e4ee8-180">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="e4ee8-181">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="e4ee8-181">wiFiSecurityType</span></span>|[<span data-ttu-id="e4ee8-182">androidWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="e4ee8-182">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="e4ee8-183">Indica se o ponto de extremidade Wi-Fi usa um tipo de segurança baseada em EAP.</span><span class="sxs-lookup"><span data-stu-id="e4ee8-183">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="e4ee8-184">Os valores possíveis são: `open` e `wpaEnterprise`.</span><span class="sxs-lookup"><span data-stu-id="e4ee8-184">Possible values are: `open`, `wpaEnterprise`.</span></span>|



## <a name="response"></a><span data-ttu-id="e4ee8-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4ee8-185">Response</span></span>
<span data-ttu-id="e4ee8-186">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e4ee8-186">If successful, this method returns a `200 OK` response code and an updated [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4ee8-187">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e4ee8-187">Example</span></span>

### <a name="request"></a><span data-ttu-id="e4ee8-188">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e4ee8-188">Request</span></span>
<span data-ttu-id="e4ee8-189">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e4ee8-189">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 435

{
  "@odata.type": "#microsoft.graph.androidWiFiConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "networkName": "Network Name value",
  "ssid": "Ssid value",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "wpaEnterprise"
}
```

### <a name="response"></a><span data-ttu-id="e4ee8-190">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4ee8-190">Response</span></span>
<span data-ttu-id="e4ee8-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e4ee8-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 607

{
  "@odata.type": "#microsoft.graph.androidWiFiConfiguration",
  "id": "51cfd26f-d26f-51cf-6fd2-cf516fd2cf51",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "networkName": "Network Name value",
  "ssid": "Ssid value",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "wpaEnterprise"
}
```




