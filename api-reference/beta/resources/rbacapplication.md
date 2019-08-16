---
title: tipo de recurso rbacApplication
description: Propriedade de navegação gerenciamento de função
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: afcef3766e4df80a3856ab59684ba826c3a78d14
ms.sourcegitcommit: 567d0420243765b4088bc8029306a517f92926fd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/16/2019
ms.locfileid: "36437822"
---
# <a name="rbacapplication-resource-type"></a><span data-ttu-id="c6767-103">tipo de recurso rbacApplication</span><span class="sxs-lookup"><span data-stu-id="c6767-103">rbacApplication resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c6767-104">Contêiner de gerenciamento de função para definições de função unificadas e atribuições de função para provedores Microsoft 365 RBAC.</span><span class="sxs-lookup"><span data-stu-id="c6767-104">Role management container for unified role definitions and role assignments for Microsoft 365 RBAC providers.</span></span> <span data-ttu-id="c6767-105">Atualmente, "Directory" é o único aplicativo RBAC compatível.</span><span class="sxs-lookup"><span data-stu-id="c6767-105">Currently "directory" is the only RBAC application supported.</span></span>

## <a name="methods"></a><span data-ttu-id="c6767-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="c6767-106">Methods</span></span>

| <span data-ttu-id="c6767-107">Método</span><span class="sxs-lookup"><span data-stu-id="c6767-107">Method</span></span>       | <span data-ttu-id="c6767-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c6767-108">Return Type</span></span> | <span data-ttu-id="c6767-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6767-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="c6767-110">Criar unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="c6767-110">Create unifiedRoleAssignment</span></span>](../api/rbacapplication-post-roleassignments.md) | [<span data-ttu-id="c6767-111">unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="c6767-111">unifiedRoleAssignment</span></span>](unifiedroleassignment.md) | <span data-ttu-id="c6767-112">Crie um novo unifiedRoleAssignment postando na coleção roleAssignments.</span><span class="sxs-lookup"><span data-stu-id="c6767-112">Create a new unifiedRoleAssignment by posting to the roleAssignments collection.</span></span> |
| [<span data-ttu-id="c6767-113">Listar roleAssignments</span><span class="sxs-lookup"><span data-stu-id="c6767-113">List roleAssignments</span></span>](../api/rbacapplication-list-roleassignments.md) | <span data-ttu-id="c6767-114">coleção [unifiedRoleAssignment](unifiedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c6767-114">[unifiedRoleAssignment](unifiedroleassignment.md) collection</span></span> | <span data-ttu-id="c6767-115">Obtenha uma coleção de objetos unifiedRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="c6767-115">Get a unifiedRoleAssignment object collection.</span></span> <span data-ttu-id="c6767-116">Somente instâncias específicas podem ser consultadas, por meio da filtragem em unifiedRoleDefitionId ou entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="c6767-116">Only specific instances can be queried, by filtering on unifiedRoleDefitionId or principalId.</span></span> |
| [<span data-ttu-id="c6767-117">Criar unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="c6767-117">Create unifiedRoleDefinition</span></span>](../api/rbacapplication-post-roledefinitions.md) | [<span data-ttu-id="c6767-118">unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="c6767-118">unifiedRoleDefinition</span></span>](unifiedroledefinition.md) | <span data-ttu-id="c6767-119">Crie um novo unifiedRoleDefinition postando na coleção roleDefinitions.</span><span class="sxs-lookup"><span data-stu-id="c6767-119">Create a new unifiedRoleDefinition by posting to the roleDefinitions collection.</span></span> |
| [<span data-ttu-id="c6767-120">Listar roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="c6767-120">List roleDefinitions</span></span>](../api/rbacapplication-list-roledefinitions.md) | <span data-ttu-id="c6767-121">coleção [unifiedRoleDefinition](unifiedroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="c6767-121">[unifiedRoleDefinition](unifiedroledefinition.md) collection</span></span> | <span data-ttu-id="c6767-122">Obtenha uma coleção de objetos unifiedRoleDefinition.</span><span class="sxs-lookup"><span data-stu-id="c6767-122">Get a unifiedRoleDefinition object collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="c6767-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c6767-123">Properties</span></span>

<span data-ttu-id="c6767-124">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="c6767-124">None</span></span>

## <a name="relationships"></a><span data-ttu-id="c6767-125">Relações</span><span class="sxs-lookup"><span data-stu-id="c6767-125">Relationships</span></span>

<span data-ttu-id="c6767-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c6767-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c6767-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c6767-127">JSON representation</span></span>

<span data-ttu-id="c6767-128">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="c6767-128">None</span></span>

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "rbacApplication resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
