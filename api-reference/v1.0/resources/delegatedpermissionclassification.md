---
title: tipo de recurso delegatedPermissionClassification
description: Usado para especificar a classificação de uma permissão delegada.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 7d5926bff0d7096080aa22fae49d0ed15c7d1fcd
ms.sourcegitcommit: 6201b3a5646f640f25a68ab033eca9eb60ccd05e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377174"
---
# <a name="delegatedpermissionclassification-resource-type"></a><span data-ttu-id="c6e4d-103">tipo de recurso delegatedPermissionClassification</span><span class="sxs-lookup"><span data-stu-id="c6e4d-103">delegatedPermissionClassification resource type</span></span>

<span data-ttu-id="c6e4d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c6e4d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c6e4d-105">Usado para especificar a classificação de uma permissão delegada.</span><span class="sxs-lookup"><span data-stu-id="c6e4d-105">Used to specify the classification of a delegated permission.</span></span>

<span data-ttu-id="c6e4d-106">As classificações de permissão delegada podem ser usadas em combinação com as configurações de consentimento do usuário para escolher a quais permissões um usuário pode concordar.</span><span class="sxs-lookup"><span data-stu-id="c6e4d-106">Delegated permission classifications can be used in combination with user consent settings to choose which permissions a user is allowed to consent to.</span></span> <span data-ttu-id="c6e4d-107">Confira [configurar como os usuários finais consentiam aos aplicativos](/azure/active-directory/manage-apps/configure-user-consent) para saber mais sobre as classificações de permissão.</span><span class="sxs-lookup"><span data-stu-id="c6e4d-107">See [Configure how end-users consent to applications](/azure/active-directory/manage-apps/configure-user-consent) to learn more about permission classifications.</span></span>

## <a name="properties"></a><span data-ttu-id="c6e4d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c6e4d-108">Properties</span></span>

| <span data-ttu-id="c6e4d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c6e4d-109">Property</span></span> | <span data-ttu-id="c6e4d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="c6e4d-110">Type</span></span> | <span data-ttu-id="c6e4d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6e4d-111">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="c6e4d-112">id</span><span class="sxs-lookup"><span data-stu-id="c6e4d-112">id</span></span> | <span data-ttu-id="c6e4d-113">String</span><span class="sxs-lookup"><span data-stu-id="c6e4d-113">String</span></span> | <span data-ttu-id="c6e4d-114">Um identificador exclusivo para a chave **delegatedPermissionClassification** .</span><span class="sxs-lookup"><span data-stu-id="c6e4d-114">A unique identifier for the **delegatedPermissionClassification** Key.</span></span> <span data-ttu-id="c6e4d-115">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="c6e4d-115">Not nullable.</span></span> <span data-ttu-id="c6e4d-116">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c6e4d-116">Read-only.</span></span> |
| <span data-ttu-id="c6e4d-117">classificação</span><span class="sxs-lookup"><span data-stu-id="c6e4d-117">classification</span></span> | <span data-ttu-id="c6e4d-118">permissionClassificationType</span><span class="sxs-lookup"><span data-stu-id="c6e4d-118">permissionClassificationType</span></span> | <span data-ttu-id="c6e4d-119">O valor de classificação que está sendo fornecido.</span><span class="sxs-lookup"><span data-stu-id="c6e4d-119">The classification value being given.</span></span> <span data-ttu-id="c6e4d-120">Valor possível: `low` .</span><span class="sxs-lookup"><span data-stu-id="c6e4d-120">Possible value: `low`.</span></span> <span data-ttu-id="c6e4d-121">O não tem suporte para `$filter`.</span><span class="sxs-lookup"><span data-stu-id="c6e4d-121">Does not support `$filter`.</span></span> |
| <span data-ttu-id="c6e4d-122">permissionid</span><span class="sxs-lookup"><span data-stu-id="c6e4d-122">permissionId</span></span> | <span data-ttu-id="c6e4d-123">Guid</span><span class="sxs-lookup"><span data-stu-id="c6e4d-123">Guid</span></span> | <span data-ttu-id="c6e4d-124">O identificador exclusivo (**ID**) da permissão delegada listada na coleção **oauth2PermissionScopes** do [servicePrincipalName](servicePrincipal.md).</span><span class="sxs-lookup"><span data-stu-id="c6e4d-124">The unique identifier (**id**) for the delegated permission listed in the **oauth2PermissionScopes** collection of the [servicePrincipal](servicePrincipal.md).</span></span> <span data-ttu-id="c6e4d-125">Obrigatório durante a criação.</span><span class="sxs-lookup"><span data-stu-id="c6e4d-125">Required on create.</span></span> <span data-ttu-id="c6e4d-126">O não tem suporte para `$filter`.</span><span class="sxs-lookup"><span data-stu-id="c6e4d-126">Does not support `$filter`.</span></span> |
| <span data-ttu-id="c6e4d-127">permissionname</span><span class="sxs-lookup"><span data-stu-id="c6e4d-127">permissionName</span></span> | <span data-ttu-id="c6e4d-128">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="c6e4d-128">String</span></span> | <span data-ttu-id="c6e4d-129">O valor de declaração (**valor**) para a permissão delegada listada na coleção **oauth2PermissionScopes** do [servicePrincipalName](servicePrincipal.md).</span><span class="sxs-lookup"><span data-stu-id="c6e4d-129">The claim value (**value**) for the delegated permission listed in the **oauth2PermissionScopes** collection of the [servicePrincipal](servicePrincipal.md).</span></span> <span data-ttu-id="c6e4d-130">O não tem suporte para `$filter`.</span><span class="sxs-lookup"><span data-stu-id="c6e4d-130">Does not support `$filter`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c6e4d-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c6e4d-131">JSON representation</span></span>

<span data-ttu-id="c6e4d-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c6e4d-132">The following is a JSON representation of the resource.</span></span>

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
