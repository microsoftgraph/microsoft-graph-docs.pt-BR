---
title: Tipo de recurso delegatedPermissionClassification
description: Usado para especificar a classificação de uma permissão delegada.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: 4a567696d2adf0cd2a53cc2eb4d193ec1e1c2855
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133634"
---
# <a name="delegatedpermissionclassification-resource-type"></a><span data-ttu-id="83f77-103">Tipo de recurso delegatedPermissionClassification</span><span class="sxs-lookup"><span data-stu-id="83f77-103">delegatedPermissionClassification resource type</span></span>

<span data-ttu-id="83f77-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="83f77-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83f77-105">Usado para especificar a classificação de uma permissão delegada.</span><span class="sxs-lookup"><span data-stu-id="83f77-105">Used to specify the classification of a delegated permission.</span></span>

<span data-ttu-id="83f77-106">As classificações de permissão delegada podem ser usadas em combinação com as configurações de consentimento do usuário para escolher quais permissões um usuário tem permissão para consentir.</span><span class="sxs-lookup"><span data-stu-id="83f77-106">Delegated permission classifications can be used in combination with user consent settings to choose which permissions a user is allowed to consent to.</span></span> <span data-ttu-id="83f77-107">Consulte [Configurar como os usuários finais permitem que os aplicativos](/azure/active-directory/manage-apps/configure-user-consent) aprendam mais sobre classificações de permissão.</span><span class="sxs-lookup"><span data-stu-id="83f77-107">See [Configure how end-users consent to applications](/azure/active-directory/manage-apps/configure-user-consent) to learn more about permission classifications.</span></span>

## <a name="properties"></a><span data-ttu-id="83f77-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="83f77-108">Properties</span></span>

| <span data-ttu-id="83f77-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="83f77-109">Property</span></span> | <span data-ttu-id="83f77-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="83f77-110">Type</span></span> | <span data-ttu-id="83f77-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="83f77-111">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="83f77-112">id</span><span class="sxs-lookup"><span data-stu-id="83f77-112">id</span></span> | <span data-ttu-id="83f77-113">String</span><span class="sxs-lookup"><span data-stu-id="83f77-113">String</span></span> | <span data-ttu-id="83f77-114">Um identificador exclusivo para a **chave delegatedPermissionClassification.**</span><span class="sxs-lookup"><span data-stu-id="83f77-114">A unique identifier for the **delegatedPermissionClassification** Key.</span></span> <span data-ttu-id="83f77-115">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="83f77-115">Not nullable.</span></span> <span data-ttu-id="83f77-116">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="83f77-116">Read-only.</span></span> |
| <span data-ttu-id="83f77-117">classificação</span><span class="sxs-lookup"><span data-stu-id="83f77-117">classification</span></span> | <span data-ttu-id="83f77-118">permissionClassificationType</span><span class="sxs-lookup"><span data-stu-id="83f77-118">permissionClassificationType</span></span> | <span data-ttu-id="83f77-119">O valor de classificação sendo dado.</span><span class="sxs-lookup"><span data-stu-id="83f77-119">The classification value being given.</span></span> <span data-ttu-id="83f77-120">Valor possível: `low` .</span><span class="sxs-lookup"><span data-stu-id="83f77-120">Possible value: `low`.</span></span> <span data-ttu-id="83f77-121">O não tem suporte para `$filter`.</span><span class="sxs-lookup"><span data-stu-id="83f77-121">Does not support `$filter`.</span></span> |
| <span data-ttu-id="83f77-122">permissionId</span><span class="sxs-lookup"><span data-stu-id="83f77-122">permissionId</span></span> | <span data-ttu-id="83f77-123">Guid</span><span class="sxs-lookup"><span data-stu-id="83f77-123">Guid</span></span> | <span data-ttu-id="83f77-124">O identificador exclusivo (**id**) para a permissão delegada listada na **coleção publishedPermissionScopes** do [servicePrincipal](servicePrincipal.md).</span><span class="sxs-lookup"><span data-stu-id="83f77-124">The unique identifier (**id**) for the delegated permission listed in the **publishedPermissionScopes** collection of the [servicePrincipal](servicePrincipal.md).</span></span> <span data-ttu-id="83f77-125">Obrigatório durante a criação.</span><span class="sxs-lookup"><span data-stu-id="83f77-125">Required on create.</span></span> <span data-ttu-id="83f77-126">O não tem suporte para `$filter`.</span><span class="sxs-lookup"><span data-stu-id="83f77-126">Does not support `$filter`.</span></span> |
| <span data-ttu-id="83f77-127">permissionName</span><span class="sxs-lookup"><span data-stu-id="83f77-127">permissionName</span></span> | <span data-ttu-id="83f77-128">String</span><span class="sxs-lookup"><span data-stu-id="83f77-128">String</span></span> | <span data-ttu-id="83f77-129">O valor da declaração (**valor**) para a permissão delegada listada na **coleção publishedPermissionScopes** do [servicePrincipal](servicePrincipal.md).</span><span class="sxs-lookup"><span data-stu-id="83f77-129">The claim value (**value**) for the delegated permission listed in the **publishedPermissionScopes** collection of the [servicePrincipal](servicePrincipal.md).</span></span> <span data-ttu-id="83f77-130">O não tem suporte para `$filter`.</span><span class="sxs-lookup"><span data-stu-id="83f77-130">Does not support `$filter`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="83f77-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="83f77-131">JSON representation</span></span>

<span data-ttu-id="83f77-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="83f77-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.delegatedPermissionClassification"
}-->

```json
{
  "id": "string (identifier)",
  "classification": "low",
  "permissionId": "string",
  "permissionName": "string"
}
```

