---
title: Tipo de recurso proxiedDomain
description: Domínio com proxy
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e437c6bf035d0f6099531fbe5ebf236d30be3a2f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42448274"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="a3d67-103">Tipo de recurso proxiedDomain</span><span class="sxs-lookup"><span data-stu-id="a3d67-103">proxiedDomain resource type</span></span>

<span data-ttu-id="a3d67-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a3d67-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a3d67-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a3d67-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3d67-106">Domínio com proxy</span><span class="sxs-lookup"><span data-stu-id="a3d67-106">Proxied Domain</span></span>

## <a name="properties"></a><span data-ttu-id="a3d67-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a3d67-107">Properties</span></span>
|<span data-ttu-id="a3d67-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a3d67-108">Property</span></span>|<span data-ttu-id="a3d67-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a3d67-109">Type</span></span>|<span data-ttu-id="a3d67-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a3d67-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3d67-111">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="a3d67-111">ipAddressOrFQDN</span></span>|<span data-ttu-id="a3d67-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a3d67-112">String</span></span>|<span data-ttu-id="a3d67-113">O endereço IP ou FQDN</span><span class="sxs-lookup"><span data-stu-id="a3d67-113">The IP address or FQDN</span></span>|
|<span data-ttu-id="a3d67-114">proxy</span><span class="sxs-lookup"><span data-stu-id="a3d67-114">proxy</span></span>|<span data-ttu-id="a3d67-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a3d67-115">String</span></span>|<span data-ttu-id="a3d67-116">IP ou FQDN do proxy</span><span class="sxs-lookup"><span data-stu-id="a3d67-116">Proxy IP or FQDN</span></span>|

## <a name="relationships"></a><span data-ttu-id="a3d67-117">Relações</span><span class="sxs-lookup"><span data-stu-id="a3d67-117">Relationships</span></span>
<span data-ttu-id="a3d67-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a3d67-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a3d67-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a3d67-119">JSON Representation</span></span>
<span data-ttu-id="a3d67-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a3d67-120">Here is a JSON representation of the resource.</span></span>
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




