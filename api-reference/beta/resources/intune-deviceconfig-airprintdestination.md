---
title: tipo de recurso de airPrintDestination
description: Representa um destino AirPrint.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ede4f580557e75d206e0b429069acb13f81bcc5f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962510"
---
# <a name="airprintdestination-resource-type"></a><span data-ttu-id="1ccd0-103">tipo de recurso de airPrintDestination</span><span class="sxs-lookup"><span data-stu-id="1ccd0-103">airPrintDestination resource type</span></span>

> <span data-ttu-id="1ccd0-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1ccd0-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1ccd0-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1ccd0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1ccd0-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1ccd0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1ccd0-107">Representa um destino AirPrint.</span><span class="sxs-lookup"><span data-stu-id="1ccd0-107">Represents an AirPrint destination.</span></span>
## <a name="properties"></a><span data-ttu-id="1ccd0-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1ccd0-108">Properties</span></span>
|<span data-ttu-id="1ccd0-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1ccd0-109">Property</span></span>|<span data-ttu-id="1ccd0-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="1ccd0-110">Type</span></span>|<span data-ttu-id="1ccd0-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1ccd0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ccd0-112">ipAddress</span><span class="sxs-lookup"><span data-stu-id="1ccd0-112">ipAddress</span></span>|<span data-ttu-id="1ccd0-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1ccd0-113">String</span></span>|<span data-ttu-id="1ccd0-114">O endereço IP de destino AirPrint.</span><span class="sxs-lookup"><span data-stu-id="1ccd0-114">The IP Address of the AirPrint destination.</span></span>|
|<span data-ttu-id="1ccd0-115">resourcePath</span><span class="sxs-lookup"><span data-stu-id="1ccd0-115">resourcePath</span></span>|<span data-ttu-id="1ccd0-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1ccd0-116">String</span></span>|<span data-ttu-id="1ccd0-117">O caminho do recurso associado à impressora.</span><span class="sxs-lookup"><span data-stu-id="1ccd0-117">The Resource Path associated with the printer.</span></span> <span data-ttu-id="1ccd0-118">Isso corresponde ao parâmetro rp do registro Bonjour _ipps.tcp.</span><span class="sxs-lookup"><span data-stu-id="1ccd0-118">This corresponds to the rp parameter of the _ipps.tcp Bonjour record.</span></span> <span data-ttu-id="1ccd0-119">Por exemplo: impressoras/Canon_MG5300_series, impressoras/Xerox_Phaser_7600, ipp/impressão, Epson_IPP_Printer.</span><span class="sxs-lookup"><span data-stu-id="1ccd0-119">For example: printers/Canon_MG5300_series, printers/Xerox_Phaser_7600, ipp/print, Epson_IPP_Printer.</span></span>|
|<span data-ttu-id="1ccd0-120">porta</span><span class="sxs-lookup"><span data-stu-id="1ccd0-120">port</span></span>|<span data-ttu-id="1ccd0-121">Int32</span><span class="sxs-lookup"><span data-stu-id="1ccd0-121">Int32</span></span>|<span data-ttu-id="1ccd0-122">A porta de escuta do destino AirPrint.</span><span class="sxs-lookup"><span data-stu-id="1ccd0-122">The listening port of the AirPrint destination.</span></span> <span data-ttu-id="1ccd0-123">Se essa chave não for especificado, AirPrint usará a porta padrão.</span><span class="sxs-lookup"><span data-stu-id="1ccd0-123">If this key is not specified AirPrint will use the default port.</span></span> <span data-ttu-id="1ccd0-124">Disponível no iOS 11.0 e versões posteriores.</span><span class="sxs-lookup"><span data-stu-id="1ccd0-124">Available in iOS 11.0 and later.</span></span>|
|<span data-ttu-id="1ccd0-125">forceTls</span><span class="sxs-lookup"><span data-stu-id="1ccd0-125">forceTls</span></span>|<span data-ttu-id="1ccd0-126">Booliano</span><span class="sxs-lookup"><span data-stu-id="1ccd0-126">Boolean</span></span>|<span data-ttu-id="1ccd0-127">Se true conexões de AirPrint são protegidas pela segurança de camada de transporte (TLS).</span><span class="sxs-lookup"><span data-stu-id="1ccd0-127">If true AirPrint connections are secured by Transport Layer Security (TLS).</span></span> <span data-ttu-id="1ccd0-128">O padrão é false.</span><span class="sxs-lookup"><span data-stu-id="1ccd0-128">Default is false.</span></span> <span data-ttu-id="1ccd0-129">Disponível no iOS 11.0 e versões posteriores.</span><span class="sxs-lookup"><span data-stu-id="1ccd0-129">Available in iOS 11.0 and later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1ccd0-130">Relações</span><span class="sxs-lookup"><span data-stu-id="1ccd0-130">Relationships</span></span>
<span data-ttu-id="1ccd0-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1ccd0-131">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1ccd0-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1ccd0-132">JSON Representation</span></span>
<span data-ttu-id="1ccd0-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1ccd0-133">Here is a JSON representation of the resource.</span></span>
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





