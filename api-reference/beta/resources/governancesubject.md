---
title: tipo de recurso governanceSubject
description: Representa usuários, grupos e entidades de serviço que estão sendo gerenciados no gerenciamento de identidade privilegiada (PIM).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: shauliu
ms.openlocfilehash: 384558109521fe93c5ef4331e88355c8757cf5fc
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809485"
---
# <a name="governancesubject-resource-type"></a><span data-ttu-id="4e11b-103">tipo de recurso governanceSubject</span><span class="sxs-lookup"><span data-stu-id="4e11b-103">governanceSubject resource type</span></span>

<span data-ttu-id="4e11b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e11b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e11b-105">Representa usuários, grupos e entidades de serviço que estão sendo gerenciados no gerenciamento de identidade privilegiada (PIM).</span><span class="sxs-lookup"><span data-stu-id="4e11b-105">Represents users, groups, and service principals being managed in Privileged Identity Management (PIM).</span></span>


## <a name="properties"></a><span data-ttu-id="4e11b-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4e11b-106">Properties</span></span>
| <span data-ttu-id="4e11b-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4e11b-107">Property</span></span>  | <span data-ttu-id="4e11b-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="4e11b-108">Type</span></span>       |<span data-ttu-id="4e11b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="4e11b-109">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="4e11b-110">id</span><span class="sxs-lookup"><span data-stu-id="4e11b-110">id</span></span>         |<span data-ttu-id="4e11b-111">String</span><span class="sxs-lookup"><span data-stu-id="4e11b-111">String</span></span>     | <span data-ttu-id="4e11b-112">A ID do assunto.</span><span class="sxs-lookup"><span data-stu-id="4e11b-112">The id of the subject.</span></span>|
|<span data-ttu-id="4e11b-113">type</span><span class="sxs-lookup"><span data-stu-id="4e11b-113">type</span></span>       |<span data-ttu-id="4e11b-114">String</span><span class="sxs-lookup"><span data-stu-id="4e11b-114">String</span></span>     |<span data-ttu-id="4e11b-115">O tipo do assunto.</span><span class="sxs-lookup"><span data-stu-id="4e11b-115">The type of the subject.</span></span> <span data-ttu-id="4e11b-116">O valor pode ser ``User`` , ``Group`` e ``ServicePrincipal`` .</span><span class="sxs-lookup"><span data-stu-id="4e11b-116">The value can be ``User``, ``Group``, and ``ServicePrincipal``.</span></span>|
|<span data-ttu-id="4e11b-117">displayName</span><span class="sxs-lookup"><span data-stu-id="4e11b-117">displayName</span></span>|<span data-ttu-id="4e11b-118">String</span><span class="sxs-lookup"><span data-stu-id="4e11b-118">String</span></span>     |<span data-ttu-id="4e11b-119">O nome de exibição do assunto.</span><span class="sxs-lookup"><span data-stu-id="4e11b-119">The display name of the subject.</span></span>|
|<span data-ttu-id="4e11b-120">email</span><span class="sxs-lookup"><span data-stu-id="4e11b-120">email</span></span>      |<span data-ttu-id="4e11b-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4e11b-121">String</span></span>     |<span data-ttu-id="4e11b-122">O endereço de email do assunto do usuário.</span><span class="sxs-lookup"><span data-stu-id="4e11b-122">The email address of the user subject.</span></span> <span data-ttu-id="4e11b-123">Se o assunto estiver em outros tipos, ele estará vazio.</span><span class="sxs-lookup"><span data-stu-id="4e11b-123">If the subject is in other types, it is empty.</span></span>|
|<span data-ttu-id="4e11b-124">principalName</span><span class="sxs-lookup"><span data-stu-id="4e11b-124">principalName</span></span>|<span data-ttu-id="4e11b-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4e11b-125">String</span></span>   |<span data-ttu-id="4e11b-126">O nome da entidade de segurança do usuário.</span><span class="sxs-lookup"><span data-stu-id="4e11b-126">The principal name of the user subject.</span></span> <span data-ttu-id="4e11b-127">Se o assunto estiver em outros tipos, ele estará vazio.</span><span class="sxs-lookup"><span data-stu-id="4e11b-127">If the subject is in other types, it is empty.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4e11b-128">Relações</span><span class="sxs-lookup"><span data-stu-id="4e11b-128">Relationships</span></span>
<span data-ttu-id="4e11b-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4e11b-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="4e11b-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4e11b-130">JSON representation</span></span>

<span data-ttu-id="4e11b-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4e11b-131">Here is a JSON representation of the resource.</span></span>

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
