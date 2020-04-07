---
title: tipo de recurso appScope
description: 'O escopo de uma atribuição de função determina o conjunto de recursos para o qual a entidade de segurança recebeu acesso. Um escopo de aplicativo é um escopo definido e compreendido por um aplicativo específico. O outro tipo de escopo é o escopo de diretório. Escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos. '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4a996b219df124ac0c287ed4ed32658584acb6ac
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/07/2020
ms.locfileid: "43160349"
---
# <a name="appscope-resource-type"></a><span data-ttu-id="8e6c6-106">tipo de recurso appScope</span><span class="sxs-lookup"><span data-stu-id="8e6c6-106">appScope resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8e6c6-107">O escopo de uma atribuição de função determina o conjunto de recursos para o qual a entidade de segurança recebeu acesso.</span><span class="sxs-lookup"><span data-stu-id="8e6c6-107">The scope of a role assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="8e6c6-108">Um escopo de aplicativo é um escopo definido e compreendido por um aplicativo específico.</span><span class="sxs-lookup"><span data-stu-id="8e6c6-108">An app scope is a scope defined and understood by a specific application.</span></span> <span data-ttu-id="8e6c6-109">O outro tipo de escopo é o escopo de diretório.</span><span class="sxs-lookup"><span data-stu-id="8e6c6-109">The other type of scope is directory scope.</span></span> <span data-ttu-id="8e6c6-110">Escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos.</span><span class="sxs-lookup"><span data-stu-id="8e6c6-110">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> 

<span data-ttu-id="8e6c6-111">Isso é empregado na entidade single principal, de escopo único e em várias entidades de escopo múltiplo.</span><span class="sxs-lookup"><span data-stu-id="8e6c6-111">This is employed in both the single principal, single scope entity and multiple principal, multiple scope entities.</span></span>

## <a name="methods"></a><span data-ttu-id="8e6c6-112">Métodos</span><span class="sxs-lookup"><span data-stu-id="8e6c6-112">Methods</span></span>
<span data-ttu-id="8e6c6-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8e6c6-113">None</span></span>

## <a name="properties"></a><span data-ttu-id="8e6c6-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8e6c6-114">Properties</span></span>

| <span data-ttu-id="8e6c6-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8e6c6-115">Property</span></span> | <span data-ttu-id="8e6c6-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="8e6c6-116">Type</span></span> | <span data-ttu-id="8e6c6-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e6c6-117">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="8e6c6-118">id</span><span class="sxs-lookup"><span data-stu-id="8e6c6-118">id</span></span> | <span data-ttu-id="8e6c6-119">string</span><span class="sxs-lookup"><span data-stu-id="8e6c6-119">string</span></span> | <span data-ttu-id="8e6c6-120">ID de um contêiner ou recurso específico do aplicativo que representa o escopo da atribuição.</span><span class="sxs-lookup"><span data-stu-id="8e6c6-120">Id of an app-specific container or resource representing the scope of the assignment.</span></span> <span data-ttu-id="8e6c6-121">Geralmente a ID imutável do recurso.</span><span class="sxs-lookup"><span data-stu-id="8e6c6-121">Usually the immutable id of the resource.</span></span> <span data-ttu-id="8e6c6-122">O escopo de uma atribuição determina o conjunto de recursos para o qual a entidade recebeu acesso.</span><span class="sxs-lookup"><span data-stu-id="8e6c6-122">The scope of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="8e6c6-123">Essa propriedade é obrigatória.</span><span class="sxs-lookup"><span data-stu-id="8e6c6-123">This property is required.</span></span> |
| <span data-ttu-id="8e6c6-124">type</span><span class="sxs-lookup"><span data-stu-id="8e6c6-124">type</span></span> | <span data-ttu-id="8e6c6-125">String</span><span class="sxs-lookup"><span data-stu-id="8e6c6-125">String</span></span> | <span data-ttu-id="8e6c6-126">Descreve o tipo de recurso específico do aplicativo representado pelo escopo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8e6c6-126">Describes the type of app-specific resource represented by the app scope.</span></span> <span data-ttu-id="8e6c6-127">Fornecido para fins de exibição, de forma que uma interface do usuário possa transmitir ao usuário o tipo de recurso específico do aplicativo representado pelo escopo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8e6c6-127">Provided for display purposes, so a user interface can convey to the user the kind of app specific resource represented by the app scope.</span></span> <span data-ttu-id="8e6c6-128">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e6c6-128">This property is read only.</span></span> |
| <span data-ttu-id="8e6c6-129">displayName</span><span class="sxs-lookup"><span data-stu-id="8e6c6-129">displayName</span></span> | <span data-ttu-id="8e6c6-130">string</span><span class="sxs-lookup"><span data-stu-id="8e6c6-130">string</span></span> | <span data-ttu-id="8e6c6-131">Fornece o nome de exibição do recurso específico do aplicativo representado pelo escopo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8e6c6-131">Provides the display name of the app-specific resource represented by the app scope.</span></span> <span data-ttu-id="8e6c6-132">Fornecido para fins de exibição, já que appScopeId é geralmente uma ID imutável inalterável e não humanamente legível. Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e6c6-132">Provided for display purposes since appScopeId is often an immutable, non-human-readable id. This property is read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="8e6c6-133">Relações</span><span class="sxs-lookup"><span data-stu-id="8e6c6-133">Relationships</span></span>

<span data-ttu-id="8e6c6-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8e6c6-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8e6c6-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8e6c6-135">JSON representation</span></span>

<span data-ttu-id="8e6c6-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8e6c6-136">The following is a JSON representation of the resource.</span></span>

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