---
title: tipo de recurso networkInterface
description: Representa uma placa de Interface de rede (NIC) associado a este host.
localization_priority: Normal
ms.openlocfilehash: 92ea26b76de8fa6ffbcdcf0bc64b85a08d0f51af
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823300"
---
# <a name="networkinterface-resource-type"></a><span data-ttu-id="1b75f-103">tipo de recurso networkInterface</span><span class="sxs-lookup"><span data-stu-id="1b75f-103">networkInterface resource type</span></span>

<span data-ttu-id="1b75f-104">Representa uma placa de Interface de rede (NIC) associado a este host.</span><span class="sxs-lookup"><span data-stu-id="1b75f-104">Represents a Network Interface Card (NIC) associated with this host.</span></span>

## <a name="properties"></a><span data-ttu-id="1b75f-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1b75f-105">Properties</span></span>

| <span data-ttu-id="1b75f-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1b75f-106">Property</span></span>   | <span data-ttu-id="1b75f-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="1b75f-107">Type</span></span> |<span data-ttu-id="1b75f-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b75f-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1b75f-109">description</span><span class="sxs-lookup"><span data-stu-id="1b75f-109">description</span></span>|<span data-ttu-id="1b75f-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1b75f-110">String</span></span>|<span data-ttu-id="1b75f-111">Descrição do NIC (adaptador de Ethernet por exemplo, Conexão de área Local de adaptador de LAN sem fio \* <> #, etc.).</span><span class="sxs-lookup"><span data-stu-id="1b75f-111">Description of the NIC (e.g. Ethernet adapter, Wireless LAN adapter Local Area Connection \*<#>, etc.).</span></span>|
|<span data-ttu-id="1b75f-112">ipV4Address</span><span class="sxs-lookup"><span data-stu-id="1b75f-112">ipV4Address</span></span>|<span data-ttu-id="1b75f-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1b75f-113">String</span></span>|<span data-ttu-id="1b75f-114">Último endereço IPv4 associado a este NIC.</span><span class="sxs-lookup"><span data-stu-id="1b75f-114">Last IPv4 address associated with this NIC.</span></span>|
|<span data-ttu-id="1b75f-115">ipV6Address</span><span class="sxs-lookup"><span data-stu-id="1b75f-115">ipV6Address</span></span>|<span data-ttu-id="1b75f-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1b75f-116">String</span></span>|<span data-ttu-id="1b75f-117">Última (também conhecido como global) endereço IPv6 público associado a este NIC.</span><span class="sxs-lookup"><span data-stu-id="1b75f-117">Last Public (aka global) IPv6 address associated with this NIC.</span></span>|
|<span data-ttu-id="1b75f-118">localIpV6Address</span><span class="sxs-lookup"><span data-stu-id="1b75f-118">localIpV6Address</span></span>|<span data-ttu-id="1b75f-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1b75f-119">String</span></span>|<span data-ttu-id="1b75f-120">Últimos local endereço IPv6 (conexão local ou de site local) associado a este NIC.</span><span class="sxs-lookup"><span data-stu-id="1b75f-120">Last local (link-local or site-local) IPv6 address associated with this NIC.</span></span>|
|<span data-ttu-id="1b75f-121">macAddress</span><span class="sxs-lookup"><span data-stu-id="1b75f-121">macAddress</span></span>|<span data-ttu-id="1b75f-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1b75f-122">String</span></span>|<span data-ttu-id="1b75f-123">Endereço MAC da NIC nesse host.</span><span class="sxs-lookup"><span data-stu-id="1b75f-123">MAC address of the NIC on this host.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1b75f-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1b75f-124">JSON representation</span></span>

<span data-ttu-id="1b75f-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1b75f-125">The following is a JSON representation of the resource.</span></span>

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
