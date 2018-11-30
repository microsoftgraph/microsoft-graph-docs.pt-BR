---
title: Tipo de recurso outlookUser
description: Representa os serviços do Outlook disponíveis para um usuário.
ms.openlocfilehash: 63bbabccc540046961d31c91fe7b1fb9afaaf4f8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006745"
---
# <a name="outlookuser-resource-type"></a><span data-ttu-id="b0050-103">Tipo de recurso outlookUser</span><span class="sxs-lookup"><span data-stu-id="b0050-103">outlookUser resource type</span></span>


<span data-ttu-id="b0050-104">Representa os serviços do Outlook disponíveis para um usuário.</span><span class="sxs-lookup"><span data-stu-id="b0050-104">Represents the Outlook services available to a user.</span></span>


## <a name="methods"></a><span data-ttu-id="b0050-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="b0050-105">Methods</span></span>

| <span data-ttu-id="b0050-106">Método</span><span class="sxs-lookup"><span data-stu-id="b0050-106">Method</span></span>           | <span data-ttu-id="b0050-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b0050-107">Return Type</span></span>    |<span data-ttu-id="b0050-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0050-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b0050-109">Criar categoria</span><span class="sxs-lookup"><span data-stu-id="b0050-109">Create category</span></span>](../api/outlookuser-post-mastercategories.md) | [<span data-ttu-id="b0050-110">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="b0050-110">outlookCategory</span></span>](outlookcategory.md) |<span data-ttu-id="b0050-111">Cria um objeto **outlookCategory** na lista mestra de categorias do usuário.</span><span class="sxs-lookup"><span data-stu-id="b0050-111">Create an **outlookCategory** object in the user's master list of categories.</span></span>|
|[<span data-ttu-id="b0050-112">Listar categorias</span><span class="sxs-lookup"><span data-stu-id="b0050-112">List categories</span></span>](../api/outlookuser-list-mastercategories.md) | <span data-ttu-id="b0050-113">Coleção [outlookCategory](outlookcategory.md)</span><span class="sxs-lookup"><span data-stu-id="b0050-113">[outlookCategory](outlookcategory.md) collection</span></span> |<span data-ttu-id="b0050-114">Obtém todas as categorias que foram definidas para o usuário.</span><span class="sxs-lookup"><span data-stu-id="b0050-114">Get all the categories that have been defined for the user.</span></span>|
|[<span data-ttu-id="b0050-115">supportedLanguages</span><span class="sxs-lookup"><span data-stu-id="b0050-115">supportedLanguages</span></span>](../api/outlookuser-supportedlanguages.md) | <span data-ttu-id="b0050-116">Coleção [localeInfo](localeinfo.md)</span><span class="sxs-lookup"><span data-stu-id="b0050-116">[localeInfo](localeinfo.md) collection</span></span> | <span data-ttu-id="b0050-117">Obtém a lista de localidades e idiomas com suporte para o usuário, conforme configurado no servidor de caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="b0050-117">Get the list of locales and languages that is supported for the user, as configured on the user's mailbox server.</span></span> |
|[<span data-ttu-id="b0050-118">supportedTimeZones</span><span class="sxs-lookup"><span data-stu-id="b0050-118">supportedTimeZones</span></span>](../api/outlookuser-supportedtimezones.md) | <span data-ttu-id="b0050-119">Coleção [timeZoneInformation](timezoneinformation.md)</span><span class="sxs-lookup"><span data-stu-id="b0050-119">[timeZoneInformation](timezoneinformation.md) collection</span></span> | <span data-ttu-id="b0050-120">Obtém a lista de fusos horários com suporte para o usuário, conforme configurado no servidor de caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="b0050-120">Get the list of time zones that is supported for the user, as configured on the user's mailbox server.</span></span> |


## <a name="properties"></a><span data-ttu-id="b0050-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b0050-121">Properties</span></span>
<span data-ttu-id="b0050-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b0050-122">None</span></span>

## <a name="relationships"></a><span data-ttu-id="b0050-123">Relações</span><span class="sxs-lookup"><span data-stu-id="b0050-123">Relationships</span></span>
| <span data-ttu-id="b0050-124">Relação</span><span class="sxs-lookup"><span data-stu-id="b0050-124">Relationship</span></span> | <span data-ttu-id="b0050-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0050-125">Type</span></span>   |<span data-ttu-id="b0050-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0050-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b0050-127">masterCategories</span><span class="sxs-lookup"><span data-stu-id="b0050-127">masterCategories</span></span>|<span data-ttu-id="b0050-128">Coleção [outlookCategory](../resources/outlookcategory.md)</span><span class="sxs-lookup"><span data-stu-id="b0050-128">[outlookCategory](../resources/outlookcategory.md) collection</span></span>| <span data-ttu-id="b0050-129">Uma lista de categorias definidas para o usuário.</span><span class="sxs-lookup"><span data-stu-id="b0050-129">A list of categories defined for the user.</span></span> | 

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