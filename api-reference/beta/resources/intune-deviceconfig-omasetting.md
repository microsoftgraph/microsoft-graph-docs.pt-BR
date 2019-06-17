---
title: Tipo de recurso omaSetting
description: Configurações de OMA.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0bb5df5f786eefc1b7b7159b1643f9d3d46d8300
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34958701"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="f29e0-103">Tipo de recurso omaSetting</span><span class="sxs-lookup"><span data-stu-id="f29e0-103">omaSetting resource type</span></span>

> <span data-ttu-id="f29e0-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f29e0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f29e0-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f29e0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f29e0-106">Configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="f29e0-106">OMA Settings definition.</span></span>

## <a name="properties"></a><span data-ttu-id="f29e0-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f29e0-107">Properties</span></span>
|<span data-ttu-id="f29e0-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f29e0-108">Property</span></span>|<span data-ttu-id="f29e0-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="f29e0-109">Type</span></span>|<span data-ttu-id="f29e0-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f29e0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f29e0-111">displayName</span><span class="sxs-lookup"><span data-stu-id="f29e0-111">displayName</span></span>|<span data-ttu-id="f29e0-112">String</span><span class="sxs-lookup"><span data-stu-id="f29e0-112">String</span></span>|<span data-ttu-id="f29e0-113">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="f29e0-113">Display Name.</span></span>|
|<span data-ttu-id="f29e0-114">descrição</span><span class="sxs-lookup"><span data-stu-id="f29e0-114">description</span></span>|<span data-ttu-id="f29e0-115">String</span><span class="sxs-lookup"><span data-stu-id="f29e0-115">String</span></span>|<span data-ttu-id="f29e0-116">Descrição.</span><span class="sxs-lookup"><span data-stu-id="f29e0-116">Description.</span></span>|
|<span data-ttu-id="f29e0-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="f29e0-117">omaUri</span></span>|<span data-ttu-id="f29e0-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f29e0-118">String</span></span>|<span data-ttu-id="f29e0-119">OMA.</span><span class="sxs-lookup"><span data-stu-id="f29e0-119">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f29e0-120">Relações</span><span class="sxs-lookup"><span data-stu-id="f29e0-120">Relationships</span></span>
<span data-ttu-id="f29e0-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f29e0-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f29e0-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f29e0-122">JSON Representation</span></span>
<span data-ttu-id="f29e0-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f29e0-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSetting",
  "displayName": "String",
  "description": "String",
  "omaUri": "String"
}
```





