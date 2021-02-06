---
title: Tipo de recurso governanceSubject
description: Representa usuários, grupos e entidades de serviço sendo gerenciadas no Privileged Identity Management (PIM).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: eedcaff8538d5a0efa110b34cd6a72aef2a3210a
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132663"
---
# <a name="governancesubject-resource-type"></a><span data-ttu-id="6f665-103">Tipo de recurso governanceSubject</span><span class="sxs-lookup"><span data-stu-id="6f665-103">governanceSubject resource type</span></span>

<span data-ttu-id="6f665-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f665-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6f665-105">Representa usuários, grupos e entidades de serviço sendo gerenciadas no Privileged Identity Management (PIM).</span><span class="sxs-lookup"><span data-stu-id="6f665-105">Represents users, groups, and service principals being managed in Privileged Identity Management (PIM).</span></span>


## <a name="properties"></a><span data-ttu-id="6f665-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6f665-106">Properties</span></span>
| <span data-ttu-id="6f665-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6f665-107">Property</span></span>  | <span data-ttu-id="6f665-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="6f665-108">Type</span></span>       |<span data-ttu-id="6f665-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f665-109">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="6f665-110">id</span><span class="sxs-lookup"><span data-stu-id="6f665-110">id</span></span>         |<span data-ttu-id="6f665-111">String</span><span class="sxs-lookup"><span data-stu-id="6f665-111">String</span></span>     | <span data-ttu-id="6f665-112">A id do assunto.</span><span class="sxs-lookup"><span data-stu-id="6f665-112">The id of the subject.</span></span>|
|<span data-ttu-id="6f665-113">type</span><span class="sxs-lookup"><span data-stu-id="6f665-113">type</span></span>       |<span data-ttu-id="6f665-114">String</span><span class="sxs-lookup"><span data-stu-id="6f665-114">String</span></span>     |<span data-ttu-id="6f665-115">O tipo do assunto.</span><span class="sxs-lookup"><span data-stu-id="6f665-115">The type of the subject.</span></span> <span data-ttu-id="6f665-116">O valor pode ser ``User`` ``Group`` , e ``ServicePrincipal`` .</span><span class="sxs-lookup"><span data-stu-id="6f665-116">The value can be ``User``, ``Group``, and ``ServicePrincipal``.</span></span>|
|<span data-ttu-id="6f665-117">displayName</span><span class="sxs-lookup"><span data-stu-id="6f665-117">displayName</span></span>|<span data-ttu-id="6f665-118">String</span><span class="sxs-lookup"><span data-stu-id="6f665-118">String</span></span>     |<span data-ttu-id="6f665-119">O nome de exibição do assunto.</span><span class="sxs-lookup"><span data-stu-id="6f665-119">The display name of the subject.</span></span>|
|<span data-ttu-id="6f665-120">email</span><span class="sxs-lookup"><span data-stu-id="6f665-120">email</span></span>      |<span data-ttu-id="6f665-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6f665-121">String</span></span>     |<span data-ttu-id="6f665-122">O endereço de email do assunto do usuário.</span><span class="sxs-lookup"><span data-stu-id="6f665-122">The email address of the user subject.</span></span> <span data-ttu-id="6f665-123">Se o assunto estiver em outros tipos, ele está vazio.</span><span class="sxs-lookup"><span data-stu-id="6f665-123">If the subject is in other types, it is empty.</span></span>|
|<span data-ttu-id="6f665-124">principalName</span><span class="sxs-lookup"><span data-stu-id="6f665-124">principalName</span></span>|<span data-ttu-id="6f665-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6f665-125">String</span></span>   |<span data-ttu-id="6f665-126">O nome principal do assunto do usuário.</span><span class="sxs-lookup"><span data-stu-id="6f665-126">The principal name of the user subject.</span></span> <span data-ttu-id="6f665-127">Se o assunto estiver em outros tipos, ele está vazio.</span><span class="sxs-lookup"><span data-stu-id="6f665-127">If the subject is in other types, it is empty.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6f665-128">Relações</span><span class="sxs-lookup"><span data-stu-id="6f665-128">Relationships</span></span>
<span data-ttu-id="6f665-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6f665-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="6f665-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6f665-130">JSON representation</span></span>

<span data-ttu-id="6f665-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6f665-131">Here is a JSON representation of the resource.</span></span>

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


