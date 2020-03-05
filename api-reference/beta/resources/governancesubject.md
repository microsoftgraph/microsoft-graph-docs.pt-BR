---
title: tipo de recurso governanceSubject
description: Representa usuários, grupos e entidades de serviço que estão sendo gerenciados no gerenciamento de identidade privilegiada (PIM).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 4d1fbf75b4e9643dc0e3b968ace7a013616904ad
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42497168"
---
# <a name="governancesubject-resource-type"></a><span data-ttu-id="89aaf-103">tipo de recurso governanceSubject</span><span class="sxs-lookup"><span data-stu-id="89aaf-103">governanceSubject resource type</span></span>

<span data-ttu-id="89aaf-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="89aaf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="89aaf-105">Representa usuários, grupos e entidades de serviço que estão sendo gerenciados no gerenciamento de identidade privilegiada (PIM).</span><span class="sxs-lookup"><span data-stu-id="89aaf-105">Represents users, groups, and service principals being managed in Privileged Identity Management (PIM).</span></span>


## <a name="properties"></a><span data-ttu-id="89aaf-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="89aaf-106">Properties</span></span>
| <span data-ttu-id="89aaf-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="89aaf-107">Property</span></span>  | <span data-ttu-id="89aaf-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="89aaf-108">Type</span></span>       |<span data-ttu-id="89aaf-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="89aaf-109">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="89aaf-110">id</span><span class="sxs-lookup"><span data-stu-id="89aaf-110">id</span></span>         |<span data-ttu-id="89aaf-111">String</span><span class="sxs-lookup"><span data-stu-id="89aaf-111">String</span></span>     | <span data-ttu-id="89aaf-112">A ID do assunto.</span><span class="sxs-lookup"><span data-stu-id="89aaf-112">The id of the subject.</span></span>|
|<span data-ttu-id="89aaf-113">type</span><span class="sxs-lookup"><span data-stu-id="89aaf-113">type</span></span>       |<span data-ttu-id="89aaf-114">String</span><span class="sxs-lookup"><span data-stu-id="89aaf-114">String</span></span>     |<span data-ttu-id="89aaf-115">O tipo do assunto.</span><span class="sxs-lookup"><span data-stu-id="89aaf-115">The type of the subject.</span></span> <span data-ttu-id="89aaf-116">O valor pode ser ``User``, ``Group``e ``ServicePrincipal``.</span><span class="sxs-lookup"><span data-stu-id="89aaf-116">The value can be ``User``, ``Group``, and ``ServicePrincipal``.</span></span>|
|<span data-ttu-id="89aaf-117">displayName</span><span class="sxs-lookup"><span data-stu-id="89aaf-117">displayName</span></span>|<span data-ttu-id="89aaf-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="89aaf-118">String</span></span>     |<span data-ttu-id="89aaf-119">O nome de exibição do assunto.</span><span class="sxs-lookup"><span data-stu-id="89aaf-119">The display name of the subject.</span></span>|
|<span data-ttu-id="89aaf-120">email</span><span class="sxs-lookup"><span data-stu-id="89aaf-120">email</span></span>      |<span data-ttu-id="89aaf-121">String</span><span class="sxs-lookup"><span data-stu-id="89aaf-121">String</span></span>     |<span data-ttu-id="89aaf-122">O endereço de email do assunto do usuário.</span><span class="sxs-lookup"><span data-stu-id="89aaf-122">The email address of the user subject.</span></span> <span data-ttu-id="89aaf-123">Se o assunto estiver em outros tipos, ele estará vazio.</span><span class="sxs-lookup"><span data-stu-id="89aaf-123">If the subject is in other types, it is empty.</span></span>|
|<span data-ttu-id="89aaf-124">principalName</span><span class="sxs-lookup"><span data-stu-id="89aaf-124">principalName</span></span>|<span data-ttu-id="89aaf-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="89aaf-125">String</span></span>   |<span data-ttu-id="89aaf-126">O nome da entidade de segurança do usuário.</span><span class="sxs-lookup"><span data-stu-id="89aaf-126">The principal name of the user subject.</span></span> <span data-ttu-id="89aaf-127">Se o assunto estiver em outros tipos, ele estará vazio.</span><span class="sxs-lookup"><span data-stu-id="89aaf-127">If the subject is in other types, it is empty.</span></span>|

## <a name="relationships"></a><span data-ttu-id="89aaf-128">Relações</span><span class="sxs-lookup"><span data-stu-id="89aaf-128">Relationships</span></span>
<span data-ttu-id="89aaf-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="89aaf-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="89aaf-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="89aaf-130">JSON representation</span></span>

<span data-ttu-id="89aaf-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="89aaf-131">Here is a JSON representation of the resource.</span></span>

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
