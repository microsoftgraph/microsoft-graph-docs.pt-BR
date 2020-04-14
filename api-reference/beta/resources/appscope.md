---
title: tipo de recurso appScope
description: Um escopo de aplicativo é um escopo definido e compreendido por um aplicativo específico.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 23a3d18a8a712ddff8470d91a677f3d0f18dabf2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43459332"
---
# <a name="appscope-resource-type"></a><span data-ttu-id="f8186-103">tipo de recurso appScope</span><span class="sxs-lookup"><span data-stu-id="f8186-103">appScope resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f8186-104">O escopo de uma atribuição de função determina o conjunto de recursos para o qual a entidade de segurança recebeu acesso.</span><span class="sxs-lookup"><span data-stu-id="f8186-104">The scope of a role assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="f8186-105">Um escopo de aplicativo é um escopo definido e compreendido por um aplicativo específico.</span><span class="sxs-lookup"><span data-stu-id="f8186-105">An app scope is a scope defined and understood by a specific application.</span></span> <span data-ttu-id="f8186-106">O outro tipo de escopo é o escopo de diretório.</span><span class="sxs-lookup"><span data-stu-id="f8186-106">The other type of scope is directory scope.</span></span> <span data-ttu-id="f8186-107">Escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos.</span><span class="sxs-lookup"><span data-stu-id="f8186-107">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> 

<span data-ttu-id="f8186-108">Isso é empregado na entidade single principal, de escopo único e em várias entidades de escopo múltiplo.</span><span class="sxs-lookup"><span data-stu-id="f8186-108">This is employed in both the single principal, single scope entity and multiple principal, multiple scope entities.</span></span>

## <a name="methods"></a><span data-ttu-id="f8186-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="f8186-109">Methods</span></span>
<span data-ttu-id="f8186-110">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f8186-110">None</span></span>

## <a name="properties"></a><span data-ttu-id="f8186-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f8186-111">Properties</span></span>

| <span data-ttu-id="f8186-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f8186-112">Property</span></span> | <span data-ttu-id="f8186-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="f8186-113">Type</span></span> | <span data-ttu-id="f8186-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="f8186-114">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="f8186-115">id</span><span class="sxs-lookup"><span data-stu-id="f8186-115">id</span></span> | <span data-ttu-id="f8186-116">string</span><span class="sxs-lookup"><span data-stu-id="f8186-116">string</span></span> | <span data-ttu-id="f8186-117">ID de um contêiner ou recurso específico do aplicativo que representa o escopo da atribuição.</span><span class="sxs-lookup"><span data-stu-id="f8186-117">Id of an app-specific container or resource representing the scope of the assignment.</span></span> <span data-ttu-id="f8186-118">Geralmente a ID imutável do recurso.</span><span class="sxs-lookup"><span data-stu-id="f8186-118">Usually the immutable id of the resource.</span></span> <span data-ttu-id="f8186-119">O escopo de uma atribuição determina o conjunto de recursos para o qual a entidade recebeu acesso.</span><span class="sxs-lookup"><span data-stu-id="f8186-119">The scope of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="f8186-120">Essa propriedade é obrigatória.</span><span class="sxs-lookup"><span data-stu-id="f8186-120">This property is required.</span></span> |
| <span data-ttu-id="f8186-121">type</span><span class="sxs-lookup"><span data-stu-id="f8186-121">type</span></span> | <span data-ttu-id="f8186-122">String</span><span class="sxs-lookup"><span data-stu-id="f8186-122">String</span></span> | <span data-ttu-id="f8186-123">Descreve o tipo de recurso específico do aplicativo representado pelo escopo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f8186-123">Describes the type of app-specific resource represented by the app scope.</span></span> <span data-ttu-id="f8186-124">Fornecido para fins de exibição, de forma que uma interface do usuário possa transmitir ao usuário o tipo de recurso específico do aplicativo representado pelo escopo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f8186-124">Provided for display purposes, so a user interface can convey to the user the kind of app specific resource represented by the app scope.</span></span> <span data-ttu-id="f8186-125">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f8186-125">This property is read only.</span></span> |
| <span data-ttu-id="f8186-126">displayName</span><span class="sxs-lookup"><span data-stu-id="f8186-126">displayName</span></span> | <span data-ttu-id="f8186-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f8186-127">string</span></span> | <span data-ttu-id="f8186-128">Fornece o nome de exibição do recurso específico do aplicativo representado pelo escopo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f8186-128">Provides the display name of the app-specific resource represented by the app scope.</span></span> <span data-ttu-id="f8186-129">Fornecido para fins de exibição, já que appScopeId é geralmente uma ID imutável inalterável e não humanamente legível. Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f8186-129">Provided for display purposes since appScopeId is often an immutable, non-human-readable id. This property is read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="f8186-130">Relações</span><span class="sxs-lookup"><span data-stu-id="f8186-130">Relationships</span></span>

<span data-ttu-id="f8186-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f8186-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f8186-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f8186-132">JSON representation</span></span>

<span data-ttu-id="f8186-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f8186-133">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.appScope"
}-->

```json
{
  "id": "String (identifier)",
  "type": "String",
  "displayName": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "appScope resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->