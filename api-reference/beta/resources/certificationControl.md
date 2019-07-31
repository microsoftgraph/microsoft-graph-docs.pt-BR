---
title: " tipo de recurso certificationControl"
description: Este recurso contém dados de certificação de conformidade associados ao controle de Pontuação segura.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 22dc12070a801988d814ba73c6bffe1414bb5218
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012993"
---
#  <a name="certificationcontrol-resource-type"></a><span data-ttu-id="9a4d3-103">tipo de recurso certificationControl</span><span class="sxs-lookup"><span data-stu-id="9a4d3-103">certificationControl resource type</span></span>

<span data-ttu-id="9a4d3-104">Contém dados de certificação de conformidade associados ao controle de Pontuação segura.</span><span class="sxs-lookup"><span data-stu-id="9a4d3-104">Contains compliance certification data associated with secure score control.</span></span>

|<span data-ttu-id="9a4d3-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9a4d3-105">Property</span></span> |<span data-ttu-id="9a4d3-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="9a4d3-106">Type</span></span> |<span data-ttu-id="9a4d3-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a4d3-107">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="9a4d3-108">name</span><span class="sxs-lookup"><span data-stu-id="9a4d3-108">name</span></span> | <span data-ttu-id="9a4d3-109">string</span><span class="sxs-lookup"><span data-stu-id="9a4d3-109">string</span></span> | <span data-ttu-id="9a4d3-110">Nome do controle de certificação</span><span class="sxs-lookup"><span data-stu-id="9a4d3-110">Certification control name</span></span> |
|<span data-ttu-id="9a4d3-111">url</span><span class="sxs-lookup"><span data-stu-id="9a4d3-111">url</span></span> | <span data-ttu-id="9a4d3-112">string</span><span class="sxs-lookup"><span data-stu-id="9a4d3-112">string</span></span> | <span data-ttu-id="9a4d3-113">URL para o portal de confiança do serviço Microsoft</span><span class="sxs-lookup"><span data-stu-id="9a4d3-113">URL for the Microsoft Service Trust Portal</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9a4d3-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9a4d3-114">JSON representation</span></span>

<span data-ttu-id="9a4d3-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9a4d3-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.certificationControl"
}-->

```json
{
  "name": "String",
  "url": "Collection(microsoft.graph.certificationControl)"
}

```


<!-- {
  "type": "#page.annotation",
  "description": "certificationControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
