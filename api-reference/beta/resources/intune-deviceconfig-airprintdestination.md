---
title: tipo de recurso airPrintDestination
description: Representa um destino de impressão.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 99693cbdfa77895e0116ac5228fdf58d95afeacb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42487358"
---
# <a name="airprintdestination-resource-type"></a><span data-ttu-id="e764b-103">tipo de recurso airPrintDestination</span><span class="sxs-lookup"><span data-stu-id="e764b-103">airPrintDestination resource type</span></span>

<span data-ttu-id="e764b-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e764b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e764b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e764b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e764b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e764b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e764b-107">Representa um destino de impressão.</span><span class="sxs-lookup"><span data-stu-id="e764b-107">Represents an AirPrint destination.</span></span>

## <a name="properties"></a><span data-ttu-id="e764b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e764b-108">Properties</span></span>
|<span data-ttu-id="e764b-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e764b-109">Property</span></span>|<span data-ttu-id="e764b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="e764b-110">Type</span></span>|<span data-ttu-id="e764b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e764b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e764b-112">ipAddress</span><span class="sxs-lookup"><span data-stu-id="e764b-112">ipAddress</span></span>|<span data-ttu-id="e764b-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e764b-113">String</span></span>|<span data-ttu-id="e764b-114">O endereço IP do destino de impressão.</span><span class="sxs-lookup"><span data-stu-id="e764b-114">The IP Address of the AirPrint destination.</span></span>|
|<span data-ttu-id="e764b-115">resourcePath</span><span class="sxs-lookup"><span data-stu-id="e764b-115">resourcePath</span></span>|<span data-ttu-id="e764b-116">String</span><span class="sxs-lookup"><span data-stu-id="e764b-116">String</span></span>|<span data-ttu-id="e764b-117">O caminho do recurso associado à impressora.</span><span class="sxs-lookup"><span data-stu-id="e764b-117">The Resource Path associated with the printer.</span></span> <span data-ttu-id="e764b-118">Isso corresponde ao parâmetro RP do registro _ipps. TCP Bonjour.</span><span class="sxs-lookup"><span data-stu-id="e764b-118">This corresponds to the rp parameter of the _ipps.tcp Bonjour record.</span></span> <span data-ttu-id="e764b-119">Por exemplo: impressoras/Canon_MG5300_series, impressoras/Xerox_Phaser_7600, IPP/imprimir Epson_IPP_Printer.</span><span class="sxs-lookup"><span data-stu-id="e764b-119">For example: printers/Canon_MG5300_series, printers/Xerox_Phaser_7600, ipp/print, Epson_IPP_Printer.</span></span>|
|<span data-ttu-id="e764b-120">propor</span><span class="sxs-lookup"><span data-stu-id="e764b-120">port</span></span>|<span data-ttu-id="e764b-121">Int32</span><span class="sxs-lookup"><span data-stu-id="e764b-121">Int32</span></span>|<span data-ttu-id="e764b-122">A porta de escuta do destino de impressão.</span><span class="sxs-lookup"><span data-stu-id="e764b-122">The listening port of the AirPrint destination.</span></span> <span data-ttu-id="e764b-123">Se essa chave não for especificada, a impressão de impressa usará a porta padrão.</span><span class="sxs-lookup"><span data-stu-id="e764b-123">If this key is not specified AirPrint will use the default port.</span></span> <span data-ttu-id="e764b-124">Disponível no iOS 11,0 e posterior.</span><span class="sxs-lookup"><span data-stu-id="e764b-124">Available in iOS 11.0 and later.</span></span>|
|<span data-ttu-id="e764b-125">forceTls</span><span class="sxs-lookup"><span data-stu-id="e764b-125">forceTls</span></span>|<span data-ttu-id="e764b-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="e764b-126">Boolean</span></span>|<span data-ttu-id="e764b-127">Se as conexões de impressão de verdade forem protegidas por TLS (Transport Layer Security).</span><span class="sxs-lookup"><span data-stu-id="e764b-127">If true AirPrint connections are secured by Transport Layer Security (TLS).</span></span> <span data-ttu-id="e764b-128">O padrão é false.</span><span class="sxs-lookup"><span data-stu-id="e764b-128">Default is false.</span></span> <span data-ttu-id="e764b-129">Disponível no iOS 11,0 e posterior.</span><span class="sxs-lookup"><span data-stu-id="e764b-129">Available in iOS 11.0 and later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e764b-130">Relações</span><span class="sxs-lookup"><span data-stu-id="e764b-130">Relationships</span></span>
<span data-ttu-id="e764b-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e764b-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e764b-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e764b-132">JSON Representation</span></span>
<span data-ttu-id="e764b-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e764b-133">Here is a JSON representation of the resource.</span></span>
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



