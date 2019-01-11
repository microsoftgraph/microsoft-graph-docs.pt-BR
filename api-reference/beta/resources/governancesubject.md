---
title: tipo de recurso de governanceSubject
description: Representa os usuários, grupos e entidades de serviço estão sendo gerenciadas no gerenciamento de identidade privilegiado (PIM).
localization_priority: Normal
ms.openlocfilehash: f3f8762c9136a3ae92269f6c06f52000fb73f710
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832587"
---
# <a name="governancesubject-resource-type"></a><span data-ttu-id="328e6-103">tipo de recurso de governanceSubject</span><span class="sxs-lookup"><span data-stu-id="328e6-103">governanceSubject resource type</span></span>

> <span data-ttu-id="328e6-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="328e6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="328e6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="328e6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="328e6-106">Representa os usuários, grupos e entidades de serviço estão sendo gerenciadas no gerenciamento de identidade privilegiado (PIM).</span><span class="sxs-lookup"><span data-stu-id="328e6-106">Represents users, groups, and service principals being managed in Privileged Identity Management (PIM).</span></span>


## <a name="properties"></a><span data-ttu-id="328e6-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="328e6-107">Properties</span></span>
| <span data-ttu-id="328e6-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="328e6-108">Property</span></span>  | <span data-ttu-id="328e6-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="328e6-109">Type</span></span>       |<span data-ttu-id="328e6-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="328e6-110">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="328e6-111">id</span><span class="sxs-lookup"><span data-stu-id="328e6-111">id</span></span>         |<span data-ttu-id="328e6-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="328e6-112">String</span></span>     | <span data-ttu-id="328e6-113">A identificação do assunto.</span><span class="sxs-lookup"><span data-stu-id="328e6-113">The id of the subject.</span></span>|
|<span data-ttu-id="328e6-114">type</span><span class="sxs-lookup"><span data-stu-id="328e6-114">type</span></span>       |<span data-ttu-id="328e6-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="328e6-115">String</span></span>     |<span data-ttu-id="328e6-116">O tipo do assunto.</span><span class="sxs-lookup"><span data-stu-id="328e6-116">The type of the subject.</span></span> <span data-ttu-id="328e6-117">O valor pode ser ``User``, ``Group``, e ``ServicePrincipal``.</span><span class="sxs-lookup"><span data-stu-id="328e6-117">The value can be ``User``, ``Group``, and ``ServicePrincipal``.</span></span>|
|<span data-ttu-id="328e6-118">displayName</span><span class="sxs-lookup"><span data-stu-id="328e6-118">displayName</span></span>|<span data-ttu-id="328e6-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="328e6-119">String</span></span>     |<span data-ttu-id="328e6-120">O nome de exibição do assunto.</span><span class="sxs-lookup"><span data-stu-id="328e6-120">The display name of the subject.</span></span>|
|<span data-ttu-id="328e6-121">email</span><span class="sxs-lookup"><span data-stu-id="328e6-121">email</span></span>      |<span data-ttu-id="328e6-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="328e6-122">String</span></span>     |<span data-ttu-id="328e6-123">O endereço de email da entidade do usuário.</span><span class="sxs-lookup"><span data-stu-id="328e6-123">The email address of the user subject.</span></span> <span data-ttu-id="328e6-124">Se o assunto estiver em outros tipos, está vazio.</span><span class="sxs-lookup"><span data-stu-id="328e6-124">If the subject is in other types, it is empty.</span></span>|
|<span data-ttu-id="328e6-125">principalName</span><span class="sxs-lookup"><span data-stu-id="328e6-125">principalName</span></span>|<span data-ttu-id="328e6-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="328e6-126">String</span></span>   |<span data-ttu-id="328e6-127">O nome principal da entidade do usuário.</span><span class="sxs-lookup"><span data-stu-id="328e6-127">The principal name of the user subject.</span></span> <span data-ttu-id="328e6-128">Se o assunto estiver em outros tipos, está vazio.</span><span class="sxs-lookup"><span data-stu-id="328e6-128">If the subject is in other types, it is empty.</span></span>|

## <a name="relationships"></a><span data-ttu-id="328e6-129">Relações</span><span class="sxs-lookup"><span data-stu-id="328e6-129">Relationships</span></span>
<span data-ttu-id="328e6-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="328e6-130">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="328e6-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="328e6-131">JSON representation</span></span>

<span data-ttu-id="328e6-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="328e6-132">Here is a JSON representation of the resource.</span></span>

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
