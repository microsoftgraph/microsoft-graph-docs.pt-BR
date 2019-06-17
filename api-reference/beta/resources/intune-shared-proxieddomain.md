---
title: Tipo de recurso proxiedDomain
description: Domínio com proxy
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9260d0fc9b446e7f61bfebff577ac10f9f3e4aee
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34986400"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="767ff-103">Tipo de recurso proxiedDomain</span><span class="sxs-lookup"><span data-stu-id="767ff-103">proxiedDomain resource type</span></span>

> <span data-ttu-id="767ff-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="767ff-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="767ff-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="767ff-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="767ff-106">Domínio com proxy</span><span class="sxs-lookup"><span data-stu-id="767ff-106">Proxied Domain</span></span>

## <a name="properties"></a><span data-ttu-id="767ff-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="767ff-107">Properties</span></span>
|<span data-ttu-id="767ff-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="767ff-108">Property</span></span>|<span data-ttu-id="767ff-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="767ff-109">Type</span></span>|<span data-ttu-id="767ff-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="767ff-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="767ff-111">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="767ff-111">ipAddressOrFQDN</span></span>|<span data-ttu-id="767ff-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="767ff-112">String</span></span>|<span data-ttu-id="767ff-113">O endereço IP ou FQDN</span><span class="sxs-lookup"><span data-stu-id="767ff-113">The IP address or FQDN</span></span>|
|<span data-ttu-id="767ff-114">proxy</span><span class="sxs-lookup"><span data-stu-id="767ff-114">proxy</span></span>|<span data-ttu-id="767ff-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="767ff-115">String</span></span>|<span data-ttu-id="767ff-116">IP ou FQDN do proxy</span><span class="sxs-lookup"><span data-stu-id="767ff-116">Proxy IP or FQDN</span></span>|

## <a name="relationships"></a><span data-ttu-id="767ff-117">Relações</span><span class="sxs-lookup"><span data-stu-id="767ff-117">Relationships</span></span>
<span data-ttu-id="767ff-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="767ff-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="767ff-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="767ff-119">JSON Representation</span></span>
<span data-ttu-id="767ff-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="767ff-120">Here is a JSON representation of the resource.</span></span>
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





