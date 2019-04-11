---
title: tipo de recurso vppTokenActionResult
description: O status da ação executada com um token do Apple Volume Purchase Program.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cf8aeb73080ea16d89ec4b1473a7c44f25b4306a
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31790946"
---
# <a name="vpptokenactionresult-resource-type"></a><span data-ttu-id="ad9c9-103">tipo de recurso vppTokenActionResult</span><span class="sxs-lookup"><span data-stu-id="ad9c9-103">vppTokenActionResult resource type</span></span>

> <span data-ttu-id="ad9c9-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ad9c9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ad9c9-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ad9c9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ad9c9-106">O status da ação executada com um token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="ad9c9-106">The status of the action performed with an Apple Volume Purchase Program token.</span></span>

## <a name="properties"></a><span data-ttu-id="ad9c9-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ad9c9-107">Properties</span></span>
|<span data-ttu-id="ad9c9-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ad9c9-108">Property</span></span>|<span data-ttu-id="ad9c9-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="ad9c9-109">Type</span></span>|<span data-ttu-id="ad9c9-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ad9c9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad9c9-111">actionName</span><span class="sxs-lookup"><span data-stu-id="ad9c9-111">actionName</span></span>|<span data-ttu-id="ad9c9-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ad9c9-112">String</span></span>|<span data-ttu-id="ad9c9-113">Nome da ação</span><span class="sxs-lookup"><span data-stu-id="ad9c9-113">Action name</span></span>|
|<span data-ttu-id="ad9c9-114">actionState</span><span class="sxs-lookup"><span data-stu-id="ad9c9-114">actionState</span></span>|[<span data-ttu-id="ad9c9-115">actionState</span><span class="sxs-lookup"><span data-stu-id="ad9c9-115">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="ad9c9-116">Estado da ação.</span><span class="sxs-lookup"><span data-stu-id="ad9c9-116">State of the action.</span></span> <span data-ttu-id="ad9c9-117">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="ad9c9-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="ad9c9-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="ad9c9-118">startDateTime</span></span>|<span data-ttu-id="ad9c9-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ad9c9-119">DateTimeOffset</span></span>|<span data-ttu-id="ad9c9-120">Hora em que a ação foi iniciada</span><span class="sxs-lookup"><span data-stu-id="ad9c9-120">Time the action was initiated</span></span>|
|<span data-ttu-id="ad9c9-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="ad9c9-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="ad9c9-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ad9c9-122">DateTimeOffset</span></span>|<span data-ttu-id="ad9c9-123">Hora da última atualização do estado da ação</span><span class="sxs-lookup"><span data-stu-id="ad9c9-123">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="ad9c9-124">Relações</span><span class="sxs-lookup"><span data-stu-id="ad9c9-124">Relationships</span></span>
<span data-ttu-id="ad9c9-125">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="ad9c9-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ad9c9-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ad9c9-126">JSON Representation</span></span>
<span data-ttu-id="ad9c9-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ad9c9-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vppTokenActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppTokenActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)"
}
```





