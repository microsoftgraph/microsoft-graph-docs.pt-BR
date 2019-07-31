---
title: Tipo de recurso proxiedDomain
description: Domínio com proxy
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3efbbf239e340b205aa84be62815ba00732a3a5d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967381"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="549b1-103">Tipo de recurso proxiedDomain</span><span class="sxs-lookup"><span data-stu-id="549b1-103">proxiedDomain resource type</span></span>

> <span data-ttu-id="549b1-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="549b1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="549b1-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="549b1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="549b1-106">Domínio com proxy</span><span class="sxs-lookup"><span data-stu-id="549b1-106">Proxied Domain</span></span>

## <a name="properties"></a><span data-ttu-id="549b1-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="549b1-107">Properties</span></span>
|<span data-ttu-id="549b1-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="549b1-108">Property</span></span>|<span data-ttu-id="549b1-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="549b1-109">Type</span></span>|<span data-ttu-id="549b1-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="549b1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="549b1-111">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="549b1-111">ipAddressOrFQDN</span></span>|<span data-ttu-id="549b1-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="549b1-112">String</span></span>|<span data-ttu-id="549b1-113">O endereço IP ou FQDN</span><span class="sxs-lookup"><span data-stu-id="549b1-113">The IP address or FQDN</span></span>|
|<span data-ttu-id="549b1-114">proxy</span><span class="sxs-lookup"><span data-stu-id="549b1-114">proxy</span></span>|<span data-ttu-id="549b1-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="549b1-115">String</span></span>|<span data-ttu-id="549b1-116">IP ou FQDN do proxy</span><span class="sxs-lookup"><span data-stu-id="549b1-116">Proxy IP or FQDN</span></span>|

## <a name="relationships"></a><span data-ttu-id="549b1-117">Relações</span><span class="sxs-lookup"><span data-stu-id="549b1-117">Relationships</span></span>
<span data-ttu-id="549b1-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="549b1-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="549b1-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="549b1-119">JSON Representation</span></span>
<span data-ttu-id="549b1-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="549b1-120">Here is a JSON representation of the resource.</span></span>
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





