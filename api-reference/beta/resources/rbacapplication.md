---
title: Tipo de recurso rbacApplication
description: Propriedade de navegação de gerenciamento de função
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: c3833d07e0fb9758cc8f4f5418f725889fd784dc
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760922"
---
# <a name="rbacapplication-resource-type"></a><span data-ttu-id="a928e-103">Tipo de recurso rbacApplication</span><span class="sxs-lookup"><span data-stu-id="a928e-103">rbacApplication resource type</span></span>

<span data-ttu-id="a928e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a928e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a928e-105">Contêiner de gerenciamento de função para definições unificadas de função e atribuições de função para provedores RBAC do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="a928e-105">Role management container for unified role definitions and role assignments for Microsoft 365 RBAC providers.</span></span> <span data-ttu-id="a928e-106">Atualmente, o "diretório" é o único aplicativo RBAC com suporte.</span><span class="sxs-lookup"><span data-stu-id="a928e-106">Currently "directory" is the only RBAC application supported.</span></span>

## <a name="methods"></a><span data-ttu-id="a928e-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="a928e-107">Methods</span></span>

| <span data-ttu-id="a928e-108">Método</span><span class="sxs-lookup"><span data-stu-id="a928e-108">Method</span></span>       | <span data-ttu-id="a928e-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a928e-109">Return Type</span></span> | <span data-ttu-id="a928e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a928e-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="a928e-111">Criar unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="a928e-111">Create unifiedRoleAssignment</span></span>](../api/rbacapplication-post-roleassignments.md) | [<span data-ttu-id="a928e-112">unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="a928e-112">unifiedRoleAssignment</span></span>](unifiedroleassignment.md) | <span data-ttu-id="a928e-113">Crie um novo unifiedRoleAssignment postando na coleção roleAssignments.</span><span class="sxs-lookup"><span data-stu-id="a928e-113">Create a new unifiedRoleAssignment by posting to the roleAssignments collection.</span></span> |
| [<span data-ttu-id="a928e-114">Listar roleAssignments</span><span class="sxs-lookup"><span data-stu-id="a928e-114">List roleAssignments</span></span>](../api/rbacapplication-list-roleassignments.md) | <span data-ttu-id="a928e-115">[Coleção unifiedRoleAssignment](unifiedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="a928e-115">[unifiedRoleAssignment](unifiedroleassignment.md) collection</span></span> | <span data-ttu-id="a928e-116">Obter uma coleção de objetos unifiedRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="a928e-116">Get a unifiedRoleAssignment object collection.</span></span> <span data-ttu-id="a928e-117">Somente instâncias específicas podem ser consultadas, filtrando-se roleDefitionId ou principalId.</span><span class="sxs-lookup"><span data-stu-id="a928e-117">Only specific instances can be queried, by filtering on roleDefitionId or principalId.</span></span> |
| [<span data-ttu-id="a928e-118">Criar unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="a928e-118">Create unifiedRoleDefinition</span></span>](../api/rbacapplication-post-roledefinitions.md) | [<span data-ttu-id="a928e-119">unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="a928e-119">unifiedRoleDefinition</span></span>](unifiedroledefinition.md) | <span data-ttu-id="a928e-120">Crie um novo unifiedRoleDefinition postando na coleção roleDefinitions.</span><span class="sxs-lookup"><span data-stu-id="a928e-120">Create a new unifiedRoleDefinition by posting to the roleDefinitions collection.</span></span> |
| [<span data-ttu-id="a928e-121">Listar roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="a928e-121">List roleDefinitions</span></span>](../api/rbacapplication-list-roledefinitions.md) | <span data-ttu-id="a928e-122">[Coleção unifiedRoleDefinition](unifiedroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="a928e-122">[unifiedRoleDefinition](unifiedroledefinition.md) collection</span></span> | <span data-ttu-id="a928e-123">Obter uma coleção de objetos unifiedRoleDefinition.</span><span class="sxs-lookup"><span data-stu-id="a928e-123">Get a unifiedRoleDefinition object collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="a928e-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a928e-124">Properties</span></span>

<span data-ttu-id="a928e-125">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="a928e-125">None</span></span>

## <a name="relationships"></a><span data-ttu-id="a928e-126">Relações</span><span class="sxs-lookup"><span data-stu-id="a928e-126">Relationships</span></span>

<span data-ttu-id="a928e-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a928e-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a928e-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a928e-128">JSON representation</span></span>

<span data-ttu-id="a928e-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a928e-129">None</span></span>

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "rbacApplication resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


