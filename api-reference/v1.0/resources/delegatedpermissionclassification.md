---
title: Tipo de recurso delegatedPermissionClassification
description: Usado para especificar a classificação de uma permissão delegada.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: ff9f4ca394e2065c69fd7cd08a19d60817fc4f99
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761755"
---
# <a name="delegatedpermissionclassification-resource-type"></a><span data-ttu-id="fc229-103">Tipo de recurso delegatedPermissionClassification</span><span class="sxs-lookup"><span data-stu-id="fc229-103">delegatedPermissionClassification resource type</span></span>

<span data-ttu-id="fc229-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc229-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fc229-105">Usado para especificar a classificação de uma permissão delegada.</span><span class="sxs-lookup"><span data-stu-id="fc229-105">Used to specify the classification of a delegated permission.</span></span>

<span data-ttu-id="fc229-106">As classificações de permissão delegadas podem ser usadas em combinação com as configurações de consentimento do usuário para escolher quais permissões um usuário tem permissão para consentir.</span><span class="sxs-lookup"><span data-stu-id="fc229-106">Delegated permission classifications can be used in combination with user consent settings to choose which permissions a user is allowed to consent to.</span></span> <span data-ttu-id="fc229-107">Consulte [Configure how end-users consent to applications](/azure/active-directory/manage-apps/configure-user-consent) to learn more about permission classifications.</span><span class="sxs-lookup"><span data-stu-id="fc229-107">See [Configure how end-users consent to applications](/azure/active-directory/manage-apps/configure-user-consent) to learn more about permission classifications.</span></span>

## <a name="properties"></a><span data-ttu-id="fc229-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fc229-108">Properties</span></span>

| <span data-ttu-id="fc229-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fc229-109">Property</span></span> | <span data-ttu-id="fc229-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="fc229-110">Type</span></span> | <span data-ttu-id="fc229-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc229-111">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="fc229-112">id</span><span class="sxs-lookup"><span data-stu-id="fc229-112">id</span></span> | <span data-ttu-id="fc229-113">String</span><span class="sxs-lookup"><span data-stu-id="fc229-113">String</span></span> | <span data-ttu-id="fc229-114">Um identificador exclusivo para **a chave delegatedPermissionClassification.**</span><span class="sxs-lookup"><span data-stu-id="fc229-114">A unique identifier for the **delegatedPermissionClassification** Key.</span></span> <span data-ttu-id="fc229-115">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="fc229-115">Not nullable.</span></span> <span data-ttu-id="fc229-116">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fc229-116">Read-only.</span></span> |
| <span data-ttu-id="fc229-117">classificação</span><span class="sxs-lookup"><span data-stu-id="fc229-117">classification</span></span> | <span data-ttu-id="fc229-118">permissionClassificationType</span><span class="sxs-lookup"><span data-stu-id="fc229-118">permissionClassificationType</span></span> | <span data-ttu-id="fc229-119">O valor de classificação que está sendo dado.</span><span class="sxs-lookup"><span data-stu-id="fc229-119">The classification value being given.</span></span> <span data-ttu-id="fc229-120">Valor possível: `low` .</span><span class="sxs-lookup"><span data-stu-id="fc229-120">Possible value: `low`.</span></span> <span data-ttu-id="fc229-121">O não tem suporte para `$filter`.</span><span class="sxs-lookup"><span data-stu-id="fc229-121">Does not support `$filter`.</span></span> |
| <span data-ttu-id="fc229-122">permissionId</span><span class="sxs-lookup"><span data-stu-id="fc229-122">permissionId</span></span> | <span data-ttu-id="fc229-123">Guid</span><span class="sxs-lookup"><span data-stu-id="fc229-123">Guid</span></span> | <span data-ttu-id="fc229-124">O identificador exclusivo (**id**) da permissão delegada listada na coleção **oauth2PermissionScopes** [do servicePrincipal](servicePrincipal.md).</span><span class="sxs-lookup"><span data-stu-id="fc229-124">The unique identifier (**id**) for the delegated permission listed in the **oauth2PermissionScopes** collection of the [servicePrincipal](servicePrincipal.md).</span></span> <span data-ttu-id="fc229-125">Obrigatório durante a criação.</span><span class="sxs-lookup"><span data-stu-id="fc229-125">Required on create.</span></span> <span data-ttu-id="fc229-126">O não tem suporte para `$filter`.</span><span class="sxs-lookup"><span data-stu-id="fc229-126">Does not support `$filter`.</span></span> |
| <span data-ttu-id="fc229-127">permissionName</span><span class="sxs-lookup"><span data-stu-id="fc229-127">permissionName</span></span> | <span data-ttu-id="fc229-128">String</span><span class="sxs-lookup"><span data-stu-id="fc229-128">String</span></span> | <span data-ttu-id="fc229-129">O valor da declaração (**valor**) da permissão delegada listada na coleção **oauth2PermissionScopes** do [servicePrincipal](servicePrincipal.md).</span><span class="sxs-lookup"><span data-stu-id="fc229-129">The claim value (**value**) for the delegated permission listed in the **oauth2PermissionScopes** collection of the [servicePrincipal](servicePrincipal.md).</span></span> <span data-ttu-id="fc229-130">O não tem suporte para `$filter`.</span><span class="sxs-lookup"><span data-stu-id="fc229-130">Does not support `$filter`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fc229-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fc229-131">JSON representation</span></span>

<span data-ttu-id="fc229-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fc229-132">The following is a JSON representation of the resource.</span></span>

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
