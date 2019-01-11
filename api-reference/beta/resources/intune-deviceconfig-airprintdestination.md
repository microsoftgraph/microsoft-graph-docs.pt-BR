---
title: tipo de recurso de airPrintDestination
description: Representa um destino AirPrint.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 6d1548737956d35d42fc077afe92de1885a54581
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27878586"
---
# <a name="airprintdestination-resource-type"></a><span data-ttu-id="13cde-103">tipo de recurso de airPrintDestination</span><span class="sxs-lookup"><span data-stu-id="13cde-103">airPrintDestination resource type</span></span>

> <span data-ttu-id="13cde-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="13cde-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="13cde-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="13cde-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="13cde-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="13cde-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="13cde-107">Representa um destino AirPrint.</span><span class="sxs-lookup"><span data-stu-id="13cde-107">Represents an AirPrint destination.</span></span>
## <a name="properties"></a><span data-ttu-id="13cde-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="13cde-108">Properties</span></span>
|<span data-ttu-id="13cde-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="13cde-109">Property</span></span>|<span data-ttu-id="13cde-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="13cde-110">Type</span></span>|<span data-ttu-id="13cde-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="13cde-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13cde-112">ipAddress</span><span class="sxs-lookup"><span data-stu-id="13cde-112">ipAddress</span></span>|<span data-ttu-id="13cde-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="13cde-113">String</span></span>|<span data-ttu-id="13cde-114">O endereço IP de destino AirPrint.</span><span class="sxs-lookup"><span data-stu-id="13cde-114">The IP Address of the AirPrint destination.</span></span>|
|<span data-ttu-id="13cde-115">resourcePath</span><span class="sxs-lookup"><span data-stu-id="13cde-115">resourcePath</span></span>|<span data-ttu-id="13cde-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="13cde-116">String</span></span>|<span data-ttu-id="13cde-117">O caminho do recurso associado à impressora.</span><span class="sxs-lookup"><span data-stu-id="13cde-117">The Resource Path associated with the printer.</span></span> <span data-ttu-id="13cde-118">Isso corresponde ao parâmetro rp do registro Bonjour _ipps.tcp.</span><span class="sxs-lookup"><span data-stu-id="13cde-118">This corresponds to the rp parameter of the _ipps.tcp Bonjour record.</span></span> <span data-ttu-id="13cde-119">Por exemplo: impressoras/Canon_MG5300_series, impressoras/Xerox_Phaser_7600, ipp/impressão, Epson_IPP_Printer.</span><span class="sxs-lookup"><span data-stu-id="13cde-119">For example: printers/Canon_MG5300_series, printers/Xerox_Phaser_7600, ipp/print, Epson_IPP_Printer.</span></span>|
|<span data-ttu-id="13cde-120">porta</span><span class="sxs-lookup"><span data-stu-id="13cde-120">port</span></span>|<span data-ttu-id="13cde-121">Int32</span><span class="sxs-lookup"><span data-stu-id="13cde-121">Int32</span></span>|<span data-ttu-id="13cde-122">A porta de escuta do destino AirPrint.</span><span class="sxs-lookup"><span data-stu-id="13cde-122">The listening port of the AirPrint destination.</span></span> <span data-ttu-id="13cde-123">Se essa chave não for especificado, AirPrint usará a porta padrão.</span><span class="sxs-lookup"><span data-stu-id="13cde-123">If this key is not specified AirPrint will use the default port.</span></span> <span data-ttu-id="13cde-124">Disponível no iOS 11.0 e versões posteriores.</span><span class="sxs-lookup"><span data-stu-id="13cde-124">Available in iOS 11.0 and later.</span></span>|
|<span data-ttu-id="13cde-125">forceTls</span><span class="sxs-lookup"><span data-stu-id="13cde-125">forceTls</span></span>|<span data-ttu-id="13cde-126">Booliano</span><span class="sxs-lookup"><span data-stu-id="13cde-126">Boolean</span></span>|<span data-ttu-id="13cde-127">Se true conexões de AirPrint são protegidas pela segurança de camada de transporte (TLS).</span><span class="sxs-lookup"><span data-stu-id="13cde-127">If true AirPrint connections are secured by Transport Layer Security (TLS).</span></span> <span data-ttu-id="13cde-128">O padrão é false.</span><span class="sxs-lookup"><span data-stu-id="13cde-128">Default is false.</span></span> <span data-ttu-id="13cde-129">Disponível no iOS 11.0 e versões posteriores.</span><span class="sxs-lookup"><span data-stu-id="13cde-129">Available in iOS 11.0 and later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="13cde-130">Relações</span><span class="sxs-lookup"><span data-stu-id="13cde-130">Relationships</span></span>
<span data-ttu-id="13cde-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="13cde-131">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="13cde-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="13cde-132">JSON Representation</span></span>
<span data-ttu-id="13cde-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="13cde-133">Here is a JSON representation of the resource.</span></span>
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





