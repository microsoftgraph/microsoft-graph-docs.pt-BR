---
title: tipo de recurso networkInterface
description: Representa uma placa de interface de rede (NIC) associada a esse host.
localization_priority: Normal
ms.openlocfilehash: 92ea26b76de8fa6ffbcdcf0bc64b85a08d0f51af
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457064"
---
# <a name="networkinterface-resource-type"></a><span data-ttu-id="c1c78-103">tipo de recurso networkInterface</span><span class="sxs-lookup"><span data-stu-id="c1c78-103">networkInterface resource type</span></span>

<span data-ttu-id="c1c78-104">Representa uma placa de interface de rede (NIC) associada a esse host.</span><span class="sxs-lookup"><span data-stu-id="c1c78-104">Represents a Network Interface Card (NIC) associated with this host.</span></span>

## <a name="properties"></a><span data-ttu-id="c1c78-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c1c78-105">Properties</span></span>

| <span data-ttu-id="c1c78-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c1c78-106">Property</span></span>   | <span data-ttu-id="c1c78-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="c1c78-107">Type</span></span> |<span data-ttu-id="c1c78-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="c1c78-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c1c78-109">description</span><span class="sxs-lookup"><span data-stu-id="c1c78-109">description</span></span>|<span data-ttu-id="c1c78-110">String</span><span class="sxs-lookup"><span data-stu-id="c1c78-110">String</span></span>|<span data-ttu-id="c1c78-111">Descrição da NIC (por exemplo, adaptador Ethernet, conexão de área local do adaptador de LAN sem fio \* < # >, etc.).</span><span class="sxs-lookup"><span data-stu-id="c1c78-111">Description of the NIC (e.g. Ethernet adapter, Wireless LAN adapter Local Area Connection \*<#>, etc.).</span></span>|
|<span data-ttu-id="c1c78-112">ipV4Address</span><span class="sxs-lookup"><span data-stu-id="c1c78-112">ipV4Address</span></span>|<span data-ttu-id="c1c78-113">String</span><span class="sxs-lookup"><span data-stu-id="c1c78-113">String</span></span>|<span data-ttu-id="c1c78-114">Último endereço IPv4 associado a esta NIC.</span><span class="sxs-lookup"><span data-stu-id="c1c78-114">Last IPv4 address associated with this NIC.</span></span>|
|<span data-ttu-id="c1c78-115">ipV6Address</span><span class="sxs-lookup"><span data-stu-id="c1c78-115">ipV6Address</span></span>|<span data-ttu-id="c1c78-116">String</span><span class="sxs-lookup"><span data-stu-id="c1c78-116">String</span></span>|<span data-ttu-id="c1c78-117">Último endereço IPv6 público (aka global) associado a esta NIC.</span><span class="sxs-lookup"><span data-stu-id="c1c78-117">Last Public (aka global) IPv6 address associated with this NIC.</span></span>|
|<span data-ttu-id="c1c78-118">localIpV6Address</span><span class="sxs-lookup"><span data-stu-id="c1c78-118">localIpV6Address</span></span>|<span data-ttu-id="c1c78-119">String</span><span class="sxs-lookup"><span data-stu-id="c1c78-119">String</span></span>|<span data-ttu-id="c1c78-120">Último endereço IPv6 local (link-local ou site-local) associado a esta NIC.</span><span class="sxs-lookup"><span data-stu-id="c1c78-120">Last local (link-local or site-local) IPv6 address associated with this NIC.</span></span>|
|<span data-ttu-id="c1c78-121">macAddress</span><span class="sxs-lookup"><span data-stu-id="c1c78-121">macAddress</span></span>|<span data-ttu-id="c1c78-122">String</span><span class="sxs-lookup"><span data-stu-id="c1c78-122">String</span></span>|<span data-ttu-id="c1c78-123">Endereço MAC da NIC neste host.</span><span class="sxs-lookup"><span data-stu-id="c1c78-123">MAC address of the NIC on this host.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c1c78-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c1c78-124">JSON representation</span></span>

<span data-ttu-id="c1c78-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c1c78-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.networkInterface"
}-->

```json
{
  "description": "String",
  "ipV4Address": "String",
  "ipV6Address": "String",
  "localIpV6Address": "String",
  "macAddress": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "networkInterface resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
