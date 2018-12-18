---
title: tipo de recurso de windowsNetworkIsolationPolicy
description: Política de isolamento de rede do Windows
author: tfitzmac
ms.openlocfilehash: af8cac99a359136bbc3d5d19842b56b57c80c6c9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323286"
---
# <a name="windowsnetworkisolationpolicy-resource-type"></a><span data-ttu-id="30817-103">tipo de recurso de windowsNetworkIsolationPolicy</span><span class="sxs-lookup"><span data-stu-id="30817-103">windowsNetworkIsolationPolicy resource type</span></span>

> <span data-ttu-id="30817-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="30817-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="30817-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="30817-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="30817-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="30817-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="30817-107">Política de isolamento de rede do Windows</span><span class="sxs-lookup"><span data-stu-id="30817-107">Windows Network Isolation Policy</span></span>
## <a name="properties"></a><span data-ttu-id="30817-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="30817-108">Properties</span></span>
|<span data-ttu-id="30817-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="30817-109">Property</span></span>|<span data-ttu-id="30817-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="30817-110">Type</span></span>|<span data-ttu-id="30817-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="30817-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30817-112">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="30817-112">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="30817-113">String collection</span><span class="sxs-lookup"><span data-stu-id="30817-113">String collection</span></span>|<span data-ttu-id="30817-114">Esta é a lista dos domínios que compõem os limites da empresa.</span><span class="sxs-lookup"><span data-stu-id="30817-114">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="30817-115">Dados de um desses domínios que será enviada para um dispositivo serão considerados dados corporativos e protegidos.</span><span class="sxs-lookup"><span data-stu-id="30817-115">Data from one of these domains that is sent to a device will be considered enterprise data and protected.</span></span> <span data-ttu-id="30817-116">Serão considerados um destino seguro para dados corporativos para serem compartilhadas desses locais.</span><span class="sxs-lookup"><span data-stu-id="30817-116">These locations will be considered a safe destination for enterprise data to be shared to.</span></span>|
|<span data-ttu-id="30817-117">enterpriseCloudResources</span><span class="sxs-lookup"><span data-stu-id="30817-117">enterpriseCloudResources</span></span>|<span data-ttu-id="30817-118">Coleção [proxiedDomain](../resources/intune-shared-proxieddomain.md)</span><span class="sxs-lookup"><span data-stu-id="30817-118">[proxiedDomain](../resources/intune-shared-proxieddomain.md) collection</span></span>|<span data-ttu-id="30817-119">Contém uma lista de domínios de recurso da empresa hospedado na nuvem que precisam ser protegidos.</span><span class="sxs-lookup"><span data-stu-id="30817-119">Contains a list of enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="30817-120">As conexões com esses recursos são consideradas dados corporativos.</span><span class="sxs-lookup"><span data-stu-id="30817-120">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="30817-121">Se um proxy for emparelhado com um recurso de nuvem, o tráfego para esse recurso será roteado pela rede da empresa por meio do servidor proxy indicado (na porta 80).</span><span class="sxs-lookup"><span data-stu-id="30817-121">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="30817-122">Um servidor proxy usado para essa finalidade também deve ser configurado usando a política de EnterpriseInternalProxyServers.</span><span class="sxs-lookup"><span data-stu-id="30817-122">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy.</span></span> <span data-ttu-id="30817-123">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="30817-123">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="30817-124">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="30817-124">enterpriseIPRanges</span></span>|<span data-ttu-id="30817-125">Coleção [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="30817-125">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="30817-126">Define os intervalos IP da empresa que definem os computadores da rede corporativa.</span><span class="sxs-lookup"><span data-stu-id="30817-126">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="30817-127">Dados provenientes desses computadores serão considerados parte da empresa e serão protegidos.</span><span class="sxs-lookup"><span data-stu-id="30817-127">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="30817-128">Serão considerados um destino seguro para dados corporativos para serem compartilhadas desses locais.</span><span class="sxs-lookup"><span data-stu-id="30817-128">These locations will be considered a safe destination for enterprise data to be shared to.</span></span> <span data-ttu-id="30817-129">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="30817-129">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="30817-130">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="30817-130">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="30817-131">String collection</span><span class="sxs-lookup"><span data-stu-id="30817-131">String collection</span></span>|<span data-ttu-id="30817-132">Esta é a lista separada por vírgula de servidores proxy internos.</span><span class="sxs-lookup"><span data-stu-id="30817-132">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="30817-133">Por exemplo, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span><span class="sxs-lookup"><span data-stu-id="30817-133">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="30817-134">Esses proxies foram configurados pelo administrador para se conectarem a recursos específicos na Internet.</span><span class="sxs-lookup"><span data-stu-id="30817-134">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="30817-135">Eles são considerados locais de rede da empresa.</span><span class="sxs-lookup"><span data-stu-id="30817-135">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="30817-136">Os proxies somente são utilizados na configuração da diretiva de EnterpriseCloudResources para forçar o tráfego para os recursos de nuvem correspondentes por meio desses proxies.</span><span class="sxs-lookup"><span data-stu-id="30817-136">The proxies are only leveraged in configuring the EnterpriseCloudResources policy to force traffic to the matched cloud resources through these proxies.</span></span>|
|<span data-ttu-id="30817-137">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="30817-137">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="30817-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="30817-138">Boolean</span></span>|<span data-ttu-id="30817-139">Valor booliano que informa ao cliente para aceitar a lista configurada e não usar heurística para tentar localizar outras sub-redes.</span><span class="sxs-lookup"><span data-stu-id="30817-139">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="30817-140">O padrão é false.</span><span class="sxs-lookup"><span data-stu-id="30817-140">Default is false.</span></span>|
|<span data-ttu-id="30817-141">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="30817-141">enterpriseProxyServers</span></span>|<span data-ttu-id="30817-142">String collection</span><span class="sxs-lookup"><span data-stu-id="30817-142">String collection</span></span>|<span data-ttu-id="30817-143">Esta é uma lista de servidores proxy.</span><span class="sxs-lookup"><span data-stu-id="30817-143">This is a list of proxy servers.</span></span> <span data-ttu-id="30817-144">Qualquer servidor não dessa lista é considerado fora da empresa.</span><span class="sxs-lookup"><span data-stu-id="30817-144">Any server not on this list is considered non-enterprise.</span></span>|
|<span data-ttu-id="30817-145">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="30817-145">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="30817-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="30817-146">Boolean</span></span>|<span data-ttu-id="30817-147">Valor booliano que informa ao cliente para aceitar a lista configurada de proxies e não tentar detectar outros proxies de trabalho.</span><span class="sxs-lookup"><span data-stu-id="30817-147">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="30817-148">O padrão é false</span><span class="sxs-lookup"><span data-stu-id="30817-148">Default is false</span></span>|
|<span data-ttu-id="30817-149">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="30817-149">neutralDomainResources</span></span>|<span data-ttu-id="30817-150">String collection</span><span class="sxs-lookup"><span data-stu-id="30817-150">String collection</span></span>|<span data-ttu-id="30817-151">Lista de nomes de domínio que podem ser usados para recursos pessoais ou de trabalho.</span><span class="sxs-lookup"><span data-stu-id="30817-151">List of domain names that can used for work or personal resource.</span></span>|

## <a name="relationships"></a><span data-ttu-id="30817-152">Relações</span><span class="sxs-lookup"><span data-stu-id="30817-152">Relationships</span></span>
<span data-ttu-id="30817-153">Nenhum</span><span class="sxs-lookup"><span data-stu-id="30817-153">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="30817-154">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="30817-154">JSON Representation</span></span>
<span data-ttu-id="30817-155">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="30817-155">Here is a JSON representation of the resource.</span></span>
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





