---
title: tipo de recurso airPrintDestination
description: Representa um destino de impressão.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3218a40ee1a735cef585866e1ca0c9f80ad95671
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31779969"
---
# <a name="airprintdestination-resource-type"></a><span data-ttu-id="f68e4-103">tipo de recurso airPrintDestination</span><span class="sxs-lookup"><span data-stu-id="f68e4-103">airPrintDestination resource type</span></span>

> <span data-ttu-id="f68e4-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f68e4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f68e4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f68e4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f68e4-106">Representa um destino de impressão.</span><span class="sxs-lookup"><span data-stu-id="f68e4-106">Represents an AirPrint destination.</span></span>

## <a name="properties"></a><span data-ttu-id="f68e4-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f68e4-107">Properties</span></span>
|<span data-ttu-id="f68e4-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f68e4-108">Property</span></span>|<span data-ttu-id="f68e4-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="f68e4-109">Type</span></span>|<span data-ttu-id="f68e4-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f68e4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f68e4-111">ipAddress</span><span class="sxs-lookup"><span data-stu-id="f68e4-111">ipAddress</span></span>|<span data-ttu-id="f68e4-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f68e4-112">String</span></span>|<span data-ttu-id="f68e4-113">O endereço IP do destino de impressão.</span><span class="sxs-lookup"><span data-stu-id="f68e4-113">The IP Address of the AirPrint destination.</span></span>|
|<span data-ttu-id="f68e4-114">resourcePath</span><span class="sxs-lookup"><span data-stu-id="f68e4-114">resourcePath</span></span>|<span data-ttu-id="f68e4-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f68e4-115">String</span></span>|<span data-ttu-id="f68e4-116">O caminho do recurso associado à impressora.</span><span class="sxs-lookup"><span data-stu-id="f68e4-116">The Resource Path associated with the printer.</span></span> <span data-ttu-id="f68e4-117">Isso corresponde ao parâmetro RP do registro Bonjour _ipps. TCP.</span><span class="sxs-lookup"><span data-stu-id="f68e4-117">This corresponds to the rp parameter of the _ipps.tcp Bonjour record.</span></span> <span data-ttu-id="f68e4-118">Por exemplo: impressoras/Canon_MG5300_series, impressoras/Xerox_Phaser_7600, IPP/imprimir, Epson_IPP_Printer.</span><span class="sxs-lookup"><span data-stu-id="f68e4-118">For example: printers/Canon_MG5300_series, printers/Xerox_Phaser_7600, ipp/print, Epson_IPP_Printer.</span></span>|
|<span data-ttu-id="f68e4-119">propor</span><span class="sxs-lookup"><span data-stu-id="f68e4-119">port</span></span>|<span data-ttu-id="f68e4-120">Int32</span><span class="sxs-lookup"><span data-stu-id="f68e4-120">Int32</span></span>|<span data-ttu-id="f68e4-121">A porta de escuta do destino de impressão.</span><span class="sxs-lookup"><span data-stu-id="f68e4-121">The listening port of the AirPrint destination.</span></span> <span data-ttu-id="f68e4-122">Se essa chave não for especificada, a impressão de impressa usará a porta padrão.</span><span class="sxs-lookup"><span data-stu-id="f68e4-122">If this key is not specified AirPrint will use the default port.</span></span> <span data-ttu-id="f68e4-123">Disponível no iOS 11,0 e posterior.</span><span class="sxs-lookup"><span data-stu-id="f68e4-123">Available in iOS 11.0 and later.</span></span>|
|<span data-ttu-id="f68e4-124">forceTls</span><span class="sxs-lookup"><span data-stu-id="f68e4-124">forceTls</span></span>|<span data-ttu-id="f68e4-125">Booliano</span><span class="sxs-lookup"><span data-stu-id="f68e4-125">Boolean</span></span>|<span data-ttu-id="f68e4-126">Se as conexões de impressão de verdade forem protegidas por TLS (Transport Layer Security).</span><span class="sxs-lookup"><span data-stu-id="f68e4-126">If true AirPrint connections are secured by Transport Layer Security (TLS).</span></span> <span data-ttu-id="f68e4-127">O padrão é false.</span><span class="sxs-lookup"><span data-stu-id="f68e4-127">Default is false.</span></span> <span data-ttu-id="f68e4-128">Disponível no iOS 11,0 e posterior.</span><span class="sxs-lookup"><span data-stu-id="f68e4-128">Available in iOS 11.0 and later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f68e4-129">Relações</span><span class="sxs-lookup"><span data-stu-id="f68e4-129">Relationships</span></span>
<span data-ttu-id="f68e4-130">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="f68e4-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f68e4-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f68e4-131">JSON Representation</span></span>
<span data-ttu-id="f68e4-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f68e4-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.airPrintDestination"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.airPrintDestination",
  "ipAddress": "String",
  "resourcePath": "String",
  "port": 1024,
  "forceTls": true
}
```





