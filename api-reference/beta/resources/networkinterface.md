---
title: tipo de recurso networkInterface
description: Representa uma placa de interface de rede (NIC) associada a esse host.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 5fd40bec964a73579863b8222cd4c90d58991502
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522572"
---
# <a name="networkinterface-resource-type"></a><span data-ttu-id="8326f-103">tipo de recurso networkInterface</span><span class="sxs-lookup"><span data-stu-id="8326f-103">networkInterface resource type</span></span>

<span data-ttu-id="8326f-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="8326f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8326f-105">Representa uma placa de interface de rede (NIC) associada a esse host.</span><span class="sxs-lookup"><span data-stu-id="8326f-105">Represents a Network Interface Card (NIC) associated with this host.</span></span>

## <a name="properties"></a><span data-ttu-id="8326f-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8326f-106">Properties</span></span>

| <span data-ttu-id="8326f-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8326f-107">Property</span></span>   | <span data-ttu-id="8326f-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="8326f-108">Type</span></span> |<span data-ttu-id="8326f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="8326f-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8326f-110">description</span><span class="sxs-lookup"><span data-stu-id="8326f-110">description</span></span>|<span data-ttu-id="8326f-111">String</span><span class="sxs-lookup"><span data-stu-id="8326f-111">String</span></span>|<span data-ttu-id="8326f-112">Descrição da NIC (por exemplo, adaptador Ethernet, conexão de área local do adaptador de LAN sem fio \* < # >, etc.).</span><span class="sxs-lookup"><span data-stu-id="8326f-112">Description of the NIC (e.g. Ethernet adapter, Wireless LAN adapter Local Area Connection \*<#>, etc.).</span></span>|
|<span data-ttu-id="8326f-113">ipV4Address</span><span class="sxs-lookup"><span data-stu-id="8326f-113">ipV4Address</span></span>|<span data-ttu-id="8326f-114">String</span><span class="sxs-lookup"><span data-stu-id="8326f-114">String</span></span>|<span data-ttu-id="8326f-115">Último endereço IPv4 associado a esta NIC.</span><span class="sxs-lookup"><span data-stu-id="8326f-115">Last IPv4 address associated with this NIC.</span></span>|
|<span data-ttu-id="8326f-116">ipV6Address</span><span class="sxs-lookup"><span data-stu-id="8326f-116">ipV6Address</span></span>|<span data-ttu-id="8326f-117">String</span><span class="sxs-lookup"><span data-stu-id="8326f-117">String</span></span>|<span data-ttu-id="8326f-118">Último endereço IPv6 público (aka global) associado a esta NIC.</span><span class="sxs-lookup"><span data-stu-id="8326f-118">Last Public (aka global) IPv6 address associated with this NIC.</span></span>|
|<span data-ttu-id="8326f-119">localIpV6Address</span><span class="sxs-lookup"><span data-stu-id="8326f-119">localIpV6Address</span></span>|<span data-ttu-id="8326f-120">String</span><span class="sxs-lookup"><span data-stu-id="8326f-120">String</span></span>|<span data-ttu-id="8326f-121">Último endereço IPv6 local (link-local ou site-local) associado a esta NIC.</span><span class="sxs-lookup"><span data-stu-id="8326f-121">Last local (link-local or site-local) IPv6 address associated with this NIC.</span></span>|
|<span data-ttu-id="8326f-122">macAddress</span><span class="sxs-lookup"><span data-stu-id="8326f-122">macAddress</span></span>|<span data-ttu-id="8326f-123">String</span><span class="sxs-lookup"><span data-stu-id="8326f-123">String</span></span>|<span data-ttu-id="8326f-124">Endereço MAC da NIC neste host.</span><span class="sxs-lookup"><span data-stu-id="8326f-124">MAC address of the NIC on this host.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8326f-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8326f-125">JSON representation</span></span>

<span data-ttu-id="8326f-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8326f-126">The following is a JSON representation of the resource.</span></span>

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
