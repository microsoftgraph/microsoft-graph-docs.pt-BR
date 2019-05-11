---
title: tipo de recurso windowsNetworkIsolationPolicy
description: Política de isolamento de rede do Windows
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 273e6d7689a81e7f64ec2000f881e963e5cbd2f8
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943939"
---
# <a name="windowsnetworkisolationpolicy-resource-type"></a><span data-ttu-id="61dea-103">tipo de recurso windowsNetworkIsolationPolicy</span><span class="sxs-lookup"><span data-stu-id="61dea-103">windowsNetworkIsolationPolicy resource type</span></span>

> <span data-ttu-id="61dea-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="61dea-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="61dea-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="61dea-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="61dea-106">Política de isolamento de rede do Windows</span><span class="sxs-lookup"><span data-stu-id="61dea-106">Windows Network Isolation Policy</span></span>

## <a name="properties"></a><span data-ttu-id="61dea-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="61dea-107">Properties</span></span>
|<span data-ttu-id="61dea-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="61dea-108">Property</span></span>|<span data-ttu-id="61dea-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="61dea-109">Type</span></span>|<span data-ttu-id="61dea-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="61dea-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61dea-111">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="61dea-111">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="61dea-112">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="61dea-112">String collection</span></span>|<span data-ttu-id="61dea-113">Esta é a lista dos domínios que compõem os limites da empresa.</span><span class="sxs-lookup"><span data-stu-id="61dea-113">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="61dea-114">Os dados de um desses domínios enviados para um dispositivo serão considerados dados corporativos e protegidos.</span><span class="sxs-lookup"><span data-stu-id="61dea-114">Data from one of these domains that is sent to a device will be considered enterprise data and protected.</span></span> <span data-ttu-id="61dea-115">Esses locais serão considerados um destino seguro para que os dados corporativos sejam compartilhados.</span><span class="sxs-lookup"><span data-stu-id="61dea-115">These locations will be considered a safe destination for enterprise data to be shared to.</span></span>|
|<span data-ttu-id="61dea-116">enterpriseCloudResources</span><span class="sxs-lookup"><span data-stu-id="61dea-116">enterpriseCloudResources</span></span>|<span data-ttu-id="61dea-117">Coleção [proxiedDomain](../resources/intune-shared-proxieddomain.md)</span><span class="sxs-lookup"><span data-stu-id="61dea-117">[proxiedDomain](../resources/intune-shared-proxieddomain.md) collection</span></span>|<span data-ttu-id="61dea-118">Contém uma lista de domínios de recursos da empresa hospedados na nuvem que precisam ser protegidos.</span><span class="sxs-lookup"><span data-stu-id="61dea-118">Contains a list of enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="61dea-119">As conexões com esses recursos são consideradas dados corporativos.</span><span class="sxs-lookup"><span data-stu-id="61dea-119">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="61dea-120">Se um proxy for emparelhado com um recurso de nuvem, o tráfego para esse recurso será roteado pela rede da empresa por meio do servidor proxy indicado (na porta 80).</span><span class="sxs-lookup"><span data-stu-id="61dea-120">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="61dea-121">Um servidor proxy usado para essa finalidade também deve ser configurado usando a política EnterpriseInternalProxyServers.</span><span class="sxs-lookup"><span data-stu-id="61dea-121">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy.</span></span> <span data-ttu-id="61dea-122">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="61dea-122">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="61dea-123">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="61dea-123">enterpriseIPRanges</span></span>|<span data-ttu-id="61dea-124">Coleção [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="61dea-124">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="61dea-125">Define os intervalos IP da empresa que definem os computadores da rede corporativa.</span><span class="sxs-lookup"><span data-stu-id="61dea-125">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="61dea-126">Dados provenientes desses computadores serão considerados parte da empresa e serão protegidos.</span><span class="sxs-lookup"><span data-stu-id="61dea-126">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="61dea-127">Esses locais serão considerados um destino seguro para que os dados corporativos sejam compartilhados.</span><span class="sxs-lookup"><span data-stu-id="61dea-127">These locations will be considered a safe destination for enterprise data to be shared to.</span></span> <span data-ttu-id="61dea-128">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="61dea-128">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="61dea-129">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="61dea-129">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="61dea-130">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="61dea-130">String collection</span></span>|<span data-ttu-id="61dea-131">Esta é a lista separada por vírgula de servidores proxy internos.</span><span class="sxs-lookup"><span data-stu-id="61dea-131">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="61dea-132">Por exemplo, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span><span class="sxs-lookup"><span data-stu-id="61dea-132">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="61dea-133">Esses proxies foram configurados pelo administrador para se conectarem a recursos específicos na Internet.</span><span class="sxs-lookup"><span data-stu-id="61dea-133">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="61dea-134">Eles são considerados locais de rede da empresa.</span><span class="sxs-lookup"><span data-stu-id="61dea-134">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="61dea-135">Os proxies são utilizados apenas na configuração da política EnterpriseCloudResources para forçar o tráfego para os recursos de nuvem correspondentes através desses proxies.</span><span class="sxs-lookup"><span data-stu-id="61dea-135">The proxies are only leveraged in configuring the EnterpriseCloudResources policy to force traffic to the matched cloud resources through these proxies.</span></span>|
|<span data-ttu-id="61dea-136">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="61dea-136">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="61dea-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="61dea-137">Boolean</span></span>|<span data-ttu-id="61dea-138">Valor booliano que informa ao cliente para aceitar a lista configurada e não usar heurística para tentar localizar outras sub-redes.</span><span class="sxs-lookup"><span data-stu-id="61dea-138">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="61dea-139">O padrão é false.</span><span class="sxs-lookup"><span data-stu-id="61dea-139">Default is false.</span></span>|
|<span data-ttu-id="61dea-140">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="61dea-140">enterpriseProxyServers</span></span>|<span data-ttu-id="61dea-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="61dea-141">String collection</span></span>|<span data-ttu-id="61dea-142">Esta é uma lista de servidores proxy.</span><span class="sxs-lookup"><span data-stu-id="61dea-142">This is a list of proxy servers.</span></span> <span data-ttu-id="61dea-143">Qualquer servidor que não esteja na lista é considerado não corporativo.</span><span class="sxs-lookup"><span data-stu-id="61dea-143">Any server not on this list is considered non-enterprise.</span></span>|
|<span data-ttu-id="61dea-144">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="61dea-144">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="61dea-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="61dea-145">Boolean</span></span>|<span data-ttu-id="61dea-146">Valor booliano que informa ao cliente para aceitar a lista configurada de proxies e não tentar detectar outros proxies de trabalho.</span><span class="sxs-lookup"><span data-stu-id="61dea-146">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="61dea-147">O padrão é false</span><span class="sxs-lookup"><span data-stu-id="61dea-147">Default is false</span></span>|
|<span data-ttu-id="61dea-148">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="61dea-148">neutralDomainResources</span></span>|<span data-ttu-id="61dea-149">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="61dea-149">String collection</span></span>|<span data-ttu-id="61dea-150">Lista de nomes de domínio que podem ser usados para trabalho ou recurso pessoal.</span><span class="sxs-lookup"><span data-stu-id="61dea-150">List of domain names that can used for work or personal resource.</span></span>|

## <a name="relationships"></a><span data-ttu-id="61dea-151">Relações</span><span class="sxs-lookup"><span data-stu-id="61dea-151">Relationships</span></span>
<span data-ttu-id="61dea-152">Nenhum</span><span class="sxs-lookup"><span data-stu-id="61dea-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="61dea-153">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="61dea-153">JSON Representation</span></span>
<span data-ttu-id="61dea-154">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="61dea-154">Here is a JSON representation of the resource.</span></span>
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




