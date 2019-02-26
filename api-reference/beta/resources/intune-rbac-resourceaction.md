---
title: Tipo de recurso resourceAction
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d229a6d4d8b514cbf092efb224ff09dfb0c78ad4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30157621"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="6fdfc-103">Tipo de recurso resourceAction</span><span class="sxs-lookup"><span data-stu-id="6fdfc-103">resourceAction resource type</span></span>

> <span data-ttu-id="6fdfc-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6fdfc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6fdfc-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6fdfc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6fdfc-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="6fdfc-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="6fdfc-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6fdfc-107">Properties</span></span>
|<span data-ttu-id="6fdfc-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6fdfc-108">Property</span></span>|<span data-ttu-id="6fdfc-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="6fdfc-109">Type</span></span>|<span data-ttu-id="6fdfc-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6fdfc-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6fdfc-111">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="6fdfc-111">allowedResourceActions</span></span>|<span data-ttu-id="6fdfc-112">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6fdfc-112">String collection</span></span>|<span data-ttu-id="6fdfc-113">Ações permitidas</span><span class="sxs-lookup"><span data-stu-id="6fdfc-113">Allowed Actions</span></span>|
|<span data-ttu-id="6fdfc-114">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="6fdfc-114">notAllowedResourceActions</span></span>|<span data-ttu-id="6fdfc-115">String collection</span><span class="sxs-lookup"><span data-stu-id="6fdfc-115">String collection</span></span>|<span data-ttu-id="6fdfc-116">Ações não permitidas</span><span class="sxs-lookup"><span data-stu-id="6fdfc-116">Not Allowed Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="6fdfc-117">Relações</span><span class="sxs-lookup"><span data-stu-id="6fdfc-117">Relationships</span></span>
<span data-ttu-id="6fdfc-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6fdfc-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6fdfc-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6fdfc-119">JSON Representation</span></span>
<span data-ttu-id="6fdfc-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6fdfc-120">Here is a JSON representation of the resource.</span></span>
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




