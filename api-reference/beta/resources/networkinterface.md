---
title: tipo de recurso networkInterface
description: Representa uma placa de interface de rede (NIC) associada a esse host.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 4f19c2fae729e437ec2d9e91a0c6be5694a85214
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812783"
---
# <a name="networkinterface-resource-type"></a><span data-ttu-id="a3223-103">tipo de recurso networkInterface</span><span class="sxs-lookup"><span data-stu-id="a3223-103">networkInterface resource type</span></span>

<span data-ttu-id="a3223-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3223-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a3223-105">Representa uma placa de interface de rede (NIC) associada a esse host.</span><span class="sxs-lookup"><span data-stu-id="a3223-105">Represents a Network Interface Card (NIC) associated with this host.</span></span>

## <a name="properties"></a><span data-ttu-id="a3223-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a3223-106">Properties</span></span>

| <span data-ttu-id="a3223-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a3223-107">Property</span></span>   | <span data-ttu-id="a3223-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="a3223-108">Type</span></span> |<span data-ttu-id="a3223-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a3223-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a3223-110">description</span><span class="sxs-lookup"><span data-stu-id="a3223-110">description</span></span>|<span data-ttu-id="a3223-111">String</span><span class="sxs-lookup"><span data-stu-id="a3223-111">String</span></span>|<span data-ttu-id="a3223-112">Descrição da NIC (por exemplo, adaptador Ethernet, conexão de área local do adaptador de LAN sem fio \* < # >, etc.).</span><span class="sxs-lookup"><span data-stu-id="a3223-112">Description of the NIC (e.g. Ethernet adapter, Wireless LAN adapter Local Area Connection \*<#>, etc.).</span></span>|
|<span data-ttu-id="a3223-113">ipV4Address</span><span class="sxs-lookup"><span data-stu-id="a3223-113">ipV4Address</span></span>|<span data-ttu-id="a3223-114">String</span><span class="sxs-lookup"><span data-stu-id="a3223-114">String</span></span>|<span data-ttu-id="a3223-115">Último endereço IPv4 associado a esta NIC.</span><span class="sxs-lookup"><span data-stu-id="a3223-115">Last IPv4 address associated with this NIC.</span></span>|
|<span data-ttu-id="a3223-116">ipV6Address</span><span class="sxs-lookup"><span data-stu-id="a3223-116">ipV6Address</span></span>|<span data-ttu-id="a3223-117">String</span><span class="sxs-lookup"><span data-stu-id="a3223-117">String</span></span>|<span data-ttu-id="a3223-118">Último endereço IPv6 público (aka global) associado a esta NIC.</span><span class="sxs-lookup"><span data-stu-id="a3223-118">Last Public (aka global) IPv6 address associated with this NIC.</span></span>|
|<span data-ttu-id="a3223-119">localIpV6Address</span><span class="sxs-lookup"><span data-stu-id="a3223-119">localIpV6Address</span></span>|<span data-ttu-id="a3223-120">String</span><span class="sxs-lookup"><span data-stu-id="a3223-120">String</span></span>|<span data-ttu-id="a3223-121">Último endereço IPv6 local (link-local ou site-local) associado a esta NIC.</span><span class="sxs-lookup"><span data-stu-id="a3223-121">Last local (link-local or site-local) IPv6 address associated with this NIC.</span></span>|
|<span data-ttu-id="a3223-122">macAddress</span><span class="sxs-lookup"><span data-stu-id="a3223-122">macAddress</span></span>|<span data-ttu-id="a3223-123">String</span><span class="sxs-lookup"><span data-stu-id="a3223-123">String</span></span>|<span data-ttu-id="a3223-124">Endereço MAC da NIC neste host.</span><span class="sxs-lookup"><span data-stu-id="a3223-124">MAC address of the NIC on this host.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a3223-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a3223-125">JSON representation</span></span>

<span data-ttu-id="a3223-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a3223-126">The following is a JSON representation of the resource.</span></span>

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
