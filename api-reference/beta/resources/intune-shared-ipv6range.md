---
title: Tipo de recurso iPv6Range
description: Descreve o recurso de iPv6Range da Microsoft Graph API para Intune, que oferece suporte a vários fluxos de trabalho.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 35b0401d3557a6afc84a27a2f47d35e17a3229a9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396347"
---
# <a name="ipv6range-resource-type"></a><span data-ttu-id="7fbfd-103">Tipo de recurso iPv6Range</span><span class="sxs-lookup"><span data-stu-id="7fbfd-103">iPv6Range resource type</span></span>

> <span data-ttu-id="7fbfd-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7fbfd-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7fbfd-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7fbfd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7fbfd-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="7fbfd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7fbfd-107">Intervalo de IPV6</span><span class="sxs-lookup"><span data-stu-id="7fbfd-107">IP V6 range</span></span>

<span data-ttu-id="7fbfd-108">Herda de [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="7fbfd-108">Inherits from [ipRange](../resources/intune-shared-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7fbfd-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7fbfd-109">Properties</span></span>
|<span data-ttu-id="7fbfd-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7fbfd-110">Property</span></span>|<span data-ttu-id="7fbfd-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="7fbfd-111">Type</span></span>|<span data-ttu-id="7fbfd-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="7fbfd-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7fbfd-113">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="7fbfd-113">lowerAddress</span></span>|<span data-ttu-id="7fbfd-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7fbfd-114">String</span></span>|<span data-ttu-id="7fbfd-115">Endereço IP de número mais baixo</span><span class="sxs-lookup"><span data-stu-id="7fbfd-115">Lower IP Address</span></span>|
|<span data-ttu-id="7fbfd-116">upperAddress</span><span class="sxs-lookup"><span data-stu-id="7fbfd-116">upperAddress</span></span>|<span data-ttu-id="7fbfd-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7fbfd-117">String</span></span>|<span data-ttu-id="7fbfd-118">Endereço IP de número mais alto</span><span class="sxs-lookup"><span data-stu-id="7fbfd-118">Upper IP Address</span></span>|

## <a name="relationships"></a><span data-ttu-id="7fbfd-119">Relações</span><span class="sxs-lookup"><span data-stu-id="7fbfd-119">Relationships</span></span>
<span data-ttu-id="7fbfd-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7fbfd-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7fbfd-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7fbfd-121">JSON Representation</span></span>
<span data-ttu-id="7fbfd-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7fbfd-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iPv6Range"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iPv6Range",
  "lowerAddress": "String",
  "upperAddress": "String"
}
```



