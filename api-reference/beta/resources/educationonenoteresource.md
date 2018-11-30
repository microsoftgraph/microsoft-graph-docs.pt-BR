---
title: tipo de recurso de educationOneNoteResource
description: 'Uma subclasse de educationResource. Isso representa o local da página do OneNote.  '
ms.openlocfilehash: cfaaaf0a97e2dcea3a0a2a7384c761b678858f5b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037381"
---
# <a name="educationonenoteresource-resource-type"></a><span data-ttu-id="2b777-104">tipo de recurso de educationOneNoteResource</span><span class="sxs-lookup"><span data-stu-id="2b777-104">educationOneNoteResource resource type</span></span>

> <span data-ttu-id="2b777-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2b777-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2b777-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2b777-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2b777-107">Uma subclasse de [educationResource](educationresource.md).</span><span class="sxs-lookup"><span data-stu-id="2b777-107">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="2b777-108">Isso representa o local da página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="2b777-108">This represents the location of the OneNote page.</span></span>  

## <a name="properties"></a><span data-ttu-id="2b777-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2b777-109">Properties</span></span>
| <span data-ttu-id="2b777-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2b777-110">Property</span></span>     | <span data-ttu-id="2b777-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="2b777-111">Type</span></span>   |<span data-ttu-id="2b777-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="2b777-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2b777-113">pageUrl</span><span class="sxs-lookup"><span data-stu-id="2b777-113">pageUrl</span></span>|<span data-ttu-id="2b777-114">String</span><span class="sxs-lookup"><span data-stu-id="2b777-114">String</span></span>|<span data-ttu-id="2b777-115">A URL de gráfico da Microsoft a página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="2b777-115">The Microsoft Graph URL to the page in OneNote.</span></span>|
|<span data-ttu-id="2b777-116">sectionName</span><span class="sxs-lookup"><span data-stu-id="2b777-116">sectionName</span></span>|<span data-ttu-id="2b777-117">String</span><span class="sxs-lookup"><span data-stu-id="2b777-117">String</span></span>|<span data-ttu-id="2b777-118">Nome da seção que devem ser copiadas para distribuições ou que foram copiadas para.</span><span class="sxs-lookup"><span data-stu-id="2b777-118">Section name that distributions should be copied into or were copied into.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2b777-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2b777-119">JSON representation</span></span>

<span data-ttu-id="2b777-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2b777-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationOneNoteResource"
}-->

```json
{
  "pageUrl": "String",
  "sectionName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationOneNoteResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
