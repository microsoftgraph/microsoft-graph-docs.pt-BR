---
title: tipo de recurso de airPrintDestination
description: Representa um destino AirPrint.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3f56578427427d45a69c4c64fe9fde3cf31f8fd9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422492"
---
# <a name="airprintdestination-resource-type"></a><span data-ttu-id="4a549-103">tipo de recurso de airPrintDestination</span><span class="sxs-lookup"><span data-stu-id="4a549-103">airPrintDestination resource type</span></span>

> <span data-ttu-id="4a549-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="4a549-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4a549-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4a549-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4a549-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="4a549-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a549-107">Representa um destino AirPrint.</span><span class="sxs-lookup"><span data-stu-id="4a549-107">Represents an AirPrint destination.</span></span>

## <a name="properties"></a><span data-ttu-id="4a549-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4a549-108">Properties</span></span>
|<span data-ttu-id="4a549-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4a549-109">Property</span></span>|<span data-ttu-id="4a549-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="4a549-110">Type</span></span>|<span data-ttu-id="4a549-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a549-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a549-112">ipAddress</span><span class="sxs-lookup"><span data-stu-id="4a549-112">ipAddress</span></span>|<span data-ttu-id="4a549-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4a549-113">String</span></span>|<span data-ttu-id="4a549-114">O endereço IP de destino AirPrint.</span><span class="sxs-lookup"><span data-stu-id="4a549-114">The IP Address of the AirPrint destination.</span></span>|
|<span data-ttu-id="4a549-115">resourcePath</span><span class="sxs-lookup"><span data-stu-id="4a549-115">resourcePath</span></span>|<span data-ttu-id="4a549-116">String</span><span class="sxs-lookup"><span data-stu-id="4a549-116">String</span></span>|<span data-ttu-id="4a549-117">O caminho do recurso associado à impressora.</span><span class="sxs-lookup"><span data-stu-id="4a549-117">The Resource Path associated with the printer.</span></span> <span data-ttu-id="4a549-118">Isso corresponde ao parâmetro rp do registro Bonjour _ipps.tcp.</span><span class="sxs-lookup"><span data-stu-id="4a549-118">This corresponds to the rp parameter of the _ipps.tcp Bonjour record.</span></span> <span data-ttu-id="4a549-119">Por exemplo: impressoras/Canon_MG5300_series, impressoras/Xerox_Phaser_7600, ipp/impressão, Epson_IPP_Printer.</span><span class="sxs-lookup"><span data-stu-id="4a549-119">For example: printers/Canon_MG5300_series, printers/Xerox_Phaser_7600, ipp/print, Epson_IPP_Printer.</span></span>|
|<span data-ttu-id="4a549-120">porta</span><span class="sxs-lookup"><span data-stu-id="4a549-120">port</span></span>|<span data-ttu-id="4a549-121">Int32</span><span class="sxs-lookup"><span data-stu-id="4a549-121">Int32</span></span>|<span data-ttu-id="4a549-122">A porta de escuta do destino AirPrint.</span><span class="sxs-lookup"><span data-stu-id="4a549-122">The listening port of the AirPrint destination.</span></span> <span data-ttu-id="4a549-123">Se essa chave não for especificado, AirPrint usará a porta padrão.</span><span class="sxs-lookup"><span data-stu-id="4a549-123">If this key is not specified AirPrint will use the default port.</span></span> <span data-ttu-id="4a549-124">Disponível no iOS 11.0 e versões posteriores.</span><span class="sxs-lookup"><span data-stu-id="4a549-124">Available in iOS 11.0 and later.</span></span>|
|<span data-ttu-id="4a549-125">forceTls</span><span class="sxs-lookup"><span data-stu-id="4a549-125">forceTls</span></span>|<span data-ttu-id="4a549-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a549-126">Boolean</span></span>|<span data-ttu-id="4a549-127">Se true conexões de AirPrint são protegidas pela segurança de camada de transporte (TLS).</span><span class="sxs-lookup"><span data-stu-id="4a549-127">If true AirPrint connections are secured by Transport Layer Security (TLS).</span></span> <span data-ttu-id="4a549-128">O padrão é false.</span><span class="sxs-lookup"><span data-stu-id="4a549-128">Default is false.</span></span> <span data-ttu-id="4a549-129">Disponível no iOS 11.0 e versões posteriores.</span><span class="sxs-lookup"><span data-stu-id="4a549-129">Available in iOS 11.0 and later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4a549-130">Relações</span><span class="sxs-lookup"><span data-stu-id="4a549-130">Relationships</span></span>
<span data-ttu-id="4a549-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4a549-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4a549-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4a549-132">JSON Representation</span></span>
<span data-ttu-id="4a549-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4a549-133">Here is a JSON representation of the resource.</span></span>
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




