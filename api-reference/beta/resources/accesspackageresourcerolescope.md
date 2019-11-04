---
title: tipo de recurso accessPackageResourceRoleScope
description: Um escopo de função de recurso de pacote do Access é uma referência a um escopo dentro de um recurso e uma função nesse recurso.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d4f10d297e59f9665d493060362a27e1c4b11a5a
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938909"
---
# <a name="accesspackageresourcerolescope-resource-type"></a><span data-ttu-id="21b60-103">tipo de recurso accessPackageResourceRoleScope</span><span class="sxs-lookup"><span data-stu-id="21b60-103">accessPackageResourceRoleScope resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="21b60-104">No [Azure ad pretitulation Management](entitlementmanagement-root.md), um escopo de função de recurso de pacote do Access é uma referência a um escopo dentro de um recurso e uma função nesse recurso.</span><span class="sxs-lookup"><span data-stu-id="21b60-104">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource role scope is a reference to both a scope within a resource, and a role in that resource.</span></span>

## <a name="properties"></a><span data-ttu-id="21b60-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="21b60-105">Properties</span></span>

| <span data-ttu-id="21b60-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="21b60-106">Property</span></span>     | <span data-ttu-id="21b60-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="21b60-107">Type</span></span>        | <span data-ttu-id="21b60-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="21b60-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="21b60-109">createdBy</span><span class="sxs-lookup"><span data-stu-id="21b60-109">createdBy</span></span>|<span data-ttu-id="21b60-110">String</span><span class="sxs-lookup"><span data-stu-id="21b60-110">String</span></span>|<span data-ttu-id="21b60-111">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="21b60-111">Read-only.</span></span>|
|<span data-ttu-id="21b60-112">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="21b60-112">createdDateTime</span></span>|<span data-ttu-id="21b60-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21b60-113">DateTimeOffset</span></span>|<span data-ttu-id="21b60-p101">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="21b60-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="21b60-116">id</span><span class="sxs-lookup"><span data-stu-id="21b60-116">id</span></span>|<span data-ttu-id="21b60-117">String</span><span class="sxs-lookup"><span data-stu-id="21b60-117">String</span></span>| <span data-ttu-id="21b60-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="21b60-118">Read-only.</span></span>|
|<span data-ttu-id="21b60-119">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="21b60-119">modifiedBy</span></span>|<span data-ttu-id="21b60-120">String</span><span class="sxs-lookup"><span data-stu-id="21b60-120">String</span></span>|<span data-ttu-id="21b60-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="21b60-121">Read-only.</span></span>|
|<span data-ttu-id="21b60-122">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="21b60-122">modifiedDateTime</span></span>|<span data-ttu-id="21b60-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21b60-123">DateTimeOffset</span></span>|<span data-ttu-id="21b60-p102">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="21b60-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="21b60-126">Relações</span><span class="sxs-lookup"><span data-stu-id="21b60-126">Relationships</span></span>

| <span data-ttu-id="21b60-127">Relação</span><span class="sxs-lookup"><span data-stu-id="21b60-127">Relationship</span></span> | <span data-ttu-id="21b60-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="21b60-128">Type</span></span>        | <span data-ttu-id="21b60-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="21b60-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="21b60-130">accessPackageResourceRole</span><span class="sxs-lookup"><span data-stu-id="21b60-130">accessPackageResourceRole</span></span>|[<span data-ttu-id="21b60-131">accessPackageResourceRole</span><span class="sxs-lookup"><span data-stu-id="21b60-131">accessPackageResourceRole</span></span>](accesspackageresourcerole.md)| <span data-ttu-id="21b60-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="21b60-132">Read-only.</span></span> <span data-ttu-id="21b60-133">Anulável.</span><span class="sxs-lookup"><span data-stu-id="21b60-133">Nullable.</span></span>|
|<span data-ttu-id="21b60-134">accessPackageResourceScope</span><span class="sxs-lookup"><span data-stu-id="21b60-134">accessPackageResourceScope</span></span>|[<span data-ttu-id="21b60-135">accessPackageResourceScope</span><span class="sxs-lookup"><span data-stu-id="21b60-135">accessPackageResourceScope</span></span>](accesspackageresourcescope.md)| <span data-ttu-id="21b60-p104">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="21b60-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="21b60-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="21b60-138">JSON representation</span></span>

<span data-ttu-id="21b60-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="21b60-139">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageResourceRoleScope",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "createdBy": "String",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "modifiedBy": "String",
  "modifiedDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageResourceRoleScope resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
