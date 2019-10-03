---
title: Tipo de recurso mimeContent
description: Contém as propriedades de um conteúdo genérico MIME.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ef174774c345debe18b9a3d66075af6e439a4583
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37367151"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="499f6-103">Tipo de recurso mimeContent</span><span class="sxs-lookup"><span data-stu-id="499f6-103">mimeContent resource type</span></span>

> <span data-ttu-id="499f6-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="499f6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="499f6-105">Contém as propriedades de um conteúdo genérico MIME.</span><span class="sxs-lookup"><span data-stu-id="499f6-105">Contains properties for a generic mime content.</span></span>

## <a name="properties"></a><span data-ttu-id="499f6-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="499f6-106">Properties</span></span>
|<span data-ttu-id="499f6-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="499f6-107">Property</span></span>|<span data-ttu-id="499f6-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="499f6-108">Type</span></span>|<span data-ttu-id="499f6-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="499f6-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="499f6-110">type</span><span class="sxs-lookup"><span data-stu-id="499f6-110">type</span></span>|<span data-ttu-id="499f6-111">String</span><span class="sxs-lookup"><span data-stu-id="499f6-111">String</span></span>|<span data-ttu-id="499f6-112">Indica o tipo de conteúdo MIME.</span><span class="sxs-lookup"><span data-stu-id="499f6-112">Indicates the content mime type.</span></span>|
|<span data-ttu-id="499f6-113">value</span><span class="sxs-lookup"><span data-stu-id="499f6-113">value</span></span>|<span data-ttu-id="499f6-114">Binária</span><span class="sxs-lookup"><span data-stu-id="499f6-114">Binary</span></span>|<span data-ttu-id="499f6-115">A matriz de byte que contém o conteúdo atual.</span><span class="sxs-lookup"><span data-stu-id="499f6-115">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="499f6-116">Relações</span><span class="sxs-lookup"><span data-stu-id="499f6-116">Relationships</span></span>
<span data-ttu-id="499f6-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="499f6-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="499f6-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="499f6-118">JSON Representation</span></span>
<span data-ttu-id="499f6-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="499f6-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mimeContent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mimeContent",
  "type": "String",
  "value": "binary"
}
```




