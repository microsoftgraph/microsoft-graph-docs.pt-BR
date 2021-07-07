---
title: Tipo de recurso rbacApplication
description: Propriedade de navegação de gerenciamento de função
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 9636f113222bbbe6a754c2977e08273d140a6086
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2021
ms.locfileid: "53317193"
---
# <a name="rbacapplication-resource-type"></a><span data-ttu-id="3b9da-103">Tipo de recurso rbacApplication</span><span class="sxs-lookup"><span data-stu-id="3b9da-103">rbacApplication resource type</span></span>

<span data-ttu-id="3b9da-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b9da-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3b9da-105">Contêiner de gerenciamento de função para definições de função unificadas e atribuições de função para Microsoft 365 provedores RBAC.</span><span class="sxs-lookup"><span data-stu-id="3b9da-105">Role management container for unified role definitions and role assignments for Microsoft 365 RBAC providers.</span></span> <span data-ttu-id="3b9da-106">Atualmente, o gerenciamento de diretórios e direitos são os únicos aplicativos RBAC com suporte.</span><span class="sxs-lookup"><span data-stu-id="3b9da-106">Currently directory and entitlement management are the only RBAC applications supported.</span></span>

## <a name="methods"></a><span data-ttu-id="3b9da-107">Methods</span><span class="sxs-lookup"><span data-stu-id="3b9da-107">Methods</span></span>

| <span data-ttu-id="3b9da-108">Método</span><span class="sxs-lookup"><span data-stu-id="3b9da-108">Method</span></span>       | <span data-ttu-id="3b9da-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3b9da-109">Return Type</span></span> | <span data-ttu-id="3b9da-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3b9da-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="3b9da-111">Criar unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="3b9da-111">Create unifiedRoleAssignment</span></span>](../api/rbacapplication-post-roleassignments.md) | [<span data-ttu-id="3b9da-112">unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="3b9da-112">unifiedRoleAssignment</span></span>](unifiedroleassignment.md) | <span data-ttu-id="3b9da-113">Crie um novo unifiedRoleAssignment postando na coleção roleAssignments.</span><span class="sxs-lookup"><span data-stu-id="3b9da-113">Create a new unifiedRoleAssignment by posting to the roleAssignments collection.</span></span> |
| [<span data-ttu-id="3b9da-114">Listar roleAssignments</span><span class="sxs-lookup"><span data-stu-id="3b9da-114">List roleAssignments</span></span>](../api/rbacapplication-list-roleassignments.md) | <span data-ttu-id="3b9da-115">[Coleção unifiedRoleAssignment](unifiedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="3b9da-115">[unifiedRoleAssignment](unifiedroleassignment.md) collection</span></span> | <span data-ttu-id="3b9da-116">Obter uma coleção de objetos unifiedRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="3b9da-116">Get a unifiedRoleAssignment object collection.</span></span> <span data-ttu-id="3b9da-117">Somente instâncias específicas podem ser consultadas, filtrando-se roleDefitionId ou principalId.</span><span class="sxs-lookup"><span data-stu-id="3b9da-117">Only specific instances can be queried, by filtering on roleDefitionId or principalId.</span></span> |
| [<span data-ttu-id="3b9da-118">Criar unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="3b9da-118">Create unifiedRoleDefinition</span></span>](../api/rbacapplication-post-roledefinitions.md) | [<span data-ttu-id="3b9da-119">unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="3b9da-119">unifiedRoleDefinition</span></span>](unifiedroledefinition.md) | <span data-ttu-id="3b9da-120">Crie um novo unifiedRoleDefinition postando na coleção roleDefinitions.</span><span class="sxs-lookup"><span data-stu-id="3b9da-120">Create a new unifiedRoleDefinition by posting to the roleDefinitions collection.</span></span> |
| [<span data-ttu-id="3b9da-121">Listar roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="3b9da-121">List roleDefinitions</span></span>](../api/rbacapplication-list-roledefinitions.md) | <span data-ttu-id="3b9da-122">[Coleção unifiedRoleDefinition](unifiedroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="3b9da-122">[unifiedRoleDefinition](unifiedroledefinition.md) collection</span></span> | <span data-ttu-id="3b9da-123">Obter uma coleção de objetos unifiedRoleDefinition.</span><span class="sxs-lookup"><span data-stu-id="3b9da-123">Get a unifiedRoleDefinition object collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="3b9da-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3b9da-124">Properties</span></span>

<span data-ttu-id="3b9da-125">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="3b9da-125">None</span></span>

## <a name="relationships"></a><span data-ttu-id="3b9da-126">Relações</span><span class="sxs-lookup"><span data-stu-id="3b9da-126">Relationships</span></span>

<span data-ttu-id="3b9da-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3b9da-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3b9da-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3b9da-128">JSON representation</span></span>

<span data-ttu-id="3b9da-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3b9da-129">None</span></span>

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "rbacApplication resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


