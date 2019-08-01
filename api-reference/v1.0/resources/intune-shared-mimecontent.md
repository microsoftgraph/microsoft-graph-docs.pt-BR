---
title: Tipo de recurso mimeContent
description: Contém as propriedades de um conteúdo genérico MIME.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 24563bb89af91c05dd71aeb284934c0406819711
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036887"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="9a4ac-103">Tipo de recurso mimeContent</span><span class="sxs-lookup"><span data-stu-id="9a4ac-103">mimeContent resource type</span></span>

> <span data-ttu-id="9a4ac-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9a4ac-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a4ac-105">Contém as propriedades de um conteúdo genérico MIME.</span><span class="sxs-lookup"><span data-stu-id="9a4ac-105">Contains properties for a generic mime content.</span></span>

## <a name="properties"></a><span data-ttu-id="9a4ac-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9a4ac-106">Properties</span></span>
|<span data-ttu-id="9a4ac-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9a4ac-107">Property</span></span>|<span data-ttu-id="9a4ac-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="9a4ac-108">Type</span></span>|<span data-ttu-id="9a4ac-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a4ac-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a4ac-110">type</span><span class="sxs-lookup"><span data-stu-id="9a4ac-110">type</span></span>|<span data-ttu-id="9a4ac-111">String</span><span class="sxs-lookup"><span data-stu-id="9a4ac-111">String</span></span>|<span data-ttu-id="9a4ac-112">Indica o tipo de conteúdo MIME.</span><span class="sxs-lookup"><span data-stu-id="9a4ac-112">Indicates the content mime type.</span></span>|
|<span data-ttu-id="9a4ac-113">value</span><span class="sxs-lookup"><span data-stu-id="9a4ac-113">value</span></span>|<span data-ttu-id="9a4ac-114">Binária</span><span class="sxs-lookup"><span data-stu-id="9a4ac-114">Binary</span></span>|<span data-ttu-id="9a4ac-115">A matriz de byte que contém o conteúdo atual.</span><span class="sxs-lookup"><span data-stu-id="9a4ac-115">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9a4ac-116">Relações</span><span class="sxs-lookup"><span data-stu-id="9a4ac-116">Relationships</span></span>
<span data-ttu-id="9a4ac-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9a4ac-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9a4ac-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9a4ac-118">JSON Representation</span></span>
<span data-ttu-id="9a4ac-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9a4ac-119">Here is a JSON representation of the resource.</span></span>
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



