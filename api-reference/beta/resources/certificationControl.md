---
title: " tipo de recurso certificationControl"
description: Este recurso contém dados de certificação de conformidade associados ao controle de Pontuação segura.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: bafd2c9d66c0d696649944f88e4fcfbdea4bcca6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507758"
---
#  <a name="certificationcontrol-resource-type"></a><span data-ttu-id="6fdf1-103">tipo de recurso certificationControl</span><span class="sxs-lookup"><span data-stu-id="6fdf1-103">certificationControl resource type</span></span>

<span data-ttu-id="6fdf1-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6fdf1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6fdf1-105">Contém dados de certificação de conformidade associados ao controle de Pontuação segura.</span><span class="sxs-lookup"><span data-stu-id="6fdf1-105">Contains compliance certification data associated with secure score control.</span></span>

|<span data-ttu-id="6fdf1-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6fdf1-106">Property</span></span> |<span data-ttu-id="6fdf1-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="6fdf1-107">Type</span></span> |<span data-ttu-id="6fdf1-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="6fdf1-108">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="6fdf1-109">nome</span><span class="sxs-lookup"><span data-stu-id="6fdf1-109">name</span></span> | <span data-ttu-id="6fdf1-110">string</span><span class="sxs-lookup"><span data-stu-id="6fdf1-110">string</span></span> | <span data-ttu-id="6fdf1-111">Nome do controle de certificação</span><span class="sxs-lookup"><span data-stu-id="6fdf1-111">Certification control name</span></span> |
|<span data-ttu-id="6fdf1-112">url</span><span class="sxs-lookup"><span data-stu-id="6fdf1-112">url</span></span> | <span data-ttu-id="6fdf1-113">string</span><span class="sxs-lookup"><span data-stu-id="6fdf1-113">string</span></span> | <span data-ttu-id="6fdf1-114">URL para o portal de confiança do serviço Microsoft</span><span class="sxs-lookup"><span data-stu-id="6fdf1-114">URL for the Microsoft Service Trust Portal</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6fdf1-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6fdf1-115">JSON representation</span></span>

<span data-ttu-id="6fdf1-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6fdf1-116">The following is a JSON representation of the resource.</span></span>

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
