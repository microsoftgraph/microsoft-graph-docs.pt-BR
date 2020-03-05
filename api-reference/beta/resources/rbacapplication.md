---
title: tipo de recurso rbacApplication
description: Propriedade de navegação gerenciamento de função
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3fd03ed6bb8f3e5e3548781c29d5d9fe16fcba23
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521268"
---
# <a name="rbacapplication-resource-type"></a><span data-ttu-id="38a8d-103">tipo de recurso rbacApplication</span><span class="sxs-lookup"><span data-stu-id="38a8d-103">rbacApplication resource type</span></span>

<span data-ttu-id="38a8d-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="38a8d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38a8d-105">Contêiner de gerenciamento de função para definições de função unificadas e atribuições de função para provedores Microsoft 365 RBAC.</span><span class="sxs-lookup"><span data-stu-id="38a8d-105">Role management container for unified role definitions and role assignments for Microsoft 365 RBAC providers.</span></span> <span data-ttu-id="38a8d-106">Atualmente, "Directory" é o único aplicativo RBAC compatível.</span><span class="sxs-lookup"><span data-stu-id="38a8d-106">Currently "directory" is the only RBAC application supported.</span></span>

## <a name="methods"></a><span data-ttu-id="38a8d-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="38a8d-107">Methods</span></span>

| <span data-ttu-id="38a8d-108">Método</span><span class="sxs-lookup"><span data-stu-id="38a8d-108">Method</span></span>       | <span data-ttu-id="38a8d-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="38a8d-109">Return Type</span></span> | <span data-ttu-id="38a8d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="38a8d-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="38a8d-111">Criar unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="38a8d-111">Create unifiedRoleAssignment</span></span>](../api/rbacapplication-post-roleassignments.md) | [<span data-ttu-id="38a8d-112">unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="38a8d-112">unifiedRoleAssignment</span></span>](unifiedroleassignment.md) | <span data-ttu-id="38a8d-113">Crie um novo unifiedRoleAssignment postando na coleção roleAssignments.</span><span class="sxs-lookup"><span data-stu-id="38a8d-113">Create a new unifiedRoleAssignment by posting to the roleAssignments collection.</span></span> |
| [<span data-ttu-id="38a8d-114">Listar roleAssignments</span><span class="sxs-lookup"><span data-stu-id="38a8d-114">List roleAssignments</span></span>](../api/rbacapplication-list-roleassignments.md) | <span data-ttu-id="38a8d-115">coleção [unifiedRoleAssignment](unifiedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="38a8d-115">[unifiedRoleAssignment](unifiedroleassignment.md) collection</span></span> | <span data-ttu-id="38a8d-116">Obtenha uma coleção de objetos unifiedRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="38a8d-116">Get a unifiedRoleAssignment object collection.</span></span> <span data-ttu-id="38a8d-117">Somente instâncias específicas podem ser consultadas, por meio da filtragem em unifiedRoleDefitionId ou entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="38a8d-117">Only specific instances can be queried, by filtering on unifiedRoleDefitionId or principalId.</span></span> |
| [<span data-ttu-id="38a8d-118">Criar unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="38a8d-118">Create unifiedRoleDefinition</span></span>](../api/rbacapplication-post-roledefinitions.md) | [<span data-ttu-id="38a8d-119">unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="38a8d-119">unifiedRoleDefinition</span></span>](unifiedroledefinition.md) | <span data-ttu-id="38a8d-120">Crie um novo unifiedRoleDefinition postando na coleção roleDefinitions.</span><span class="sxs-lookup"><span data-stu-id="38a8d-120">Create a new unifiedRoleDefinition by posting to the roleDefinitions collection.</span></span> |
| [<span data-ttu-id="38a8d-121">Listar roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="38a8d-121">List roleDefinitions</span></span>](../api/rbacapplication-list-roledefinitions.md) | <span data-ttu-id="38a8d-122">coleção [unifiedRoleDefinition](unifiedroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="38a8d-122">[unifiedRoleDefinition](unifiedroledefinition.md) collection</span></span> | <span data-ttu-id="38a8d-123">Obtenha uma coleção de objetos unifiedRoleDefinition.</span><span class="sxs-lookup"><span data-stu-id="38a8d-123">Get a unifiedRoleDefinition object collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="38a8d-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="38a8d-124">Properties</span></span>

<span data-ttu-id="38a8d-125">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="38a8d-125">None</span></span>

## <a name="relationships"></a><span data-ttu-id="38a8d-126">Relações</span><span class="sxs-lookup"><span data-stu-id="38a8d-126">Relationships</span></span>

<span data-ttu-id="38a8d-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="38a8d-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="38a8d-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="38a8d-128">JSON representation</span></span>

<span data-ttu-id="38a8d-129">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="38a8d-129">None</span></span>

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "rbacApplication resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
