---
title: Tipo de recurso identitySecurityDefaultsEnforcementPolicy
description: Representa a política de padrões de segurança do Azure Active Directory. Os padrões de segurança contêm configurações de segurança pré-configuradas que protegem contra ataques comuns.
localization_priority: Normal
author: rohinigoyal1
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 21b012338e6ca168e932a8aaf2560ce825304ae9
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439839"
---
# <a name="identitysecuritydefaultsenforcementpolicy-resource-type"></a><span data-ttu-id="d6678-104">Tipo de recurso identitySecurityDefaultsEnforcementPolicy</span><span class="sxs-lookup"><span data-stu-id="d6678-104">identitySecurityDefaultsEnforcementPolicy resource type</span></span>

<span data-ttu-id="d6678-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6678-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d6678-106">Representa a política de padrões de [segurança](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d6678-106">Represents the Azure Active Directory [security defaults](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) policy.</span></span> <span data-ttu-id="d6678-107">Os padrões de segurança contêm configurações de segurança pré-configuradas que protegem contra ataques comuns.</span><span class="sxs-lookup"><span data-stu-id="d6678-107">Security defaults contain preconfigured security settings that protect against common attacks.</span></span>

<span data-ttu-id="d6678-108">Herda de [policyBase](../resources/policybase.md).</span><span class="sxs-lookup"><span data-stu-id="d6678-108">Inherits from [policyBase](../resources/policybase.md).</span></span>

## <a name="methods"></a><span data-ttu-id="d6678-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="d6678-109">Methods</span></span>

| <span data-ttu-id="d6678-110">Método</span><span class="sxs-lookup"><span data-stu-id="d6678-110">Method</span></span>       | <span data-ttu-id="d6678-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d6678-111">Return Type</span></span> | <span data-ttu-id="d6678-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6678-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="d6678-113">Get</span><span class="sxs-lookup"><span data-stu-id="d6678-113">Get</span></span>](../api/identitysecuritydefaultsenforcementpolicy-get.md) | [<span data-ttu-id="d6678-114">identitySecurityDefaultsEnforcementPolicy</span><span class="sxs-lookup"><span data-stu-id="d6678-114">identitySecurityDefaultsEnforcementPolicy</span></span>](identitysecuritydefaultsenforcementpolicy.md) | <span data-ttu-id="d6678-115">Leia as propriedades de **um objeto identitySecurityDefaultsEnforcementPolicy.**</span><span class="sxs-lookup"><span data-stu-id="d6678-115">Read the properties of an **identitySecurityDefaultsEnforcementPolicy** object.</span></span> |
| [<span data-ttu-id="d6678-116">Atualizar</span><span class="sxs-lookup"><span data-stu-id="d6678-116">Update</span></span>](../api/identitysecuritydefaultsenforcementpolicy-update.md) | [<span data-ttu-id="d6678-117">identitySecurityDefaultsEnforcementPolicy</span><span class="sxs-lookup"><span data-stu-id="d6678-117">identitySecurityDefaultsEnforcementPolicy</span></span>](identitysecuritydefaultsenforcementpolicy.md) | <span data-ttu-id="d6678-118">Atualize **um objeto identitySecurityDefaultsEnforcementPolicy.**</span><span class="sxs-lookup"><span data-stu-id="d6678-118">Update an **identitySecurityDefaultsEnforcementPolicy** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="d6678-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d6678-119">Properties</span></span>

| <span data-ttu-id="d6678-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d6678-120">Property</span></span>     | <span data-ttu-id="d6678-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="d6678-121">Type</span></span>        | <span data-ttu-id="d6678-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6678-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d6678-123">description</span><span class="sxs-lookup"><span data-stu-id="d6678-123">description</span></span>|<span data-ttu-id="d6678-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6678-124">String</span></span>|<span data-ttu-id="d6678-125">Descrição dessa política.</span><span class="sxs-lookup"><span data-stu-id="d6678-125">Description for this policy.</span></span> <span data-ttu-id="d6678-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d6678-126">Read-only.</span></span>|
|<span data-ttu-id="d6678-127">displayName</span><span class="sxs-lookup"><span data-stu-id="d6678-127">displayName</span></span>|<span data-ttu-id="d6678-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6678-128">String</span></span>|<span data-ttu-id="d6678-129">Nome de exibição para esta política.</span><span class="sxs-lookup"><span data-stu-id="d6678-129">Display name for this policy.</span></span> <span data-ttu-id="d6678-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d6678-130">Read-only.</span></span>|
|<span data-ttu-id="d6678-131">id</span><span class="sxs-lookup"><span data-stu-id="d6678-131">id</span></span>|<span data-ttu-id="d6678-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6678-132">String</span></span>|<span data-ttu-id="d6678-133">Identificador dessa política.</span><span class="sxs-lookup"><span data-stu-id="d6678-133">Identifier for this policy.</span></span> <span data-ttu-id="d6678-134">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d6678-134">Read-only.</span></span>|
|<span data-ttu-id="d6678-135">isEnabled</span><span class="sxs-lookup"><span data-stu-id="d6678-135">isEnabled</span></span>|<span data-ttu-id="d6678-136">Booliano</span><span class="sxs-lookup"><span data-stu-id="d6678-136">Boolean</span></span>|<span data-ttu-id="d6678-137">Se definido como true, os padrões de segurança do Azure Active Directory são habilitados para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d6678-137">If set to true, Azure Active Directory security defaults is enabled for the tenant.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d6678-138">Relações</span><span class="sxs-lookup"><span data-stu-id="d6678-138">Relationships</span></span>

<span data-ttu-id="d6678-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d6678-139">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d6678-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d6678-140">JSON representation</span></span>

<span data-ttu-id="d6678-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d6678-141">The following is a JSON representation of the resource.</span></span>

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
