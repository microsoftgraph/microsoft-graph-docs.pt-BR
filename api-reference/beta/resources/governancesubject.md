---
title: tipo de recurso governanceSubject
description: Representa usuários, grupos e entidades de serviço que estão sendo gerenciados no gerenciamento de identidade privilegiada (PIM).
localization_priority: Normal
ms.openlocfilehash: a83825a147429c81b3e83b2f2fb384672d2f527e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506424"
---
# <a name="governancesubject-resource-type"></a><span data-ttu-id="e1e2c-103">tipo de recurso governanceSubject</span><span class="sxs-lookup"><span data-stu-id="e1e2c-103">governanceSubject resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1e2c-104">Representa usuários, grupos e entidades de serviço que estão sendo gerenciados no gerenciamento de identidade privilegiada (PIM).</span><span class="sxs-lookup"><span data-stu-id="e1e2c-104">Represents users, groups, and service principals being managed in Privileged Identity Management (PIM).</span></span>


## <a name="properties"></a><span data-ttu-id="e1e2c-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e1e2c-105">Properties</span></span>
| <span data-ttu-id="e1e2c-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e1e2c-106">Property</span></span>  | <span data-ttu-id="e1e2c-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="e1e2c-107">Type</span></span>       |<span data-ttu-id="e1e2c-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1e2c-108">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="e1e2c-109">id</span><span class="sxs-lookup"><span data-stu-id="e1e2c-109">id</span></span>         |<span data-ttu-id="e1e2c-110">String</span><span class="sxs-lookup"><span data-stu-id="e1e2c-110">String</span></span>     | <span data-ttu-id="e1e2c-111">A ID do assunto.</span><span class="sxs-lookup"><span data-stu-id="e1e2c-111">The id of the subject.</span></span>|
|<span data-ttu-id="e1e2c-112">type</span><span class="sxs-lookup"><span data-stu-id="e1e2c-112">type</span></span>       |<span data-ttu-id="e1e2c-113">String</span><span class="sxs-lookup"><span data-stu-id="e1e2c-113">String</span></span>     |<span data-ttu-id="e1e2c-114">O tipo do assunto.</span><span class="sxs-lookup"><span data-stu-id="e1e2c-114">The type of the subject.</span></span> <span data-ttu-id="e1e2c-115">O valor pode ser ``User``, ``Group``e ``ServicePrincipal``.</span><span class="sxs-lookup"><span data-stu-id="e1e2c-115">The value can be ``User``, ``Group``, and ``ServicePrincipal``.</span></span>|
|<span data-ttu-id="e1e2c-116">displayName</span><span class="sxs-lookup"><span data-stu-id="e1e2c-116">displayName</span></span>|<span data-ttu-id="e1e2c-117">String</span><span class="sxs-lookup"><span data-stu-id="e1e2c-117">String</span></span>     |<span data-ttu-id="e1e2c-118">O nome de exibição do assunto.</span><span class="sxs-lookup"><span data-stu-id="e1e2c-118">The display name of the subject.</span></span>|
|<span data-ttu-id="e1e2c-119">email</span><span class="sxs-lookup"><span data-stu-id="e1e2c-119">email</span></span>      |<span data-ttu-id="e1e2c-120">String</span><span class="sxs-lookup"><span data-stu-id="e1e2c-120">String</span></span>     |<span data-ttu-id="e1e2c-121">O endereço de email do assunto do usuário.</span><span class="sxs-lookup"><span data-stu-id="e1e2c-121">The email address of the user subject.</span></span> <span data-ttu-id="e1e2c-122">Se o assunto estiver em outros tipos, ele estará vazio.</span><span class="sxs-lookup"><span data-stu-id="e1e2c-122">If the subject is in other types, it is empty.</span></span>|
|<span data-ttu-id="e1e2c-123">principalName</span><span class="sxs-lookup"><span data-stu-id="e1e2c-123">principalName</span></span>|<span data-ttu-id="e1e2c-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e1e2c-124">String</span></span>   |<span data-ttu-id="e1e2c-125">O nome da entidade de segurança do usuário.</span><span class="sxs-lookup"><span data-stu-id="e1e2c-125">The principal name of the user subject.</span></span> <span data-ttu-id="e1e2c-126">Se o assunto estiver em outros tipos, ele estará vazio.</span><span class="sxs-lookup"><span data-stu-id="e1e2c-126">If the subject is in other types, it is empty.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e1e2c-127">Relações</span><span class="sxs-lookup"><span data-stu-id="e1e2c-127">Relationships</span></span>
<span data-ttu-id="e1e2c-128">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="e1e2c-128">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="e1e2c-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e1e2c-129">JSON representation</span></span>

<span data-ttu-id="e1e2c-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e1e2c-130">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/governancesubject.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
