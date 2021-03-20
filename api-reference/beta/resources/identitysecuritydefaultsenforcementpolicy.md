---
title: Tipo de recurso identitySecurityDefaultsEnforcementPolicy
description: Representa a política de padrões de segurança do Azure Active Directory. Os padrões de segurança contêm configurações de segurança pré-configuradas que protegem contra ataques comuns.
localization_priority: Normal
author: rohinigoyal1
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 249396b0c2bfc4b39ca21c198958adc3d0b9e228
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945638"
---
# <a name="identitysecuritydefaultsenforcementpolicy-resource-type"></a><span data-ttu-id="825ac-104">Tipo de recurso identitySecurityDefaultsEnforcementPolicy</span><span class="sxs-lookup"><span data-stu-id="825ac-104">identitySecurityDefaultsEnforcementPolicy resource type</span></span>

<span data-ttu-id="825ac-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="825ac-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="825ac-106">Representa a política de padrões de [segurança](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="825ac-106">Represents the Azure Active Directory [security defaults](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) policy.</span></span> <span data-ttu-id="825ac-107">Os padrões de segurança contêm configurações de segurança pré-configuradas que protegem contra ataques comuns.</span><span class="sxs-lookup"><span data-stu-id="825ac-107">Security defaults contain preconfigured security settings that protect against common attacks.</span></span>

<span data-ttu-id="825ac-108">Herda de [policyBase](../resources/policybase.md).</span><span class="sxs-lookup"><span data-stu-id="825ac-108">Inherits from [policyBase](../resources/policybase.md).</span></span>

## <a name="methods"></a><span data-ttu-id="825ac-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="825ac-109">Methods</span></span>

| <span data-ttu-id="825ac-110">Método</span><span class="sxs-lookup"><span data-stu-id="825ac-110">Method</span></span>       | <span data-ttu-id="825ac-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="825ac-111">Return Type</span></span> | <span data-ttu-id="825ac-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="825ac-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="825ac-113">Get</span><span class="sxs-lookup"><span data-stu-id="825ac-113">Get</span></span>](../api/identitysecuritydefaultsenforcementpolicy-get.md) | [<span data-ttu-id="825ac-114">identitySecurityDefaultsEnforcementPolicy</span><span class="sxs-lookup"><span data-stu-id="825ac-114">identitySecurityDefaultsEnforcementPolicy</span></span>](identitysecuritydefaultsenforcementpolicy.md) | <span data-ttu-id="825ac-115">Leia as propriedades de **um objeto identitySecurityDefaultsEnforcementPolicy.**</span><span class="sxs-lookup"><span data-stu-id="825ac-115">Read the properties of an **identitySecurityDefaultsEnforcementPolicy** object.</span></span> |
| [<span data-ttu-id="825ac-116">Atualização</span><span class="sxs-lookup"><span data-stu-id="825ac-116">Update</span></span>](../api/identitysecuritydefaultsenforcementpolicy-update.md) | [<span data-ttu-id="825ac-117">identitySecurityDefaultsEnforcementPolicy</span><span class="sxs-lookup"><span data-stu-id="825ac-117">identitySecurityDefaultsEnforcementPolicy</span></span>](identitysecuritydefaultsenforcementpolicy.md) | <span data-ttu-id="825ac-118">Atualize **um objeto identitySecurityDefaultsEnforcementPolicy.**</span><span class="sxs-lookup"><span data-stu-id="825ac-118">Update an **identitySecurityDefaultsEnforcementPolicy** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="825ac-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="825ac-119">Properties</span></span>

| <span data-ttu-id="825ac-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="825ac-120">Property</span></span>     | <span data-ttu-id="825ac-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="825ac-121">Type</span></span>        | <span data-ttu-id="825ac-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="825ac-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="825ac-123">description</span><span class="sxs-lookup"><span data-stu-id="825ac-123">description</span></span>|<span data-ttu-id="825ac-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="825ac-124">String</span></span>|<span data-ttu-id="825ac-125">Descrição dessa política.</span><span class="sxs-lookup"><span data-stu-id="825ac-125">Description for this policy.</span></span> <span data-ttu-id="825ac-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="825ac-126">Read-only.</span></span>|
|<span data-ttu-id="825ac-127">displayName</span><span class="sxs-lookup"><span data-stu-id="825ac-127">displayName</span></span>|<span data-ttu-id="825ac-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="825ac-128">String</span></span>|<span data-ttu-id="825ac-129">Nome de exibição para esta política.</span><span class="sxs-lookup"><span data-stu-id="825ac-129">Display name for this policy.</span></span> <span data-ttu-id="825ac-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="825ac-130">Read-only.</span></span>|
|<span data-ttu-id="825ac-131">id</span><span class="sxs-lookup"><span data-stu-id="825ac-131">id</span></span>|<span data-ttu-id="825ac-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="825ac-132">String</span></span>|<span data-ttu-id="825ac-133">Identificador dessa política.</span><span class="sxs-lookup"><span data-stu-id="825ac-133">Identifier for this policy.</span></span> <span data-ttu-id="825ac-134">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="825ac-134">Read-only.</span></span>|
|<span data-ttu-id="825ac-135">isEnabled</span><span class="sxs-lookup"><span data-stu-id="825ac-135">isEnabled</span></span>|<span data-ttu-id="825ac-136">Booliano</span><span class="sxs-lookup"><span data-stu-id="825ac-136">Boolean</span></span>|<span data-ttu-id="825ac-137">Se definido como , os padrões de segurança do `true` Azure Active Directory estão habilitados para o locatário.</span><span class="sxs-lookup"><span data-stu-id="825ac-137">If set to `true`, Azure Active Directory security defaults is enabled for the tenant.</span></span>|

## <a name="relationships"></a><span data-ttu-id="825ac-138">Relações</span><span class="sxs-lookup"><span data-stu-id="825ac-138">Relationships</span></span>

<span data-ttu-id="825ac-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="825ac-139">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="825ac-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="825ac-140">JSON representation</span></span>

<span data-ttu-id="825ac-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="825ac-141">The following is a JSON representation of the resource.</span></span>

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
