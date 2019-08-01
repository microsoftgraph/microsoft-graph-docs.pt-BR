---
title: Tipo de recurso omaSetting
description: Configurações de OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b5a2d2152d107050f655d43dab2cb2c65f114868
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031343"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="07784-103">Tipo de recurso omaSetting</span><span class="sxs-lookup"><span data-stu-id="07784-103">omaSetting resource type</span></span>

> <span data-ttu-id="07784-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="07784-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07784-105">Configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="07784-105">OMA Settings definition.</span></span>

## <a name="properties"></a><span data-ttu-id="07784-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="07784-106">Properties</span></span>
|<span data-ttu-id="07784-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="07784-107">Property</span></span>|<span data-ttu-id="07784-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="07784-108">Type</span></span>|<span data-ttu-id="07784-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="07784-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07784-110">displayName</span><span class="sxs-lookup"><span data-stu-id="07784-110">displayName</span></span>|<span data-ttu-id="07784-111">String</span><span class="sxs-lookup"><span data-stu-id="07784-111">String</span></span>|<span data-ttu-id="07784-112">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="07784-112">Display Name.</span></span>|
|<span data-ttu-id="07784-113">descrição</span><span class="sxs-lookup"><span data-stu-id="07784-113">description</span></span>|<span data-ttu-id="07784-114">String</span><span class="sxs-lookup"><span data-stu-id="07784-114">String</span></span>|<span data-ttu-id="07784-115">Descrição.</span><span class="sxs-lookup"><span data-stu-id="07784-115">Description.</span></span>|
|<span data-ttu-id="07784-116">omaUri</span><span class="sxs-lookup"><span data-stu-id="07784-116">omaUri</span></span>|<span data-ttu-id="07784-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="07784-117">String</span></span>|<span data-ttu-id="07784-118">OMA.</span><span class="sxs-lookup"><span data-stu-id="07784-118">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="07784-119">Relações</span><span class="sxs-lookup"><span data-stu-id="07784-119">Relationships</span></span>
<span data-ttu-id="07784-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="07784-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="07784-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="07784-121">JSON Representation</span></span>
<span data-ttu-id="07784-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="07784-122">Here is a JSON representation of the resource.</span></span>
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



