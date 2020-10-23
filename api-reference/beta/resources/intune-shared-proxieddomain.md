---
title: Tipo de recurso proxiedDomain
description: Domínio com proxy
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ac366425621867e75dfc1a0c1ae8b09336ed0214
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48704690"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="2ecd6-103">Tipo de recurso proxiedDomain</span><span class="sxs-lookup"><span data-stu-id="2ecd6-103">proxiedDomain resource type</span></span>

<span data-ttu-id="2ecd6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ecd6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2ecd6-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2ecd6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2ecd6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2ecd6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ecd6-107">Domínio com proxy</span><span class="sxs-lookup"><span data-stu-id="2ecd6-107">Proxied Domain</span></span>

## <a name="properties"></a><span data-ttu-id="2ecd6-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2ecd6-108">Properties</span></span>
|<span data-ttu-id="2ecd6-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2ecd6-109">Property</span></span>|<span data-ttu-id="2ecd6-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="2ecd6-110">Type</span></span>|<span data-ttu-id="2ecd6-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ecd6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ecd6-112">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="2ecd6-112">ipAddressOrFQDN</span></span>|<span data-ttu-id="2ecd6-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2ecd6-113">String</span></span>|<span data-ttu-id="2ecd6-114">O endereço IP ou FQDN</span><span class="sxs-lookup"><span data-stu-id="2ecd6-114">The IP address or FQDN</span></span>|
|<span data-ttu-id="2ecd6-115">proxy</span><span class="sxs-lookup"><span data-stu-id="2ecd6-115">proxy</span></span>|<span data-ttu-id="2ecd6-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2ecd6-116">String</span></span>|<span data-ttu-id="2ecd6-117">IP ou FQDN do proxy</span><span class="sxs-lookup"><span data-stu-id="2ecd6-117">Proxy IP or FQDN</span></span>|

## <a name="relationships"></a><span data-ttu-id="2ecd6-118">Relações</span><span class="sxs-lookup"><span data-stu-id="2ecd6-118">Relationships</span></span>
<span data-ttu-id="2ecd6-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2ecd6-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2ecd6-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2ecd6-120">JSON Representation</span></span>
<span data-ttu-id="2ecd6-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2ecd6-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.proxiedDomain"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.proxiedDomain",
  "ipAddressOrFQDN": "String",
  "proxy": "String"
}
```





