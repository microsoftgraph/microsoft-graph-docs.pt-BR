---
title: Tipo de recurso outlookUser
description: Representa os serviços do Outlook disponíveis para um usuário.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 32d621b71770d220487b60b4573fb34cdf28d526
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462666"
---
# <a name="outlookuser-resource-type"></a><span data-ttu-id="bb846-103">Tipo de recurso outlookUser</span><span class="sxs-lookup"><span data-stu-id="bb846-103">outlookUser resource type</span></span>


<span data-ttu-id="bb846-104">Representa os serviços do Outlook disponíveis para um usuário.</span><span class="sxs-lookup"><span data-stu-id="bb846-104">Represents the Outlook services available to a user.</span></span>


## <a name="methods"></a><span data-ttu-id="bb846-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="bb846-105">Methods</span></span>

| <span data-ttu-id="bb846-106">Método</span><span class="sxs-lookup"><span data-stu-id="bb846-106">Method</span></span>           | <span data-ttu-id="bb846-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="bb846-107">Return Type</span></span>    |<span data-ttu-id="bb846-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb846-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bb846-109">Criar categoria</span><span class="sxs-lookup"><span data-stu-id="bb846-109">Create category</span></span>](../api/outlookuser-post-mastercategories.md) | [<span data-ttu-id="bb846-110">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="bb846-110">outlookCategory</span></span>](outlookcategory.md) |<span data-ttu-id="bb846-111">Cria um objeto **outlookCategory** na lista mestra de categorias do usuário.</span><span class="sxs-lookup"><span data-stu-id="bb846-111">Create an **outlookCategory** object in the user's master list of categories.</span></span>|
|[<span data-ttu-id="bb846-112">Listar categorias</span><span class="sxs-lookup"><span data-stu-id="bb846-112">List categories</span></span>](../api/outlookuser-list-mastercategories.md) | <span data-ttu-id="bb846-113">Coleção [outlookCategory](outlookcategory.md)</span><span class="sxs-lookup"><span data-stu-id="bb846-113">[outlookCategory](outlookcategory.md) collection</span></span> |<span data-ttu-id="bb846-114">Obtém todas as categorias que foram definidas para o usuário.</span><span class="sxs-lookup"><span data-stu-id="bb846-114">Get all the categories that have been defined for the user.</span></span>|
|[<span data-ttu-id="bb846-115">supportedLanguages</span><span class="sxs-lookup"><span data-stu-id="bb846-115">supportedLanguages</span></span>](../api/outlookuser-supportedlanguages.md) | <span data-ttu-id="bb846-116">Coleção [localeInfo](localeinfo.md)</span><span class="sxs-lookup"><span data-stu-id="bb846-116">[localeInfo](localeinfo.md) collection</span></span> | <span data-ttu-id="bb846-117">Obtém a lista de localidades e idiomas com suporte para o usuário, conforme configurado no servidor de caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="bb846-117">Get the list of locales and languages that is supported for the user, as configured on the user's mailbox server.</span></span> |
|[<span data-ttu-id="bb846-118">supportedTimeZones</span><span class="sxs-lookup"><span data-stu-id="bb846-118">supportedTimeZones</span></span>](../api/outlookuser-supportedtimezones.md) | <span data-ttu-id="bb846-119">Coleção [timeZoneInformation](timezoneinformation.md)</span><span class="sxs-lookup"><span data-stu-id="bb846-119">[timeZoneInformation](timezoneinformation.md) collection</span></span> | <span data-ttu-id="bb846-120">Obtém a lista de fusos horários com suporte para o usuário, conforme configurado no servidor de caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="bb846-120">Get the list of time zones that is supported for the user, as configured on the user's mailbox server.</span></span> |


## <a name="properties"></a><span data-ttu-id="bb846-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bb846-121">Properties</span></span>
<span data-ttu-id="bb846-122">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="bb846-122">None</span></span>

## <a name="relationships"></a><span data-ttu-id="bb846-123">Relações</span><span class="sxs-lookup"><span data-stu-id="bb846-123">Relationships</span></span>
| <span data-ttu-id="bb846-124">Relação</span><span class="sxs-lookup"><span data-stu-id="bb846-124">Relationship</span></span> | <span data-ttu-id="bb846-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="bb846-125">Type</span></span>   |<span data-ttu-id="bb846-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb846-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bb846-127">masterCategories</span><span class="sxs-lookup"><span data-stu-id="bb846-127">masterCategories</span></span>|<span data-ttu-id="bb846-128">Coleção [outlookCategory](../resources/outlookcategory.md)</span><span class="sxs-lookup"><span data-stu-id="bb846-128">[outlookCategory](../resources/outlookcategory.md) collection</span></span>| <span data-ttu-id="bb846-129">Uma lista de categorias definidas para o usuário.</span><span class="sxs-lookup"><span data-stu-id="bb846-129">A list of categories defined for the user.</span></span> | 

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
