---
title: tipo de recurso rbacApplication
description: Propriedade de navegação gerenciamento de função
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e7145509745bdb696ebe3342035096af27d89b38
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47993046"
---
# <a name="rbacapplication-resource-type"></a><span data-ttu-id="1480b-103">tipo de recurso rbacApplication</span><span class="sxs-lookup"><span data-stu-id="1480b-103">rbacApplication resource type</span></span>

<span data-ttu-id="1480b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1480b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1480b-105">Contêiner de gerenciamento de função para definições de função unificadas e atribuições de função para provedores Microsoft 365 RBAC.</span><span class="sxs-lookup"><span data-stu-id="1480b-105">Role management container for unified role definitions and role assignments for Microsoft 365 RBAC providers.</span></span> <span data-ttu-id="1480b-106">Atualmente, "Directory" é o único aplicativo RBAC compatível.</span><span class="sxs-lookup"><span data-stu-id="1480b-106">Currently "directory" is the only RBAC application supported.</span></span>

## <a name="methods"></a><span data-ttu-id="1480b-107">Methods</span><span class="sxs-lookup"><span data-stu-id="1480b-107">Methods</span></span>

| <span data-ttu-id="1480b-108">Método</span><span class="sxs-lookup"><span data-stu-id="1480b-108">Method</span></span>       | <span data-ttu-id="1480b-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1480b-109">Return Type</span></span> | <span data-ttu-id="1480b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1480b-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="1480b-111">Criar unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="1480b-111">Create unifiedRoleAssignment</span></span>](../api/rbacapplication-post-roleassignments.md) | [<span data-ttu-id="1480b-112">unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="1480b-112">unifiedRoleAssignment</span></span>](unifiedroleassignment.md) | <span data-ttu-id="1480b-113">Crie um novo unifiedRoleAssignment postando na coleção roleAssignments.</span><span class="sxs-lookup"><span data-stu-id="1480b-113">Create a new unifiedRoleAssignment by posting to the roleAssignments collection.</span></span> |
| [<span data-ttu-id="1480b-114">Listar roleAssignments</span><span class="sxs-lookup"><span data-stu-id="1480b-114">List roleAssignments</span></span>](../api/rbacapplication-list-roleassignments.md) | <span data-ttu-id="1480b-115">coleção [unifiedRoleAssignment](unifiedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="1480b-115">[unifiedRoleAssignment](unifiedroleassignment.md) collection</span></span> | <span data-ttu-id="1480b-116">Obtenha uma coleção de objetos unifiedRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="1480b-116">Get a unifiedRoleAssignment object collection.</span></span> <span data-ttu-id="1480b-117">Somente instâncias específicas podem ser consultadas, por meio da filtragem em roleDefitionId ou entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="1480b-117">Only specific instances can be queried, by filtering on roleDefitionId or principalId.</span></span> |
| [<span data-ttu-id="1480b-118">Criar unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="1480b-118">Create unifiedRoleDefinition</span></span>](../api/rbacapplication-post-roledefinitions.md) | [<span data-ttu-id="1480b-119">unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="1480b-119">unifiedRoleDefinition</span></span>](unifiedroledefinition.md) | <span data-ttu-id="1480b-120">Crie um novo unifiedRoleDefinition postando na coleção roleDefinitions.</span><span class="sxs-lookup"><span data-stu-id="1480b-120">Create a new unifiedRoleDefinition by posting to the roleDefinitions collection.</span></span> |
| [<span data-ttu-id="1480b-121">Listar roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="1480b-121">List roleDefinitions</span></span>](../api/rbacapplication-list-roledefinitions.md) | <span data-ttu-id="1480b-122">coleção [unifiedRoleDefinition](unifiedroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="1480b-122">[unifiedRoleDefinition](unifiedroledefinition.md) collection</span></span> | <span data-ttu-id="1480b-123">Obtenha uma coleção de objetos unifiedRoleDefinition.</span><span class="sxs-lookup"><span data-stu-id="1480b-123">Get a unifiedRoleDefinition object collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="1480b-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1480b-124">Properties</span></span>

<span data-ttu-id="1480b-125">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="1480b-125">None</span></span>

## <a name="relationships"></a><span data-ttu-id="1480b-126">Relações</span><span class="sxs-lookup"><span data-stu-id="1480b-126">Relationships</span></span>

<span data-ttu-id="1480b-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1480b-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1480b-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1480b-128">JSON representation</span></span>

<span data-ttu-id="1480b-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1480b-129">None</span></span>

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "rbacApplication resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


