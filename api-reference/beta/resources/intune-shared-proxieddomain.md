---
title: Tipo de recurso proxiedDomain
description: Domínio com proxy
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 352f466ad12f767feb68acd654d6d7d8133a25c3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523587"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="1ca97-103">Tipo de recurso proxiedDomain</span><span class="sxs-lookup"><span data-stu-id="1ca97-103">proxiedDomain resource type</span></span>

<span data-ttu-id="1ca97-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1ca97-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1ca97-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1ca97-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1ca97-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1ca97-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ca97-107">Domínio com proxy</span><span class="sxs-lookup"><span data-stu-id="1ca97-107">Proxied Domain</span></span>

## <a name="properties"></a><span data-ttu-id="1ca97-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1ca97-108">Properties</span></span>
|<span data-ttu-id="1ca97-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1ca97-109">Property</span></span>|<span data-ttu-id="1ca97-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="1ca97-110">Type</span></span>|<span data-ttu-id="1ca97-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1ca97-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ca97-112">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="1ca97-112">ipAddressOrFQDN</span></span>|<span data-ttu-id="1ca97-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1ca97-113">String</span></span>|<span data-ttu-id="1ca97-114">O endereço IP ou FQDN</span><span class="sxs-lookup"><span data-stu-id="1ca97-114">The IP address or FQDN</span></span>|
|<span data-ttu-id="1ca97-115">proxy</span><span class="sxs-lookup"><span data-stu-id="1ca97-115">proxy</span></span>|<span data-ttu-id="1ca97-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1ca97-116">String</span></span>|<span data-ttu-id="1ca97-117">IP ou FQDN do proxy</span><span class="sxs-lookup"><span data-stu-id="1ca97-117">Proxy IP or FQDN</span></span>|

## <a name="relationships"></a><span data-ttu-id="1ca97-118">Relações</span><span class="sxs-lookup"><span data-stu-id="1ca97-118">Relationships</span></span>
<span data-ttu-id="1ca97-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1ca97-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1ca97-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1ca97-120">JSON Representation</span></span>
<span data-ttu-id="1ca97-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1ca97-121">Here is a JSON representation of the resource.</span></span>
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



