---
title: Atualizar androidWorkProfileWiFiConfiguration
description: Atualize as propriedades de um objeto androidWorkProfileWiFiConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 229ace77c5e921c77a988608d7c2dacce5fc1bf4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983048"
---
# <a name="update-androidworkprofilewificonfiguration"></a><span data-ttu-id="d8d00-103">Atualizar androidWorkProfileWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="d8d00-103">Update androidWorkProfileWiFiConfiguration</span></span>

> <span data-ttu-id="d8d00-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d8d00-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d8d00-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d8d00-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d8d00-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d8d00-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d8d00-107">Atualize as propriedades de um objeto [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="d8d00-107">Update the properties of a [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d8d00-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d8d00-108">Prerequisites</span></span>
<span data-ttu-id="d8d00-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8d00-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8d00-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d8d00-111">Permission type</span></span>|<span data-ttu-id="d8d00-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d8d00-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d8d00-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d8d00-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d8d00-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8d00-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d8d00-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d8d00-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d8d00-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d8d00-116">Not supported.</span></span>|
|<span data-ttu-id="d8d00-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d8d00-117">Application</span></span>|<span data-ttu-id="d8d00-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d8d00-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d8d00-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d8d00-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d8d00-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d8d00-120">Request headers</span></span>
|<span data-ttu-id="d8d00-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d8d00-121">Header</span></span>|<span data-ttu-id="d8d00-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d8d00-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d8d00-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d8d00-123">Authorization</span></span>|<span data-ttu-id="d8d00-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d8d00-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d8d00-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d8d00-125">Accept</span></span>|<span data-ttu-id="d8d00-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d8d00-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8d00-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d8d00-127">Request body</span></span>
<span data-ttu-id="d8d00-128">No corpo da solicitação, fornece uma representação JSON para o objeto [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="d8d00-128">In the request body, supply a JSON representation for the [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) object.</span></span>

<span data-ttu-id="d8d00-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d8d00-129">The following table shows the properties that are required when you create the [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md).</span></span>

|<span data-ttu-id="d8d00-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d8d00-130">Property</span></span>|<span data-ttu-id="d8d00-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d8d00-131">Type</span></span>|<span data-ttu-id="d8d00-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8d00-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8d00-133">id</span><span class="sxs-lookup"><span data-stu-id="d8d00-133">id</span></span>|<span data-ttu-id="d8d00-134">String</span><span class="sxs-lookup"><span data-stu-id="d8d00-134">String</span></span>|<span data-ttu-id="d8d00-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d8d00-135">Key of the entity.</span></span> <span data-ttu-id="d8d00-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8d00-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8d00-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d8d00-137">lastModifiedDateTime</span></span>|<span data-ttu-id="d8d00-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8d00-138">DateTimeOffset</span></span>|<span data-ttu-id="d8d00-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="d8d00-139">DateTime the object was last modified.</span></span> <span data-ttu-id="d8d00-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8d00-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8d00-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d8d00-141">roleScopeTagIds</span></span>|<span data-ttu-id="d8d00-142">String collection</span><span class="sxs-lookup"><span data-stu-id="d8d00-142">String collection</span></span>|<span data-ttu-id="d8d00-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="d8d00-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d8d00-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8d00-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8d00-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d8d00-145">supportsScopeTags</span></span>|<span data-ttu-id="d8d00-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="d8d00-146">Boolean</span></span>|<span data-ttu-id="d8d00-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="d8d00-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d8d00-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="d8d00-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d8d00-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="d8d00-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d8d00-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d8d00-150">This property is read-only.</span></span> <span data-ttu-id="d8d00-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8d00-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8d00-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d8d00-152">createdDateTime</span></span>|<span data-ttu-id="d8d00-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8d00-153">DateTimeOffset</span></span>|<span data-ttu-id="d8d00-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="d8d00-154">DateTime the object was created.</span></span> <span data-ttu-id="d8d00-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8d00-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8d00-156">description</span><span class="sxs-lookup"><span data-stu-id="d8d00-156">description</span></span>|<span data-ttu-id="d8d00-157">String</span><span class="sxs-lookup"><span data-stu-id="d8d00-157">String</span></span>|<span data-ttu-id="d8d00-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d8d00-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d8d00-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8d00-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8d00-160">displayName</span><span class="sxs-lookup"><span data-stu-id="d8d00-160">displayName</span></span>|<span data-ttu-id="d8d00-161">String</span><span class="sxs-lookup"><span data-stu-id="d8d00-161">String</span></span>|<span data-ttu-id="d8d00-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d8d00-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d8d00-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8d00-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8d00-164">version</span><span class="sxs-lookup"><span data-stu-id="d8d00-164">version</span></span>|<span data-ttu-id="d8d00-165">Int32</span><span class="sxs-lookup"><span data-stu-id="d8d00-165">Int32</span></span>|<span data-ttu-id="d8d00-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d8d00-166">Version of the device configuration.</span></span> <span data-ttu-id="d8d00-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8d00-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8d00-168">networkName</span><span class="sxs-lookup"><span data-stu-id="d8d00-168">networkName</span></span>|<span data-ttu-id="d8d00-169">String</span><span class="sxs-lookup"><span data-stu-id="d8d00-169">String</span></span>|<span data-ttu-id="d8d00-170">Nome da rede</span><span class="sxs-lookup"><span data-stu-id="d8d00-170">Network Name</span></span>|
|<span data-ttu-id="d8d00-171">SSID</span><span class="sxs-lookup"><span data-stu-id="d8d00-171">ssid</span></span>|<span data-ttu-id="d8d00-172">String</span><span class="sxs-lookup"><span data-stu-id="d8d00-172">String</span></span>|<span data-ttu-id="d8d00-173">Este é o nome da rede Wi-Fi que é difundido para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="d8d00-173">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="d8d00-174">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="d8d00-174">connectAutomatically</span></span>|<span data-ttu-id="d8d00-175">Booliano</span><span class="sxs-lookup"><span data-stu-id="d8d00-175">Boolean</span></span>|<span data-ttu-id="d8d00-176">Conecte automaticamente quando esta rede estiver no intervalo.</span><span class="sxs-lookup"><span data-stu-id="d8d00-176">Connect automatically when this network is in range.</span></span> <span data-ttu-id="d8d00-177">Essa configuração como true ignorar o prompt do usuário e se conecte automaticamente o dispositivo à rede Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="d8d00-177">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="d8d00-178">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="d8d00-178">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="d8d00-179">Booliano</span><span class="sxs-lookup"><span data-stu-id="d8d00-179">Boolean</span></span>|<span data-ttu-id="d8d00-180">Quando definido como true, esse perfil força o dispositivo para se conectar a uma rede que não transmite seu SSID para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="d8d00-180">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="d8d00-181">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="d8d00-181">wiFiSecurityType</span></span>|[<span data-ttu-id="d8d00-182">androidWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="d8d00-182">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="d8d00-183">Indica se o ponto de extremidade Wi-Fi usa um tipo de segurança baseada em EAP.</span><span class="sxs-lookup"><span data-stu-id="d8d00-183">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="d8d00-184">Os valores possíveis são: `open` e `wpaEnterprise`.</span><span class="sxs-lookup"><span data-stu-id="d8d00-184">Possible values are: `open`, `wpaEnterprise`.</span></span>|



## <a name="response"></a><span data-ttu-id="d8d00-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8d00-185">Response</span></span>
<span data-ttu-id="d8d00-186">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d8d00-186">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8d00-187">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d8d00-187">Example</span></span>
### <a name="request"></a><span data-ttu-id="d8d00-188">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d8d00-188">Request</span></span>
<span data-ttu-id="d8d00-189">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d8d00-189">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 436

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="d8d00-190">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8d00-190">Response</span></span>
<span data-ttu-id="d8d00-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d8d00-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 618

{
  "@odata.type": "#microsoft.graph.androidWorkProfileWiFiConfiguration",
  "id": "8400d131-d131-8400-31d1-008431d10084",
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





