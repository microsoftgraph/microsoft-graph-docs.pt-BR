---
title: Tipo de recurso proxiedDomain
description: Domínio com proxy
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0e7530bf3bc08deded241257a9c787698682cd9a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037825"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="4e092-103">Tipo de recurso proxiedDomain</span><span class="sxs-lookup"><span data-stu-id="4e092-103">proxiedDomain resource type</span></span>

> <span data-ttu-id="4e092-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4e092-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e092-105">Domínio com proxy</span><span class="sxs-lookup"><span data-stu-id="4e092-105">Proxied Domain</span></span>

## <a name="properties"></a><span data-ttu-id="4e092-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4e092-106">Properties</span></span>
|<span data-ttu-id="4e092-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4e092-107">Property</span></span>|<span data-ttu-id="4e092-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="4e092-108">Type</span></span>|<span data-ttu-id="4e092-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="4e092-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e092-110">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="4e092-110">ipAddressOrFQDN</span></span>|<span data-ttu-id="4e092-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4e092-111">String</span></span>|<span data-ttu-id="4e092-112">O endereço IP ou FQDN</span><span class="sxs-lookup"><span data-stu-id="4e092-112">The IP address or FQDN</span></span>|
|<span data-ttu-id="4e092-113">proxy</span><span class="sxs-lookup"><span data-stu-id="4e092-113">proxy</span></span>|<span data-ttu-id="4e092-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4e092-114">String</span></span>|<span data-ttu-id="4e092-115">IP ou FQDN do proxy</span><span class="sxs-lookup"><span data-stu-id="4e092-115">Proxy IP or FQDN</span></span>|

## <a name="relationships"></a><span data-ttu-id="4e092-116">Relações</span><span class="sxs-lookup"><span data-stu-id="4e092-116">Relationships</span></span>
<span data-ttu-id="4e092-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4e092-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4e092-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4e092-118">JSON Representation</span></span>
<span data-ttu-id="4e092-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4e092-119">Here is a JSON representation of the resource.</span></span>
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



