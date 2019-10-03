---
title: Tipo de recurso proxiedDomain
description: Domínio com proxy
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8d4b100fd312576fdb81f09e06b51d7e74bef4c0
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37366955"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="ddd32-103">Tipo de recurso proxiedDomain</span><span class="sxs-lookup"><span data-stu-id="ddd32-103">proxiedDomain resource type</span></span>

> <span data-ttu-id="ddd32-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ddd32-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ddd32-105">Domínio com proxy</span><span class="sxs-lookup"><span data-stu-id="ddd32-105">Proxied Domain</span></span>

## <a name="properties"></a><span data-ttu-id="ddd32-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ddd32-106">Properties</span></span>
|<span data-ttu-id="ddd32-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ddd32-107">Property</span></span>|<span data-ttu-id="ddd32-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="ddd32-108">Type</span></span>|<span data-ttu-id="ddd32-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ddd32-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ddd32-110">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="ddd32-110">ipAddressOrFQDN</span></span>|<span data-ttu-id="ddd32-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ddd32-111">String</span></span>|<span data-ttu-id="ddd32-112">O endereço IP ou FQDN</span><span class="sxs-lookup"><span data-stu-id="ddd32-112">The IP address or FQDN</span></span>|
|<span data-ttu-id="ddd32-113">proxy</span><span class="sxs-lookup"><span data-stu-id="ddd32-113">proxy</span></span>|<span data-ttu-id="ddd32-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ddd32-114">String</span></span>|<span data-ttu-id="ddd32-115">IP ou FQDN do proxy</span><span class="sxs-lookup"><span data-stu-id="ddd32-115">Proxy IP or FQDN</span></span>|

## <a name="relationships"></a><span data-ttu-id="ddd32-116">Relações</span><span class="sxs-lookup"><span data-stu-id="ddd32-116">Relationships</span></span>
<span data-ttu-id="ddd32-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ddd32-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ddd32-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ddd32-118">JSON Representation</span></span>
<span data-ttu-id="ddd32-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ddd32-119">Here is a JSON representation of the resource.</span></span>
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




