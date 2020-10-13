---
title: tipo de recurso delegatedPermissionClassification
description: Usado para especificar a classificação de uma permissão delegada.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: f41ea807859b11982283b2a9743d6167e99dac66
ms.sourcegitcommit: 775b38baac6a4e7704d6144ef4589f2fc476bd61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/13/2020
ms.locfileid: "48433517"
---
# <a name="delegatedpermissionclassification-resource-type"></a><span data-ttu-id="1750e-103">tipo de recurso delegatedPermissionClassification</span><span class="sxs-lookup"><span data-stu-id="1750e-103">delegatedPermissionClassification resource type</span></span>

<span data-ttu-id="1750e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1750e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1750e-105">Usado para especificar a classificação de uma permissão delegada.</span><span class="sxs-lookup"><span data-stu-id="1750e-105">Used to specify the classification of a delegated permission.</span></span>

<span data-ttu-id="1750e-106">As classificações de permissão delegada podem ser usadas em combinação com as configurações de consentimento do usuário para escolher a quais permissões um usuário pode concordar.</span><span class="sxs-lookup"><span data-stu-id="1750e-106">Delegated permission classifications can be used in combination with user consent settings to choose which permissions a user is allowed to consent to.</span></span> <span data-ttu-id="1750e-107">Confira [configurar como os usuários finais consentiam aos aplicativos](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) para saber mais sobre as classificações de permissão.</span><span class="sxs-lookup"><span data-stu-id="1750e-107">See [Configure how end-users consent to applications](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) to learn more about permission classifications.</span></span>

## <a name="properties"></a><span data-ttu-id="1750e-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1750e-108">Properties</span></span>

| <span data-ttu-id="1750e-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1750e-109">Property</span></span> | <span data-ttu-id="1750e-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="1750e-110">Type</span></span> | <span data-ttu-id="1750e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1750e-111">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="1750e-112">id</span><span class="sxs-lookup"><span data-stu-id="1750e-112">id</span></span> | <span data-ttu-id="1750e-113">String</span><span class="sxs-lookup"><span data-stu-id="1750e-113">String</span></span> | <span data-ttu-id="1750e-114">Um identificador exclusivo para a chave **delegatedPermissionClassification** .</span><span class="sxs-lookup"><span data-stu-id="1750e-114">A unique identifier for the **delegatedPermissionClassification** Key.</span></span> <span data-ttu-id="1750e-115">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="1750e-115">Not nullable.</span></span> <span data-ttu-id="1750e-116">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1750e-116">Read-only.</span></span> |
| <span data-ttu-id="1750e-117">classificação</span><span class="sxs-lookup"><span data-stu-id="1750e-117">classification</span></span> | <span data-ttu-id="1750e-118">permissionClassificationType</span><span class="sxs-lookup"><span data-stu-id="1750e-118">permissionClassificationType</span></span> | <span data-ttu-id="1750e-119">O valor de classificação que está sendo fornecido.</span><span class="sxs-lookup"><span data-stu-id="1750e-119">The classification value being given.</span></span> <span data-ttu-id="1750e-120">Valor possível: `low` .</span><span class="sxs-lookup"><span data-stu-id="1750e-120">Possible value: `low`.</span></span> <span data-ttu-id="1750e-121">O não tem suporte para `$filter`.</span><span class="sxs-lookup"><span data-stu-id="1750e-121">Does not support `$filter`.</span></span> |
| <span data-ttu-id="1750e-122">permissionid</span><span class="sxs-lookup"><span data-stu-id="1750e-122">permissionId</span></span> | <span data-ttu-id="1750e-123">Guid</span><span class="sxs-lookup"><span data-stu-id="1750e-123">Guid</span></span> | <span data-ttu-id="1750e-124">O identificador exclusivo (**ID**) da permissão delegada listada na coleção **publishedPermissionScopes** do [servicePrincipalName](servicePrincipal.md).</span><span class="sxs-lookup"><span data-stu-id="1750e-124">The unique identifier (**id**) for the delegated permission listed in the **publishedPermissionScopes** collection of the [servicePrincipal](servicePrincipal.md).</span></span> <span data-ttu-id="1750e-125">Obrigatório durante a criação.</span><span class="sxs-lookup"><span data-stu-id="1750e-125">Required on create.</span></span> <span data-ttu-id="1750e-126">O não tem suporte para `$filter`.</span><span class="sxs-lookup"><span data-stu-id="1750e-126">Does not support `$filter`.</span></span> |
| <span data-ttu-id="1750e-127">permissionname</span><span class="sxs-lookup"><span data-stu-id="1750e-127">permissionName</span></span> | <span data-ttu-id="1750e-128">String</span><span class="sxs-lookup"><span data-stu-id="1750e-128">String</span></span> | <span data-ttu-id="1750e-129">O valor de declaração (**valor**) para a permissão delegada listada na coleção **publishedPermissionScopes** do [servicePrincipalName](servicePrincipal.md).</span><span class="sxs-lookup"><span data-stu-id="1750e-129">The claim value (**value**) for the delegated permission listed in the **publishedPermissionScopes** collection of the [servicePrincipal](servicePrincipal.md).</span></span> <span data-ttu-id="1750e-130">O não tem suporte para `$filter`.</span><span class="sxs-lookup"><span data-stu-id="1750e-130">Does not support `$filter`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1750e-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1750e-131">JSON representation</span></span>

<span data-ttu-id="1750e-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1750e-132">The following is a JSON representation of the resource.</span></span>

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
