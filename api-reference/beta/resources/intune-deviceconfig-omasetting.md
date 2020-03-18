---
title: Tipo de recurso omaSetting
description: Configurações de OMA.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f53e50bdf3584ab7f34afedbd938ad0749eb23b6
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42788482"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="48de2-103">Tipo de recurso omaSetting</span><span class="sxs-lookup"><span data-stu-id="48de2-103">omaSetting resource type</span></span>

> <span data-ttu-id="48de2-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="48de2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="48de2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="48de2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="48de2-106">Configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="48de2-106">OMA Settings definition.</span></span>

## <a name="properties"></a><span data-ttu-id="48de2-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="48de2-107">Properties</span></span>
|<span data-ttu-id="48de2-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="48de2-108">Property</span></span>|<span data-ttu-id="48de2-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="48de2-109">Type</span></span>|<span data-ttu-id="48de2-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="48de2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48de2-111">displayName</span><span class="sxs-lookup"><span data-stu-id="48de2-111">displayName</span></span>|<span data-ttu-id="48de2-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="48de2-112">String</span></span>|<span data-ttu-id="48de2-113">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="48de2-113">Display Name.</span></span>|
|<span data-ttu-id="48de2-114">description</span><span class="sxs-lookup"><span data-stu-id="48de2-114">description</span></span>|<span data-ttu-id="48de2-115">String</span><span class="sxs-lookup"><span data-stu-id="48de2-115">String</span></span>|<span data-ttu-id="48de2-116">Descrição.</span><span class="sxs-lookup"><span data-stu-id="48de2-116">Description.</span></span>|
|<span data-ttu-id="48de2-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="48de2-117">omaUri</span></span>|<span data-ttu-id="48de2-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="48de2-118">String</span></span>|<span data-ttu-id="48de2-119">OMA.</span><span class="sxs-lookup"><span data-stu-id="48de2-119">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="48de2-120">Relações</span><span class="sxs-lookup"><span data-stu-id="48de2-120">Relationships</span></span>
<span data-ttu-id="48de2-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="48de2-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="48de2-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="48de2-122">JSON Representation</span></span>
<span data-ttu-id="48de2-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="48de2-123">Here is a JSON representation of the resource.</span></span>
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



