---
title: tipo de recurso windowsNetworkIsolationPolicy
description: Política de isolamento de rede do Windows
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 504bd8471751653138ebe3c4b5488ca6041ae18f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529008"
---
# <a name="windowsnetworkisolationpolicy-resource-type"></a><span data-ttu-id="2a1e0-103">tipo de recurso windowsNetworkIsolationPolicy</span><span class="sxs-lookup"><span data-stu-id="2a1e0-103">windowsNetworkIsolationPolicy resource type</span></span>

<span data-ttu-id="2a1e0-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="2a1e0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2a1e0-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2a1e0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2a1e0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2a1e0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a1e0-107">Política de isolamento de rede do Windows</span><span class="sxs-lookup"><span data-stu-id="2a1e0-107">Windows Network Isolation Policy</span></span>

## <a name="properties"></a><span data-ttu-id="2a1e0-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2a1e0-108">Properties</span></span>
|<span data-ttu-id="2a1e0-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2a1e0-109">Property</span></span>|<span data-ttu-id="2a1e0-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="2a1e0-110">Type</span></span>|<span data-ttu-id="2a1e0-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2a1e0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a1e0-112">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="2a1e0-112">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="2a1e0-113">String collection</span><span class="sxs-lookup"><span data-stu-id="2a1e0-113">String collection</span></span>|<span data-ttu-id="2a1e0-114">Esta é a lista dos domínios que compõem os limites da empresa.</span><span class="sxs-lookup"><span data-stu-id="2a1e0-114">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="2a1e0-115">Os dados de um desses domínios enviados para um dispositivo serão considerados dados corporativos e protegidos.</span><span class="sxs-lookup"><span data-stu-id="2a1e0-115">Data from one of these domains that is sent to a device will be considered enterprise data and protected.</span></span> <span data-ttu-id="2a1e0-116">Esses locais serão considerados um destino seguro para que os dados corporativos sejam compartilhados.</span><span class="sxs-lookup"><span data-stu-id="2a1e0-116">These locations will be considered a safe destination for enterprise data to be shared to.</span></span>|
|<span data-ttu-id="2a1e0-117">enterpriseCloudResources</span><span class="sxs-lookup"><span data-stu-id="2a1e0-117">enterpriseCloudResources</span></span>|<span data-ttu-id="2a1e0-118">Coleção [proxiedDomain](../resources/intune-shared-proxieddomain.md)</span><span class="sxs-lookup"><span data-stu-id="2a1e0-118">[proxiedDomain](../resources/intune-shared-proxieddomain.md) collection</span></span>|<span data-ttu-id="2a1e0-119">Contém uma lista de domínios de recursos da empresa hospedados na nuvem que precisam ser protegidos.</span><span class="sxs-lookup"><span data-stu-id="2a1e0-119">Contains a list of enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="2a1e0-120">As conexões com esses recursos são consideradas dados corporativos.</span><span class="sxs-lookup"><span data-stu-id="2a1e0-120">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="2a1e0-121">Se um proxy for emparelhado com um recurso de nuvem, o tráfego para esse recurso será roteado pela rede da empresa por meio do servidor proxy indicado (na porta 80).</span><span class="sxs-lookup"><span data-stu-id="2a1e0-121">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="2a1e0-122">Um servidor proxy usado para essa finalidade também deve ser configurado usando a política EnterpriseInternalProxyServers.</span><span class="sxs-lookup"><span data-stu-id="2a1e0-122">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy.</span></span> <span data-ttu-id="2a1e0-123">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="2a1e0-123">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="2a1e0-124">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="2a1e0-124">enterpriseIPRanges</span></span>|<span data-ttu-id="2a1e0-125">Coleção [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="2a1e0-125">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="2a1e0-126">Define os intervalos IP da empresa que definem os computadores da rede corporativa.</span><span class="sxs-lookup"><span data-stu-id="2a1e0-126">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="2a1e0-127">Dados provenientes desses computadores serão considerados parte da empresa e serão protegidos.</span><span class="sxs-lookup"><span data-stu-id="2a1e0-127">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="2a1e0-128">Esses locais serão considerados um destino seguro para que os dados corporativos sejam compartilhados.</span><span class="sxs-lookup"><span data-stu-id="2a1e0-128">These locations will be considered a safe destination for enterprise data to be shared to.</span></span> <span data-ttu-id="2a1e0-129">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="2a1e0-129">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="2a1e0-130">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="2a1e0-130">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="2a1e0-131">String collection</span><span class="sxs-lookup"><span data-stu-id="2a1e0-131">String collection</span></span>|<span data-ttu-id="2a1e0-132">Esta é a lista separada por vírgula de servidores proxy internos.</span><span class="sxs-lookup"><span data-stu-id="2a1e0-132">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="2a1e0-133">Por exemplo, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span><span class="sxs-lookup"><span data-stu-id="2a1e0-133">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="2a1e0-134">Esses proxies foram configurados pelo administrador para se conectarem a recursos específicos na Internet.</span><span class="sxs-lookup"><span data-stu-id="2a1e0-134">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="2a1e0-135">Eles são considerados locais de rede da empresa.</span><span class="sxs-lookup"><span data-stu-id="2a1e0-135">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="2a1e0-136">Os proxies são utilizados apenas na configuração da política EnterpriseCloudResources para forçar o tráfego para os recursos de nuvem correspondentes através desses proxies.</span><span class="sxs-lookup"><span data-stu-id="2a1e0-136">The proxies are only leveraged in configuring the EnterpriseCloudResources policy to force traffic to the matched cloud resources through these proxies.</span></span>|
|<span data-ttu-id="2a1e0-137">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="2a1e0-137">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="2a1e0-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="2a1e0-138">Boolean</span></span>|<span data-ttu-id="2a1e0-139">Valor booliano que informa ao cliente para aceitar a lista configurada e não usar heurística para tentar localizar outras sub-redes.</span><span class="sxs-lookup"><span data-stu-id="2a1e0-139">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="2a1e0-140">O padrão é false.</span><span class="sxs-lookup"><span data-stu-id="2a1e0-140">Default is false.</span></span>|
|<span data-ttu-id="2a1e0-141">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="2a1e0-141">enterpriseProxyServers</span></span>|<span data-ttu-id="2a1e0-142">String collection</span><span class="sxs-lookup"><span data-stu-id="2a1e0-142">String collection</span></span>|<span data-ttu-id="2a1e0-143">Esta é uma lista de servidores proxy.</span><span class="sxs-lookup"><span data-stu-id="2a1e0-143">This is a list of proxy servers.</span></span> <span data-ttu-id="2a1e0-144">Qualquer servidor que não esteja na lista é considerado não corporativo.</span><span class="sxs-lookup"><span data-stu-id="2a1e0-144">Any server not on this list is considered non-enterprise.</span></span>|
|<span data-ttu-id="2a1e0-145">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="2a1e0-145">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="2a1e0-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="2a1e0-146">Boolean</span></span>|<span data-ttu-id="2a1e0-147">Valor booliano que informa ao cliente para aceitar a lista configurada de proxies e não tentar detectar outros proxies de trabalho.</span><span class="sxs-lookup"><span data-stu-id="2a1e0-147">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="2a1e0-148">O padrão é false</span><span class="sxs-lookup"><span data-stu-id="2a1e0-148">Default is false</span></span>|
|<span data-ttu-id="2a1e0-149">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="2a1e0-149">neutralDomainResources</span></span>|<span data-ttu-id="2a1e0-150">String collection</span><span class="sxs-lookup"><span data-stu-id="2a1e0-150">String collection</span></span>|<span data-ttu-id="2a1e0-151">Lista de nomes de domínio que podem ser usados para trabalho ou recurso pessoal.</span><span class="sxs-lookup"><span data-stu-id="2a1e0-151">List of domain names that can used for work or personal resource.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2a1e0-152">Relações</span><span class="sxs-lookup"><span data-stu-id="2a1e0-152">Relationships</span></span>
<span data-ttu-id="2a1e0-153">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2a1e0-153">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2a1e0-154">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2a1e0-154">JSON Representation</span></span>
<span data-ttu-id="2a1e0-155">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2a1e0-155">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsNetworkIsolationPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsNetworkIsolationPolicy",
  "enterpriseNetworkDomainNames": [
    "String"
  ],
  "enterpriseCloudResources": [
    {
      "@odata.type": "microsoft.graph.proxiedDomain",
      "ipAddressOrFQDN": "String",
      "proxy": "String"
    }
  ],
  "enterpriseIPRanges": [
    {
      "@odata.type": "microsoft.graph.iPv6Range",
      "lowerAddress": "String",
      "upperAddress": "String"
    }
  ],
  "enterpriseInternalProxyServers": [
    "String"
  ],
  "enterpriseIPRangesAreAuthoritative": true,
  "enterpriseProxyServers": [
    "String"
  ],
  "enterpriseProxyServersAreAuthoritative": true,
  "neutralDomainResources": [
    "String"
  ]
}
```



