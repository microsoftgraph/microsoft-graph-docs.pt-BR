---
title: Tipo de recurso outlookUser
description: Representa os serviços do Outlook disponíveis para um usuário.
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: fd2cd782fafbcff4c3006bea22c659c6607bf11a
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137001"
---
# <a name="outlookuser-resource-type"></a><span data-ttu-id="416a6-103">Tipo de recurso outlookUser</span><span class="sxs-lookup"><span data-stu-id="416a6-103">outlookUser resource type</span></span>

<span data-ttu-id="416a6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="416a6-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="416a6-105">Representa os serviços do Outlook disponíveis para um usuário.</span><span class="sxs-lookup"><span data-stu-id="416a6-105">Represents the Outlook services available to a user.</span></span>


## <a name="methods"></a><span data-ttu-id="416a6-106">Methods</span><span class="sxs-lookup"><span data-stu-id="416a6-106">Methods</span></span>

| <span data-ttu-id="416a6-107">Método</span><span class="sxs-lookup"><span data-stu-id="416a6-107">Method</span></span>           | <span data-ttu-id="416a6-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="416a6-108">Return Type</span></span>    |<span data-ttu-id="416a6-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="416a6-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="416a6-110">Criar categoria</span><span class="sxs-lookup"><span data-stu-id="416a6-110">Create category</span></span>](../api/outlookuser-post-mastercategories.md) | [<span data-ttu-id="416a6-111">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="416a6-111">outlookCategory</span></span>](outlookcategory.md) |<span data-ttu-id="416a6-112">Cria um objeto **outlookCategory** na lista mestra de categorias do usuário.</span><span class="sxs-lookup"><span data-stu-id="416a6-112">Create an **outlookCategory** object in the user's master list of categories.</span></span>|
|[<span data-ttu-id="416a6-113">Listar categorias</span><span class="sxs-lookup"><span data-stu-id="416a6-113">List categories</span></span>](../api/outlookuser-list-mastercategories.md) | <span data-ttu-id="416a6-114">Coleção [outlookCategory](outlookcategory.md)</span><span class="sxs-lookup"><span data-stu-id="416a6-114">[outlookCategory](outlookcategory.md) collection</span></span> |<span data-ttu-id="416a6-115">Obtém todas as categorias que foram definidas para o usuário.</span><span class="sxs-lookup"><span data-stu-id="416a6-115">Get all the categories that have been defined for the user.</span></span>|
|[<span data-ttu-id="416a6-116">supportedLanguages</span><span class="sxs-lookup"><span data-stu-id="416a6-116">supportedLanguages</span></span>](../api/outlookuser-supportedlanguages.md) | <span data-ttu-id="416a6-117">Coleção [localeInfo](localeinfo.md)</span><span class="sxs-lookup"><span data-stu-id="416a6-117">[localeInfo](localeinfo.md) collection</span></span> | <span data-ttu-id="416a6-118">Obtém a lista de localidades e idiomas com suporte para o usuário, conforme configurado no servidor de caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="416a6-118">Get the list of locales and languages that is supported for the user, as configured on the user's mailbox server.</span></span> |
|[<span data-ttu-id="416a6-119">supportedTimeZones</span><span class="sxs-lookup"><span data-stu-id="416a6-119">supportedTimeZones</span></span>](../api/outlookuser-supportedtimezones.md) | <span data-ttu-id="416a6-120">Coleção [timeZoneInformation](timezoneinformation.md)</span><span class="sxs-lookup"><span data-stu-id="416a6-120">[timeZoneInformation](timezoneinformation.md) collection</span></span> | <span data-ttu-id="416a6-121">Obtém a lista de fusos horários com suporte para o usuário, conforme configurado no servidor de caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="416a6-121">Get the list of time zones that is supported for the user, as configured on the user's mailbox server.</span></span> |


## <a name="properties"></a><span data-ttu-id="416a6-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="416a6-122">Properties</span></span>
<span data-ttu-id="416a6-123">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="416a6-123">None</span></span>

## <a name="relationships"></a><span data-ttu-id="416a6-124">Relações</span><span class="sxs-lookup"><span data-stu-id="416a6-124">Relationships</span></span>
| <span data-ttu-id="416a6-125">Relação</span><span class="sxs-lookup"><span data-stu-id="416a6-125">Relationship</span></span> | <span data-ttu-id="416a6-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="416a6-126">Type</span></span>   |<span data-ttu-id="416a6-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="416a6-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="416a6-128">masterCategories</span><span class="sxs-lookup"><span data-stu-id="416a6-128">masterCategories</span></span>|<span data-ttu-id="416a6-129">Coleção [outlookCategory](../resources/outlookcategory.md)</span><span class="sxs-lookup"><span data-stu-id="416a6-129">[outlookCategory](../resources/outlookcategory.md) collection</span></span>| <span data-ttu-id="416a6-130">Uma lista de categorias definidas para o usuário.</span><span class="sxs-lookup"><span data-stu-id="416a6-130">A list of categories defined for the user.</span></span> | 

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

