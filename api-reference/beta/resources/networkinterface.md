---
title: tipo de recurso networkInterface
description: Representa uma placa de interface de rede (NIC) associada a esse host.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: d7b712c50d8cc19951f583cb8c9af7e185dba7ad
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48029159"
---
# <a name="networkinterface-resource-type"></a><span data-ttu-id="11161-103">tipo de recurso networkInterface</span><span class="sxs-lookup"><span data-stu-id="11161-103">networkInterface resource type</span></span>

<span data-ttu-id="11161-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11161-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="11161-105">Representa uma placa de interface de rede (NIC) associada a esse host.</span><span class="sxs-lookup"><span data-stu-id="11161-105">Represents a Network Interface Card (NIC) associated with this host.</span></span>

## <a name="properties"></a><span data-ttu-id="11161-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="11161-106">Properties</span></span>

| <span data-ttu-id="11161-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="11161-107">Property</span></span>   | <span data-ttu-id="11161-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="11161-108">Type</span></span> |<span data-ttu-id="11161-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="11161-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="11161-110">description</span><span class="sxs-lookup"><span data-stu-id="11161-110">description</span></span>|<span data-ttu-id="11161-111">String</span><span class="sxs-lookup"><span data-stu-id="11161-111">String</span></span>|<span data-ttu-id="11161-112">Descrição da NIC (por exemplo, adaptador Ethernet, conexão de área local do adaptador de LAN sem fio \* < # >, etc.).</span><span class="sxs-lookup"><span data-stu-id="11161-112">Description of the NIC (e.g. Ethernet adapter, Wireless LAN adapter Local Area Connection \*<#>, etc.).</span></span>|
|<span data-ttu-id="11161-113">ipV4Address</span><span class="sxs-lookup"><span data-stu-id="11161-113">ipV4Address</span></span>|<span data-ttu-id="11161-114">String</span><span class="sxs-lookup"><span data-stu-id="11161-114">String</span></span>|<span data-ttu-id="11161-115">Último endereço IPv4 associado a esta NIC.</span><span class="sxs-lookup"><span data-stu-id="11161-115">Last IPv4 address associated with this NIC.</span></span>|
|<span data-ttu-id="11161-116">ipV6Address</span><span class="sxs-lookup"><span data-stu-id="11161-116">ipV6Address</span></span>|<span data-ttu-id="11161-117">String</span><span class="sxs-lookup"><span data-stu-id="11161-117">String</span></span>|<span data-ttu-id="11161-118">Último endereço IPv6 público (aka global) associado a esta NIC.</span><span class="sxs-lookup"><span data-stu-id="11161-118">Last Public (aka global) IPv6 address associated with this NIC.</span></span>|
|<span data-ttu-id="11161-119">localIpV6Address</span><span class="sxs-lookup"><span data-stu-id="11161-119">localIpV6Address</span></span>|<span data-ttu-id="11161-120">String</span><span class="sxs-lookup"><span data-stu-id="11161-120">String</span></span>|<span data-ttu-id="11161-121">Último endereço IPv6 local (link-local ou site-local) associado a esta NIC.</span><span class="sxs-lookup"><span data-stu-id="11161-121">Last local (link-local or site-local) IPv6 address associated with this NIC.</span></span>|
|<span data-ttu-id="11161-122">macAddress</span><span class="sxs-lookup"><span data-stu-id="11161-122">macAddress</span></span>|<span data-ttu-id="11161-123">String</span><span class="sxs-lookup"><span data-stu-id="11161-123">String</span></span>|<span data-ttu-id="11161-124">Endereço MAC da NIC neste host.</span><span class="sxs-lookup"><span data-stu-id="11161-124">MAC address of the NIC on this host.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="11161-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="11161-125">JSON representation</span></span>

<span data-ttu-id="11161-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="11161-126">The following is a JSON representation of the resource.</span></span>

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


