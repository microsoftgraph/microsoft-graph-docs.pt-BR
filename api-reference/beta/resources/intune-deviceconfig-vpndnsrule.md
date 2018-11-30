---
title: tipo de recurso de vpnDnsRule
description: Definição de regra de DNS da VPN.
ms.openlocfilehash: dcb6a0d3a0cd709e8a88835c553f9f29cb094e57
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034906"
---
# <a name="vpndnsrule-resource-type"></a><span data-ttu-id="4cb13-103">tipo de recurso de vpnDnsRule</span><span class="sxs-lookup"><span data-stu-id="4cb13-103">vpnDnsRule resource type</span></span>

> <span data-ttu-id="4cb13-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4cb13-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4cb13-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4cb13-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4cb13-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4cb13-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4cb13-107">Definição de regra de DNS da VPN.</span><span class="sxs-lookup"><span data-stu-id="4cb13-107">VPN DNS Rule definition.</span></span>
## <a name="properties"></a><span data-ttu-id="4cb13-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4cb13-108">Properties</span></span>
|<span data-ttu-id="4cb13-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4cb13-109">Property</span></span>|<span data-ttu-id="4cb13-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="4cb13-110">Type</span></span>|<span data-ttu-id="4cb13-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4cb13-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4cb13-112">name</span><span class="sxs-lookup"><span data-stu-id="4cb13-112">name</span></span>|<span data-ttu-id="4cb13-113">String</span><span class="sxs-lookup"><span data-stu-id="4cb13-113">String</span></span>|<span data-ttu-id="4cb13-114">Nome.</span><span class="sxs-lookup"><span data-stu-id="4cb13-114">Name.</span></span>|
|<span data-ttu-id="4cb13-115">servidores</span><span class="sxs-lookup"><span data-stu-id="4cb13-115">servers</span></span>|<span data-ttu-id="4cb13-116">String collection</span><span class="sxs-lookup"><span data-stu-id="4cb13-116">String collection</span></span>|<span data-ttu-id="4cb13-117">Servidores.</span><span class="sxs-lookup"><span data-stu-id="4cb13-117">Servers.</span></span>|
|<span data-ttu-id="4cb13-118">proxyServerUri</span><span class="sxs-lookup"><span data-stu-id="4cb13-118">proxyServerUri</span></span>|<span data-ttu-id="4cb13-119">String</span><span class="sxs-lookup"><span data-stu-id="4cb13-119">String</span></span>|<span data-ttu-id="4cb13-120">Uri do servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="4cb13-120">Proxy Server Uri.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4cb13-121">Relações</span><span class="sxs-lookup"><span data-stu-id="4cb13-121">Relationships</span></span>
<span data-ttu-id="4cb13-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4cb13-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4cb13-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4cb13-123">JSON Representation</span></span>
<span data-ttu-id="4cb13-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4cb13-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnDnsRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnDnsRule",
  "name": "String",
  "servers": [
    "String"
  ],
  "proxyServerUri": "String"
}
```





