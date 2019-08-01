---
title: Tipo de recurso outlookUser
description: Representa os serviços do Outlook disponíveis para um usuário.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 754ae286c97e4c6ddae4ed6fb4f34aef5733090f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035676"
---
# <a name="outlookuser-resource-type"></a><span data-ttu-id="0d8a4-103">Tipo de recurso outlookUser</span><span class="sxs-lookup"><span data-stu-id="0d8a4-103">outlookUser resource type</span></span>


<span data-ttu-id="0d8a4-104">Representa os serviços do Outlook disponíveis para um usuário.</span><span class="sxs-lookup"><span data-stu-id="0d8a4-104">Represents the Outlook services available to a user.</span></span>


## <a name="methods"></a><span data-ttu-id="0d8a4-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="0d8a4-105">Methods</span></span>

| <span data-ttu-id="0d8a4-106">Método</span><span class="sxs-lookup"><span data-stu-id="0d8a4-106">Method</span></span>           | <span data-ttu-id="0d8a4-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0d8a4-107">Return Type</span></span>    |<span data-ttu-id="0d8a4-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="0d8a4-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0d8a4-109">Criar categoria</span><span class="sxs-lookup"><span data-stu-id="0d8a4-109">Create category</span></span>](../api/outlookuser-post-mastercategories.md) | [<span data-ttu-id="0d8a4-110">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="0d8a4-110">outlookCategory</span></span>](outlookcategory.md) |<span data-ttu-id="0d8a4-111">Cria um objeto **outlookCategory** na lista mestra de categorias do usuário.</span><span class="sxs-lookup"><span data-stu-id="0d8a4-111">Create an **outlookCategory** object in the user's master list of categories.</span></span>|
|[<span data-ttu-id="0d8a4-112">Listar categorias</span><span class="sxs-lookup"><span data-stu-id="0d8a4-112">List categories</span></span>](../api/outlookuser-list-mastercategories.md) | <span data-ttu-id="0d8a4-113">Coleção [outlookCategory](outlookcategory.md)</span><span class="sxs-lookup"><span data-stu-id="0d8a4-113">[outlookCategory](outlookcategory.md) collection</span></span> |<span data-ttu-id="0d8a4-114">Obtém todas as categorias que foram definidas para o usuário.</span><span class="sxs-lookup"><span data-stu-id="0d8a4-114">Get all the categories that have been defined for the user.</span></span>|
|[<span data-ttu-id="0d8a4-115">supportedLanguages</span><span class="sxs-lookup"><span data-stu-id="0d8a4-115">supportedLanguages</span></span>](../api/outlookuser-supportedlanguages.md) | <span data-ttu-id="0d8a4-116">Coleção [localeInfo](localeinfo.md)</span><span class="sxs-lookup"><span data-stu-id="0d8a4-116">[localeInfo](localeinfo.md) collection</span></span> | <span data-ttu-id="0d8a4-117">Obtém a lista de localidades e idiomas com suporte para o usuário, conforme configurado no servidor de caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="0d8a4-117">Get the list of locales and languages that is supported for the user, as configured on the user's mailbox server.</span></span> |
|[<span data-ttu-id="0d8a4-118">supportedTimeZones</span><span class="sxs-lookup"><span data-stu-id="0d8a4-118">supportedTimeZones</span></span>](../api/outlookuser-supportedtimezones.md) | <span data-ttu-id="0d8a4-119">Coleção [timeZoneInformation](timezoneinformation.md)</span><span class="sxs-lookup"><span data-stu-id="0d8a4-119">[timeZoneInformation](timezoneinformation.md) collection</span></span> | <span data-ttu-id="0d8a4-120">Obtém a lista de fusos horários com suporte para o usuário, conforme configurado no servidor de caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="0d8a4-120">Get the list of time zones that is supported for the user, as configured on the user's mailbox server.</span></span> |


## <a name="properties"></a><span data-ttu-id="0d8a4-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0d8a4-121">Properties</span></span>
<span data-ttu-id="0d8a4-122">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="0d8a4-122">None</span></span>

## <a name="relationships"></a><span data-ttu-id="0d8a4-123">Relações</span><span class="sxs-lookup"><span data-stu-id="0d8a4-123">Relationships</span></span>
| <span data-ttu-id="0d8a4-124">Relação</span><span class="sxs-lookup"><span data-stu-id="0d8a4-124">Relationship</span></span> | <span data-ttu-id="0d8a4-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="0d8a4-125">Type</span></span>   |<span data-ttu-id="0d8a4-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="0d8a4-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0d8a4-127">masterCategories</span><span class="sxs-lookup"><span data-stu-id="0d8a4-127">masterCategories</span></span>|<span data-ttu-id="0d8a4-128">Coleção [outlookCategory](../resources/outlookcategory.md)</span><span class="sxs-lookup"><span data-stu-id="0d8a4-128">[outlookCategory](../resources/outlookcategory.md) collection</span></span>| <span data-ttu-id="0d8a4-129">Uma lista de categorias definidas para o usuário.</span><span class="sxs-lookup"><span data-stu-id="0d8a4-129">A list of categories defined for the user.</span></span> | 

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.outlookUser",
  "@odata.annotations": [
    {
      "property": "masterCategories",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false
      }
    }
  ]
}-->
```json
{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
