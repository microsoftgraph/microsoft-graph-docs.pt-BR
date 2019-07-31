---
title: tipo de recurso governanceSubject
description: Representa usuários, grupos e entidades de serviço que estão sendo gerenciados no gerenciamento de identidade privilegiada (PIM).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 26f6c6904de97fc96eb1b29b9bcbc376bcf69c61
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005972"
---
# <a name="governancesubject-resource-type"></a><span data-ttu-id="a9af3-103">tipo de recurso governanceSubject</span><span class="sxs-lookup"><span data-stu-id="a9af3-103">governanceSubject resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9af3-104">Representa usuários, grupos e entidades de serviço que estão sendo gerenciados no gerenciamento de identidade privilegiada (PIM).</span><span class="sxs-lookup"><span data-stu-id="a9af3-104">Represents users, groups, and service principals being managed in Privileged Identity Management (PIM).</span></span>


## <a name="properties"></a><span data-ttu-id="a9af3-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a9af3-105">Properties</span></span>
| <span data-ttu-id="a9af3-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a9af3-106">Property</span></span>  | <span data-ttu-id="a9af3-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="a9af3-107">Type</span></span>       |<span data-ttu-id="a9af3-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9af3-108">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="a9af3-109">id</span><span class="sxs-lookup"><span data-stu-id="a9af3-109">id</span></span>         |<span data-ttu-id="a9af3-110">String</span><span class="sxs-lookup"><span data-stu-id="a9af3-110">String</span></span>     | <span data-ttu-id="a9af3-111">A ID do assunto.</span><span class="sxs-lookup"><span data-stu-id="a9af3-111">The id of the subject.</span></span>|
|<span data-ttu-id="a9af3-112">type</span><span class="sxs-lookup"><span data-stu-id="a9af3-112">type</span></span>       |<span data-ttu-id="a9af3-113">String</span><span class="sxs-lookup"><span data-stu-id="a9af3-113">String</span></span>     |<span data-ttu-id="a9af3-114">O tipo do assunto.</span><span class="sxs-lookup"><span data-stu-id="a9af3-114">The type of the subject.</span></span> <span data-ttu-id="a9af3-115">O valor pode ser ``User``, ``Group``e ``ServicePrincipal``.</span><span class="sxs-lookup"><span data-stu-id="a9af3-115">The value can be ``User``, ``Group``, and ``ServicePrincipal``.</span></span>|
|<span data-ttu-id="a9af3-116">displayName</span><span class="sxs-lookup"><span data-stu-id="a9af3-116">displayName</span></span>|<span data-ttu-id="a9af3-117">String</span><span class="sxs-lookup"><span data-stu-id="a9af3-117">String</span></span>     |<span data-ttu-id="a9af3-118">O nome de exibição do assunto.</span><span class="sxs-lookup"><span data-stu-id="a9af3-118">The display name of the subject.</span></span>|
|<span data-ttu-id="a9af3-119">email</span><span class="sxs-lookup"><span data-stu-id="a9af3-119">email</span></span>      |<span data-ttu-id="a9af3-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a9af3-120">String</span></span>     |<span data-ttu-id="a9af3-121">O endereço de email do assunto do usuário.</span><span class="sxs-lookup"><span data-stu-id="a9af3-121">The email address of the user subject.</span></span> <span data-ttu-id="a9af3-122">Se o assunto estiver em outros tipos, ele estará vazio.</span><span class="sxs-lookup"><span data-stu-id="a9af3-122">If the subject is in other types, it is empty.</span></span>|
|<span data-ttu-id="a9af3-123">principalName</span><span class="sxs-lookup"><span data-stu-id="a9af3-123">principalName</span></span>|<span data-ttu-id="a9af3-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a9af3-124">String</span></span>   |<span data-ttu-id="a9af3-125">O nome da entidade de segurança do usuário.</span><span class="sxs-lookup"><span data-stu-id="a9af3-125">The principal name of the user subject.</span></span> <span data-ttu-id="a9af3-126">Se o assunto estiver em outros tipos, ele estará vazio.</span><span class="sxs-lookup"><span data-stu-id="a9af3-126">If the subject is in other types, it is empty.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a9af3-127">Relações</span><span class="sxs-lookup"><span data-stu-id="a9af3-127">Relationships</span></span>
<span data-ttu-id="a9af3-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a9af3-128">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="a9af3-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a9af3-129">JSON representation</span></span>

<span data-ttu-id="a9af3-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a9af3-130">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceSubject"
}-->

```json
{
  "id": "String",  
  "displayName": "String",
  "email": "String",
  "principalName": "String",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceSubject",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
