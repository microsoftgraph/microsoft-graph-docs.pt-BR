---
title: tipo de recurso rbacApplicationMultiple
description: Propriedade de navegação gerenciamento de função
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e7f44133050a616cac190aee5c7eeac9904f8715
ms.sourcegitcommit: 05645bc582d14781a9ca6b78ed598a4e7dc26869
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2020
ms.locfileid: "44990261"
---
# <a name="rbacapplicationmultiple-resource-type"></a><span data-ttu-id="50f63-103">tipo de recurso rbacApplicationMultiple</span><span class="sxs-lookup"><span data-stu-id="50f63-103">rbacApplicationMultiple resource type</span></span>

<span data-ttu-id="50f63-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50f63-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50f63-105">Contêiner de gerenciamento de função para definições de função unificadas e atribuições de função para provedores Microsoft 365 RBAC que oferecem suporte a várias entidades e vários escopos em uma única atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="50f63-105">Role management container for unified role definitions and role assignments for Microsoft 365 RBAC providers that support multiple principals and multiple scopes in a single role assignment.</span></span> <span data-ttu-id="50f63-106">Isso é diferente do tipo de recurso [rbacApplication](rbacapplication.md) .</span><span class="sxs-lookup"><span data-stu-id="50f63-106">This is different from [rbacApplication](rbacapplication.md) resource type.</span></span> <span data-ttu-id="50f63-107">O Microsoft Intune é um exemplo de um provedor RBAC.</span><span class="sxs-lookup"><span data-stu-id="50f63-107">Microsoft Intune is an example of such a RBAC provider.</span></span> <span data-ttu-id="50f63-108">Uma atribuição de função no Intune pode ter uma matriz de entidades e uma matriz de grupos de escopo.</span><span class="sxs-lookup"><span data-stu-id="50f63-108">A role assignment in Intune can have an array of principals and an array of scope groups.</span></span>

## <a name="methods"></a><span data-ttu-id="50f63-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="50f63-109">Methods</span></span>

| <span data-ttu-id="50f63-110">Método</span><span class="sxs-lookup"><span data-stu-id="50f63-110">Method</span></span>       | <span data-ttu-id="50f63-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="50f63-111">Return Type</span></span> | <span data-ttu-id="50f63-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="50f63-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="50f63-113">Criar unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="50f63-113">Create unifiedRoleAssignmentMultiple</span></span>](../api/unifiedroleassignmentmultiple-post.md) | [<span data-ttu-id="50f63-114">unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="50f63-114">unifiedRoleAssignmentMultiple</span></span>](unifiedroleassignmentmultiple.md) | <span data-ttu-id="50f63-115">Crie um novo unifiedRoleAssignmentMultiple postando na coleção roleAssignments.</span><span class="sxs-lookup"><span data-stu-id="50f63-115">Create a new unifiedRoleAssignmentMultiple by posting to the roleAssignments collection.</span></span> |
| [<span data-ttu-id="50f63-116">Listar roleAssignmentsMultiple</span><span class="sxs-lookup"><span data-stu-id="50f63-116">List roleAssignmentsMultiple</span></span>](../api/unifiedroleassignmentmultiple-list.md) | <span data-ttu-id="50f63-117">coleção [unifiedRoleAssignmentMultiple](unifiedroleassignmentmultiple.md)</span><span class="sxs-lookup"><span data-stu-id="50f63-117">[unifiedRoleAssignmentMultiple](unifiedroleassignmentmultiple.md) collection</span></span> | <span data-ttu-id="50f63-118">Obtém a coleção de objetos unifiedRoleAssignmentMultiple.</span><span class="sxs-lookup"><span data-stu-id="50f63-118">Get unifiedRoleAssignmentMultiple object collection.</span></span> |
| [<span data-ttu-id="50f63-119">Criar unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="50f63-119">Create unifiedRoleDefinition</span></span>](../api/rbacapplication-post-roledefinitions.md) | [<span data-ttu-id="50f63-120">unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="50f63-120">unifiedRoleDefinition</span></span>](unifiedroledefinition.md) | <span data-ttu-id="50f63-121">Crie um novo unifiedRoleDefinition postando na coleção roleDefinitions.</span><span class="sxs-lookup"><span data-stu-id="50f63-121">Create a new unifiedRoleDefinition by posting to the roleDefinitions collection.</span></span> |
| [<span data-ttu-id="50f63-122">Listar roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="50f63-122">List roleDefinitions</span></span>](../api/rbacapplication-list-roledefinitions.md) | <span data-ttu-id="50f63-123">coleção [unifiedRoleDefinition](unifiedroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="50f63-123">[unifiedRoleDefinition](unifiedroledefinition.md) collection</span></span> | <span data-ttu-id="50f63-124">Obtenha uma coleção de objetos unifiedRoleDefinition.</span><span class="sxs-lookup"><span data-stu-id="50f63-124">Get a unifiedRoleDefinition object collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="50f63-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="50f63-125">Properties</span></span>

<span data-ttu-id="50f63-126">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="50f63-126">None</span></span>

## <a name="relationships"></a><span data-ttu-id="50f63-127">Relações</span><span class="sxs-lookup"><span data-stu-id="50f63-127">Relationships</span></span>

<span data-ttu-id="50f63-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="50f63-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="50f63-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="50f63-129">JSON representation</span></span>

<span data-ttu-id="50f63-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="50f63-130">None</span></span>

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "rbacApplicationMultiple resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
