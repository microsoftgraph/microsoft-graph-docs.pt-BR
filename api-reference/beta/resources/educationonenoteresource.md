---
title: tipo de recurso de educationOneNoteResource
description: 'Uma subclasse de educationResource. Isso representa o local da página do OneNote.  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: b10bef551cdc2dd29a8a20c69d2c4657ee66af4e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27927916"
---
# <a name="educationonenoteresource-resource-type"></a><span data-ttu-id="c7c98-104">tipo de recurso de educationOneNoteResource</span><span class="sxs-lookup"><span data-stu-id="c7c98-104">educationOneNoteResource resource type</span></span>

> <span data-ttu-id="c7c98-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c7c98-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c7c98-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c7c98-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c7c98-107">Uma subclasse de [educationResource](educationresource.md).</span><span class="sxs-lookup"><span data-stu-id="c7c98-107">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="c7c98-108">Isso representa o local da página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="c7c98-108">This represents the location of the OneNote page.</span></span>  

## <a name="properties"></a><span data-ttu-id="c7c98-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c7c98-109">Properties</span></span>
| <span data-ttu-id="c7c98-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c7c98-110">Property</span></span>     | <span data-ttu-id="c7c98-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="c7c98-111">Type</span></span>   |<span data-ttu-id="c7c98-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7c98-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c7c98-113">pageUrl</span><span class="sxs-lookup"><span data-stu-id="c7c98-113">pageUrl</span></span>|<span data-ttu-id="c7c98-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c7c98-114">String</span></span>|<span data-ttu-id="c7c98-115">A URL de gráfico da Microsoft a página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="c7c98-115">The Microsoft Graph URL to the page in OneNote.</span></span>|
|<span data-ttu-id="c7c98-116">sectionName</span><span class="sxs-lookup"><span data-stu-id="c7c98-116">sectionName</span></span>|<span data-ttu-id="c7c98-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c7c98-117">String</span></span>|<span data-ttu-id="c7c98-118">Nome da seção que devem ser copiadas para distribuições ou que foram copiadas para.</span><span class="sxs-lookup"><span data-stu-id="c7c98-118">Section name that distributions should be copied into or were copied into.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c7c98-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c7c98-119">JSON representation</span></span>

<span data-ttu-id="c7c98-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c7c98-120">The following is a JSON representation of the resource.</span></span>

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
