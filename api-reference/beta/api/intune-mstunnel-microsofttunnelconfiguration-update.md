---
title: Atualizar microsoftTunnelConfiguration
description: Atualize as propriedades de um objeto microsoftTunnelConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 258fe480a1154d12b3c6c7e716329bb704e09eef
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51125916"
---
# <a name="update-microsofttunnelconfiguration"></a><span data-ttu-id="8c097-103">Atualizar microsoftTunnelConfiguration</span><span class="sxs-lookup"><span data-stu-id="8c097-103">Update microsoftTunnelConfiguration</span></span>

<span data-ttu-id="8c097-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c097-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8c097-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8c097-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8c097-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8c097-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c097-107">Atualize as propriedades de um [objeto microsoftTunnelConfiguration.](../resources/intune-mstunnel-microsofttunnelconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8c097-107">Update the properties of a [microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8c097-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8c097-108">Prerequisites</span></span>
<span data-ttu-id="8c097-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c097-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c097-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8c097-111">Permission type</span></span>|<span data-ttu-id="8c097-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8c097-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c097-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8c097-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8c097-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c097-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8c097-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8c097-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c097-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8c097-116">Not supported.</span></span>|
|<span data-ttu-id="8c097-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8c097-117">Application</span></span>|<span data-ttu-id="8c097-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c097-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c097-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8c097-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/microsoftTunnelConfigurations/{microsoftTunnelConfigurationId}
PATCH /deviceManagement/microsoftTunnelSites/{microsoftTunnelSiteId}/microsoftTunnelConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="8c097-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8c097-120">Request headers</span></span>
|<span data-ttu-id="8c097-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8c097-121">Header</span></span>|<span data-ttu-id="8c097-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8c097-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8c097-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8c097-123">Authorization</span></span>|<span data-ttu-id="8c097-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8c097-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8c097-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8c097-125">Accept</span></span>|<span data-ttu-id="8c097-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8c097-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c097-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8c097-127">Request body</span></span>
<span data-ttu-id="8c097-128">No corpo da solicitação, fornece uma representação JSON para o [objeto microsoftTunnelConfiguration.](../resources/intune-mstunnel-microsofttunnelconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8c097-128">In the request body, supply a JSON representation for the [microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md) object.</span></span>

<span data-ttu-id="8c097-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8c097-129">The following table shows the properties that are required when you create the [microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md).</span></span>

|<span data-ttu-id="8c097-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8c097-130">Property</span></span>|<span data-ttu-id="8c097-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="8c097-131">Type</span></span>|<span data-ttu-id="8c097-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c097-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c097-133">id</span><span class="sxs-lookup"><span data-stu-id="8c097-133">id</span></span>|<span data-ttu-id="8c097-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c097-134">String</span></span>|<span data-ttu-id="8c097-135">Id do MicrosoftTunnelConfiguration</span><span class="sxs-lookup"><span data-stu-id="8c097-135">The MicrosoftTunnelConfiguration's Id</span></span>|
|<span data-ttu-id="8c097-136">displayName</span><span class="sxs-lookup"><span data-stu-id="8c097-136">displayName</span></span>|<span data-ttu-id="8c097-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c097-137">String</span></span>|<span data-ttu-id="8c097-138">O nome de exibição do MicrosoftTunnelConfiguration</span><span class="sxs-lookup"><span data-stu-id="8c097-138">The MicrosoftTunnelConfiguration's display name</span></span>|
|<span data-ttu-id="8c097-139">descrição</span><span class="sxs-lookup"><span data-stu-id="8c097-139">description</span></span>|<span data-ttu-id="8c097-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c097-140">String</span></span>|<span data-ttu-id="8c097-141">A descrição do MicrosoftTunnelConfiguration</span><span class="sxs-lookup"><span data-stu-id="8c097-141">The MicrosoftTunnelConfiguration's description</span></span>|
|<span data-ttu-id="8c097-142">network</span><span class="sxs-lookup"><span data-stu-id="8c097-142">network</span></span>|<span data-ttu-id="8c097-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c097-143">String</span></span>|<span data-ttu-id="8c097-144">A sub-rede que será usada para alocar endereço virtual para os clientes</span><span class="sxs-lookup"><span data-stu-id="8c097-144">The subnet that will be used to allocate virtual address for the clients</span></span>|
|<span data-ttu-id="8c097-145">dnsServers</span><span class="sxs-lookup"><span data-stu-id="8c097-145">dnsServers</span></span>|<span data-ttu-id="8c097-146">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c097-146">String collection</span></span>|<span data-ttu-id="8c097-147">Os servidores DNS que serão usados pelos clientes</span><span class="sxs-lookup"><span data-stu-id="8c097-147">The DNS servers that will be used by the clients</span></span>|
|<span data-ttu-id="8c097-148">defaultDomainSuffix</span><span class="sxs-lookup"><span data-stu-id="8c097-148">defaultDomainSuffix</span></span>|<span data-ttu-id="8c097-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c097-149">String</span></span>|<span data-ttu-id="8c097-150">O apêndice Domínio Padrão que será usado pelos clientes</span><span class="sxs-lookup"><span data-stu-id="8c097-150">The Default Domain appendix that will be used by the clients</span></span>|
|<span data-ttu-id="8c097-151">routesInclude</span><span class="sxs-lookup"><span data-stu-id="8c097-151">routesInclude</span></span>|<span data-ttu-id="8c097-152">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c097-152">String collection</span></span>|<span data-ttu-id="8c097-153">Os routs que serão roteados pelo servidor</span><span class="sxs-lookup"><span data-stu-id="8c097-153">The routs that will be routed by the server</span></span>|
|<span data-ttu-id="8c097-154">routesExclude</span><span class="sxs-lookup"><span data-stu-id="8c097-154">routesExclude</span></span>|<span data-ttu-id="8c097-155">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c097-155">String collection</span></span>|<span data-ttu-id="8c097-156">Subconjunto das rotas que não serão roteadas pelo servidor</span><span class="sxs-lookup"><span data-stu-id="8c097-156">Subsets of the routes that will not be routed by the server</span></span>|
|<span data-ttu-id="8c097-157">splitDNS</span><span class="sxs-lookup"><span data-stu-id="8c097-157">splitDNS</span></span>|<span data-ttu-id="8c097-158">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c097-158">String collection</span></span>|<span data-ttu-id="8c097-159">Os domínios que serão resolvidos usando os servidores dns fornecidos</span><span class="sxs-lookup"><span data-stu-id="8c097-159">The domains that will be resolved using the provided dns servers</span></span>|
|<span data-ttu-id="8c097-160">listenPort</span><span class="sxs-lookup"><span data-stu-id="8c097-160">listenPort</span></span>|<span data-ttu-id="8c097-161">Int32</span><span class="sxs-lookup"><span data-stu-id="8c097-161">Int32</span></span>|<span data-ttu-id="8c097-162">A porta que o TCP e o UPD escutarão no servidor</span><span class="sxs-lookup"><span data-stu-id="8c097-162">The port that both TCP and UPD will listen over on the server</span></span>|
|<span data-ttu-id="8c097-163">advancedSettings</span><span class="sxs-lookup"><span data-stu-id="8c097-163">advancedSettings</span></span>|<span data-ttu-id="8c097-164">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="8c097-164">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="8c097-165">Configurações adicionais que podem ser aplicadas ao servidor</span><span class="sxs-lookup"><span data-stu-id="8c097-165">Additional settings that may be applied to the server</span></span>|
|<span data-ttu-id="8c097-166">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="8c097-166">lastUpdateDateTime</span></span>|<span data-ttu-id="8c097-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c097-167">DateTimeOffset</span></span>|<span data-ttu-id="8c097-168">Quando o MicrosoftTunnelConfiguration foi atualizado pela última vez</span><span class="sxs-lookup"><span data-stu-id="8c097-168">When the MicrosoftTunnelConfiguration was last updated</span></span>|
|<span data-ttu-id="8c097-169">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8c097-169">roleScopeTagIds</span></span>|<span data-ttu-id="8c097-170">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c097-170">String collection</span></span>|<span data-ttu-id="8c097-171">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="8c097-171">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="8c097-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c097-172">Response</span></span>
<span data-ttu-id="8c097-173">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8c097-173">If successful, this method returns a `200 OK` response code and an updated [microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c097-174">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8c097-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="8c097-175">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8c097-175">Request</span></span>
<span data-ttu-id="8c097-176">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8c097-176">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/microsoftTunnelConfigurations/{microsoftTunnelConfigurationId}
Content-type: application/json
Content-length: 748

{
  "@odata.type": "#microsoft.graph.microsoftTunnelConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "network": "Network value",
  "dnsServers": [
    "Dns Servers value"
  ],
  "defaultDomainSuffix": "Default Domain Suffix value",
  "routesInclude": [
    "Routes Include value"
  ],
  "routesExclude": [
    "Routes Exclude value"
  ],
  "splitDNS": [
    "Split DNS value"
  ],
  "listenPort": 10,
  "advancedSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="8c097-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c097-177">Response</span></span>
<span data-ttu-id="8c097-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8c097-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 797

{
  "@odata.type": "#microsoft.graph.microsoftTunnelConfiguration",
  "id": "b8bdb469-b469-b8bd-69b4-bdb869b4bdb8",
  "displayName": "Display Name value",
  "description": "Description value",
  "network": "Network value",
  "dnsServers": [
    "Dns Servers value"
  ],
  "defaultDomainSuffix": "Default Domain Suffix value",
  "routesInclude": [
    "Routes Include value"
  ],
  "routesExclude": [
    "Routes Exclude value"
  ],
  "splitDNS": [
    "Split DNS value"
  ],
  "listenPort": 10,
  "advancedSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```




