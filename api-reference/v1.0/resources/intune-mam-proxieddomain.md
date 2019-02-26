---
title: Tipo de recurso proxiedDomain
description: Domínio com proxy
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b28271308f5256d034de3b4704353aa0471aeb29
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30264040"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="1e7ce-103">Tipo de recurso proxiedDomain</span><span class="sxs-lookup"><span data-stu-id="1e7ce-103">proxiedDomain resource type</span></span>

> <span data-ttu-id="1e7ce-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1e7ce-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1e7ce-105">Domínio com proxy</span><span class="sxs-lookup"><span data-stu-id="1e7ce-105">Proxied Domain</span></span>

## <a name="properties"></a><span data-ttu-id="1e7ce-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1e7ce-106">Properties</span></span>
|<span data-ttu-id="1e7ce-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1e7ce-107">Property</span></span>|<span data-ttu-id="1e7ce-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="1e7ce-108">Type</span></span>|<span data-ttu-id="1e7ce-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e7ce-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e7ce-110">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="1e7ce-110">ipAddressOrFQDN</span></span>|<span data-ttu-id="1e7ce-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e7ce-111">String</span></span>|<span data-ttu-id="1e7ce-112">O endereço IP ou FQDN</span><span class="sxs-lookup"><span data-stu-id="1e7ce-112">The IP address or FQDN</span></span>|
|<span data-ttu-id="1e7ce-113">proxy</span><span class="sxs-lookup"><span data-stu-id="1e7ce-113">proxy</span></span>|<span data-ttu-id="1e7ce-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e7ce-114">String</span></span>|<span data-ttu-id="1e7ce-115">IP ou FQDN do proxy</span><span class="sxs-lookup"><span data-stu-id="1e7ce-115">Proxy IP or FQDN</span></span>|

## <a name="relationships"></a><span data-ttu-id="1e7ce-116">Relações</span><span class="sxs-lookup"><span data-stu-id="1e7ce-116">Relationships</span></span>
<span data-ttu-id="1e7ce-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1e7ce-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1e7ce-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1e7ce-118">JSON Representation</span></span>
<span data-ttu-id="1e7ce-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1e7ce-119">Here is a JSON representation of the resource.</span></span>
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



