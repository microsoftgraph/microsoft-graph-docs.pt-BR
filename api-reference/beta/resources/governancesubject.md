---
title: tipo de recurso de governanceSubject
description: Representa os usuários, grupos e entidades de serviço estão sendo gerenciadas no gerenciamento de identidade privilegiado (PIM).
ms.openlocfilehash: c2129a0da488d4e7f425d6ef3596a955269e0da8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033767"
---
# <a name="governancesubject-resource-type"></a><span data-ttu-id="76842-103">tipo de recurso de governanceSubject</span><span class="sxs-lookup"><span data-stu-id="76842-103">governanceSubject resource type</span></span>

> <span data-ttu-id="76842-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="76842-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="76842-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="76842-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="76842-106">Representa os usuários, grupos e entidades de serviço estão sendo gerenciadas no gerenciamento de identidade privilegiado (PIM).</span><span class="sxs-lookup"><span data-stu-id="76842-106">Represents users, groups, and service principals being managed in Privileged Identity Management (PIM).</span></span>


## <a name="properties"></a><span data-ttu-id="76842-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="76842-107">Properties</span></span>
| <span data-ttu-id="76842-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="76842-108">Property</span></span>  | <span data-ttu-id="76842-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="76842-109">Type</span></span>       |<span data-ttu-id="76842-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="76842-110">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="76842-111">id</span><span class="sxs-lookup"><span data-stu-id="76842-111">id</span></span>         |<span data-ttu-id="76842-112">String</span><span class="sxs-lookup"><span data-stu-id="76842-112">String</span></span>     | <span data-ttu-id="76842-113">A identificação do assunto.</span><span class="sxs-lookup"><span data-stu-id="76842-113">The id of the subject.</span></span>|
|<span data-ttu-id="76842-114">type</span><span class="sxs-lookup"><span data-stu-id="76842-114">type</span></span>       |<span data-ttu-id="76842-115">String</span><span class="sxs-lookup"><span data-stu-id="76842-115">String</span></span>     |<span data-ttu-id="76842-116">O tipo do assunto.</span><span class="sxs-lookup"><span data-stu-id="76842-116">The type of the subject.</span></span> <span data-ttu-id="76842-117">O valor pode ser ``User``, ``Group``, e ``ServicePrincipal``.</span><span class="sxs-lookup"><span data-stu-id="76842-117">The value can be ``User``, ``Group``, and ``ServicePrincipal``.</span></span>|
|<span data-ttu-id="76842-118">displayName</span><span class="sxs-lookup"><span data-stu-id="76842-118">displayName</span></span>|<span data-ttu-id="76842-119">String</span><span class="sxs-lookup"><span data-stu-id="76842-119">String</span></span>     |<span data-ttu-id="76842-120">O nome de exibição do assunto.</span><span class="sxs-lookup"><span data-stu-id="76842-120">The display name of the subject.</span></span>|
|<span data-ttu-id="76842-121">email</span><span class="sxs-lookup"><span data-stu-id="76842-121">email</span></span>      |<span data-ttu-id="76842-122">String</span><span class="sxs-lookup"><span data-stu-id="76842-122">String</span></span>     |<span data-ttu-id="76842-123">O endereço de email da entidade do usuário.</span><span class="sxs-lookup"><span data-stu-id="76842-123">The email address of the user subject.</span></span> <span data-ttu-id="76842-124">Se o assunto estiver em outros tipos, está vazio.</span><span class="sxs-lookup"><span data-stu-id="76842-124">If the subject is in other types, it is empty.</span></span>|
|<span data-ttu-id="76842-125">principalName</span><span class="sxs-lookup"><span data-stu-id="76842-125">principalName</span></span>|<span data-ttu-id="76842-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="76842-126">String</span></span>   |<span data-ttu-id="76842-127">O nome principal da entidade do usuário.</span><span class="sxs-lookup"><span data-stu-id="76842-127">The principal name of the user subject.</span></span> <span data-ttu-id="76842-128">Se o assunto estiver em outros tipos, está vazio.</span><span class="sxs-lookup"><span data-stu-id="76842-128">If the subject is in other types, it is empty.</span></span>|

## <a name="relationships"></a><span data-ttu-id="76842-129">Relações</span><span class="sxs-lookup"><span data-stu-id="76842-129">Relationships</span></span>
<span data-ttu-id="76842-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="76842-130">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="76842-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="76842-131">JSON representation</span></span>

<span data-ttu-id="76842-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="76842-132">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "governanceSubject",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->