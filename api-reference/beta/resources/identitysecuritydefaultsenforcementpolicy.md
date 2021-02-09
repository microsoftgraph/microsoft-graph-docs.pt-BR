---
title: Tipo de recurso identitySecurityDefaultsEnforcementPolicy
description: Representa a política de padrões de segurança do Azure Active Directory. Os padrões de segurança contêm configurações de segurança pré-configuradas que protegem contra ataques comuns.
localization_priority: Normal
author: rohinigoyal1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1dea4d94dfc8de8310410498fdf8d83c2a5e8f68
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50154926"
---
# <a name="identitysecuritydefaultsenforcementpolicy-resource-type"></a><span data-ttu-id="92826-104">Tipo de recurso identitySecurityDefaultsEnforcementPolicy</span><span class="sxs-lookup"><span data-stu-id="92826-104">identitySecurityDefaultsEnforcementPolicy resource type</span></span>

<span data-ttu-id="92826-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92826-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92826-106">Representa a política de padrões de [segurança](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="92826-106">Represents the Azure Active Directory [security defaults](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) policy.</span></span> <span data-ttu-id="92826-107">Os padrões de segurança contêm configurações de segurança pré-configuradas que protegem contra ataques comuns.</span><span class="sxs-lookup"><span data-stu-id="92826-107">Security defaults contain preconfigured security settings that protect against common attacks.</span></span>

<span data-ttu-id="92826-108">Herda de [policyBase](../resources/policybase.md).</span><span class="sxs-lookup"><span data-stu-id="92826-108">Inherits from [policyBase](../resources/policybase.md).</span></span>

## <a name="methods"></a><span data-ttu-id="92826-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="92826-109">Methods</span></span>

| <span data-ttu-id="92826-110">Método</span><span class="sxs-lookup"><span data-stu-id="92826-110">Method</span></span>       | <span data-ttu-id="92826-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="92826-111">Return Type</span></span> | <span data-ttu-id="92826-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="92826-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="92826-113">Get</span><span class="sxs-lookup"><span data-stu-id="92826-113">Get</span></span>](../api/identitysecuritydefaultsenforcementpolicy-get.md) | [<span data-ttu-id="92826-114">identitySecurityDefaultsEnforcementPolicy</span><span class="sxs-lookup"><span data-stu-id="92826-114">identitySecurityDefaultsEnforcementPolicy</span></span>](identitysecuritydefaultsenforcementpolicy.md) | <span data-ttu-id="92826-115">Leia as propriedades de um **objeto identitySecurityDefaultsEnforcementPolicy.**</span><span class="sxs-lookup"><span data-stu-id="92826-115">Read the properties of an **identitySecurityDefaultsEnforcementPolicy** object.</span></span> |
| [<span data-ttu-id="92826-116">Update</span><span class="sxs-lookup"><span data-stu-id="92826-116">Update</span></span>](../api/identitysecuritydefaultsenforcementpolicy-update.md) | [<span data-ttu-id="92826-117">identitySecurityDefaultsEnforcementPolicy</span><span class="sxs-lookup"><span data-stu-id="92826-117">identitySecurityDefaultsEnforcementPolicy</span></span>](identitysecuritydefaultsenforcementpolicy.md) | <span data-ttu-id="92826-118">Atualize **um objeto identitySecurityDefaultsEnforcementPolicy.**</span><span class="sxs-lookup"><span data-stu-id="92826-118">Update an **identitySecurityDefaultsEnforcementPolicy** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="92826-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="92826-119">Properties</span></span>

| <span data-ttu-id="92826-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="92826-120">Property</span></span>     | <span data-ttu-id="92826-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="92826-121">Type</span></span>        | <span data-ttu-id="92826-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="92826-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="92826-123">description</span><span class="sxs-lookup"><span data-stu-id="92826-123">description</span></span>|<span data-ttu-id="92826-124">String</span><span class="sxs-lookup"><span data-stu-id="92826-124">String</span></span>|<span data-ttu-id="92826-125">Descrição desta política.</span><span class="sxs-lookup"><span data-stu-id="92826-125">Description for this policy.</span></span> <span data-ttu-id="92826-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="92826-126">Read-only.</span></span>|
|<span data-ttu-id="92826-127">displayName</span><span class="sxs-lookup"><span data-stu-id="92826-127">displayName</span></span>|<span data-ttu-id="92826-128">String</span><span class="sxs-lookup"><span data-stu-id="92826-128">String</span></span>|<span data-ttu-id="92826-129">Nome para exibição desta política.</span><span class="sxs-lookup"><span data-stu-id="92826-129">Display name for this policy.</span></span> <span data-ttu-id="92826-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="92826-130">Read-only.</span></span>|
|<span data-ttu-id="92826-131">id</span><span class="sxs-lookup"><span data-stu-id="92826-131">id</span></span>|<span data-ttu-id="92826-132">String</span><span class="sxs-lookup"><span data-stu-id="92826-132">String</span></span>|<span data-ttu-id="92826-133">Identificador desta política.</span><span class="sxs-lookup"><span data-stu-id="92826-133">Identifier for this policy.</span></span> <span data-ttu-id="92826-134">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="92826-134">Read-only.</span></span>|
|<span data-ttu-id="92826-135">isEnabled</span><span class="sxs-lookup"><span data-stu-id="92826-135">isEnabled</span></span>|<span data-ttu-id="92826-136">Booliano</span><span class="sxs-lookup"><span data-stu-id="92826-136">Boolean</span></span>|<span data-ttu-id="92826-137">Se definido como verdadeiro, os padrões de segurança do Azure Active Directory são habilitados para o locatário.</span><span class="sxs-lookup"><span data-stu-id="92826-137">If set to true, Azure Active Directory security defaults is enabled for the tenant.</span></span>|

## <a name="relationships"></a><span data-ttu-id="92826-138">Relações</span><span class="sxs-lookup"><span data-stu-id="92826-138">Relationships</span></span>

<span data-ttu-id="92826-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="92826-139">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="92826-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="92826-140">JSON representation</span></span>

<span data-ttu-id="92826-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="92826-141">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.identitySecurityDefaultsEnforcementPolicy",
  "keyProperty": "id"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "isEnabled": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "identitySecurityDefaultsEnforcementPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->