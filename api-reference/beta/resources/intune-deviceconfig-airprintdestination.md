---
title: tipo de recurso airPrintDestination
description: Representa um destino de impressão.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c8e359e5df1ae55fdc50c42d98c2c5f44f8ea7dc
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36334938"
---
# <a name="airprintdestination-resource-type"></a><span data-ttu-id="fc073-103">tipo de recurso airPrintDestination</span><span class="sxs-lookup"><span data-stu-id="fc073-103">airPrintDestination resource type</span></span>

> <span data-ttu-id="fc073-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fc073-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fc073-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fc073-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc073-106">Representa um destino de impressão.</span><span class="sxs-lookup"><span data-stu-id="fc073-106">Represents an AirPrint destination.</span></span>

## <a name="properties"></a><span data-ttu-id="fc073-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fc073-107">Properties</span></span>
|<span data-ttu-id="fc073-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fc073-108">Property</span></span>|<span data-ttu-id="fc073-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="fc073-109">Type</span></span>|<span data-ttu-id="fc073-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc073-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc073-111">ipAddress</span><span class="sxs-lookup"><span data-stu-id="fc073-111">ipAddress</span></span>|<span data-ttu-id="fc073-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fc073-112">String</span></span>|<span data-ttu-id="fc073-113">O endereço IP do destino de impressão.</span><span class="sxs-lookup"><span data-stu-id="fc073-113">The IP Address of the AirPrint destination.</span></span>|
|<span data-ttu-id="fc073-114">resourcePath</span><span class="sxs-lookup"><span data-stu-id="fc073-114">resourcePath</span></span>|<span data-ttu-id="fc073-115">String</span><span class="sxs-lookup"><span data-stu-id="fc073-115">String</span></span>|<span data-ttu-id="fc073-116">O caminho do recurso associado à impressora.</span><span class="sxs-lookup"><span data-stu-id="fc073-116">The Resource Path associated with the printer.</span></span> <span data-ttu-id="fc073-117">Isso corresponde ao parâmetro RP do registro Bonjour _ipps. TCP.</span><span class="sxs-lookup"><span data-stu-id="fc073-117">This corresponds to the rp parameter of the _ipps.tcp Bonjour record.</span></span> <span data-ttu-id="fc073-118">Por exemplo: impressoras/Canon_MG5300_series, impressoras/Xerox_Phaser_7600, IPP/imprimir, Epson_IPP_Printer.</span><span class="sxs-lookup"><span data-stu-id="fc073-118">For example: printers/Canon_MG5300_series, printers/Xerox_Phaser_7600, ipp/print, Epson_IPP_Printer.</span></span>|
|<span data-ttu-id="fc073-119">propor</span><span class="sxs-lookup"><span data-stu-id="fc073-119">port</span></span>|<span data-ttu-id="fc073-120">Int32</span><span class="sxs-lookup"><span data-stu-id="fc073-120">Int32</span></span>|<span data-ttu-id="fc073-121">A porta de escuta do destino de impressão.</span><span class="sxs-lookup"><span data-stu-id="fc073-121">The listening port of the AirPrint destination.</span></span> <span data-ttu-id="fc073-122">Se essa chave não for especificada, a impressão de impressa usará a porta padrão.</span><span class="sxs-lookup"><span data-stu-id="fc073-122">If this key is not specified AirPrint will use the default port.</span></span> <span data-ttu-id="fc073-123">Disponível no iOS 11,0 e posterior.</span><span class="sxs-lookup"><span data-stu-id="fc073-123">Available in iOS 11.0 and later.</span></span>|
|<span data-ttu-id="fc073-124">forceTls</span><span class="sxs-lookup"><span data-stu-id="fc073-124">forceTls</span></span>|<span data-ttu-id="fc073-125">Booliano</span><span class="sxs-lookup"><span data-stu-id="fc073-125">Boolean</span></span>|<span data-ttu-id="fc073-126">Se as conexões de impressão de verdade forem protegidas por TLS (Transport Layer Security).</span><span class="sxs-lookup"><span data-stu-id="fc073-126">If true AirPrint connections are secured by Transport Layer Security (TLS).</span></span> <span data-ttu-id="fc073-127">O padrão é false.</span><span class="sxs-lookup"><span data-stu-id="fc073-127">Default is false.</span></span> <span data-ttu-id="fc073-128">Disponível no iOS 11,0 e posterior.</span><span class="sxs-lookup"><span data-stu-id="fc073-128">Available in iOS 11.0 and later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fc073-129">Relações</span><span class="sxs-lookup"><span data-stu-id="fc073-129">Relationships</span></span>
<span data-ttu-id="fc073-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fc073-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fc073-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fc073-131">JSON Representation</span></span>
<span data-ttu-id="fc073-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fc073-132">Here is a JSON representation of the resource.</span></span>
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



