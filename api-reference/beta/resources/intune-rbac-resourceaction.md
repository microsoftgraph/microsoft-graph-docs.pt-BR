---
title: Tipo de recurso resourceAction
description: Conjunto de ações permitidas e não permitidas para um recurso.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e49c06c8ca58f94948cc6458fd9dedd0adfa227e
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34993603"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="ece75-103">Tipo de recurso resourceAction</span><span class="sxs-lookup"><span data-stu-id="ece75-103">resourceAction resource type</span></span>

> <span data-ttu-id="ece75-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ece75-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ece75-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ece75-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ece75-106">Conjunto de ações permitidas e não permitidas para um recurso.</span><span class="sxs-lookup"><span data-stu-id="ece75-106">Set of allowed and not allowed actions for a resource.</span></span>

## <a name="properties"></a><span data-ttu-id="ece75-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ece75-107">Properties</span></span>
|<span data-ttu-id="ece75-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ece75-108">Property</span></span>|<span data-ttu-id="ece75-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="ece75-109">Type</span></span>|<span data-ttu-id="ece75-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ece75-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ece75-111">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="ece75-111">allowedResourceActions</span></span>|<span data-ttu-id="ece75-112">String collection</span><span class="sxs-lookup"><span data-stu-id="ece75-112">String collection</span></span>|<span data-ttu-id="ece75-113">Ações permitidas</span><span class="sxs-lookup"><span data-stu-id="ece75-113">Allowed Actions</span></span>|
|<span data-ttu-id="ece75-114">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="ece75-114">notAllowedResourceActions</span></span>|<span data-ttu-id="ece75-115">String collection</span><span class="sxs-lookup"><span data-stu-id="ece75-115">String collection</span></span>|<span data-ttu-id="ece75-116">Ações não permitidas.</span><span class="sxs-lookup"><span data-stu-id="ece75-116">Not Allowed Actions.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ece75-117">Relações</span><span class="sxs-lookup"><span data-stu-id="ece75-117">Relationships</span></span>
<span data-ttu-id="ece75-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ece75-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ece75-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ece75-119">JSON Representation</span></span>
<span data-ttu-id="ece75-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ece75-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.resourceAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.resourceAction",
  "allowedResourceActions": [
    "String"
  ],
  "notAllowedResourceActions": [
    "String"
  ]
}
```





