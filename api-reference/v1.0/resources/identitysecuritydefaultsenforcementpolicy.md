---
title: tipo de recurso identitySecurityDefaultsEnforcementPolicy
description: Representa a política de padrões de segurança do Azure Active Directory. Os padrões de segurança contêm configurações de segurança pré-configuradas que protegem contra ataques comuns.
localization_priority: Normal
author: rohinigoyal1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c208733525162397c190bd425cdf7c770a302c0f
ms.sourcegitcommit: 577bfd3bb8a2e2679ef1c5942a4a496c2aa3a277
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/17/2020
ms.locfileid: "48581915"
---
# <a name="identitysecuritydefaultsenforcementpolicy-resource-type"></a><span data-ttu-id="b96b9-104">tipo de recurso identitySecurityDefaultsEnforcementPolicy</span><span class="sxs-lookup"><span data-stu-id="b96b9-104">identitySecurityDefaultsEnforcementPolicy resource type</span></span>

<span data-ttu-id="b96b9-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b96b9-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b96b9-106">Representa a política de [padrões de segurança](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b96b9-106">Represents the Azure Active Directory [security defaults](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) policy.</span></span> <span data-ttu-id="b96b9-107">Os padrões de segurança contêm configurações de segurança pré-configuradas que protegem contra ataques comuns.</span><span class="sxs-lookup"><span data-stu-id="b96b9-107">Security defaults contain preconfigured security settings that protect against common attacks.</span></span>

<span data-ttu-id="b96b9-108">Herda de [policyBase](../resources/policybase.md).</span><span class="sxs-lookup"><span data-stu-id="b96b9-108">Inherits from [policyBase](../resources/policybase.md).</span></span>

## <a name="methods"></a><span data-ttu-id="b96b9-109">Methods</span><span class="sxs-lookup"><span data-stu-id="b96b9-109">Methods</span></span>

| <span data-ttu-id="b96b9-110">Método</span><span class="sxs-lookup"><span data-stu-id="b96b9-110">Method</span></span>       | <span data-ttu-id="b96b9-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b96b9-111">Return Type</span></span> | <span data-ttu-id="b96b9-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="b96b9-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="b96b9-113">Get</span><span class="sxs-lookup"><span data-stu-id="b96b9-113">Get</span></span>](../api/identitysecuritydefaultsenforcementpolicy-get.md) | [<span data-ttu-id="b96b9-114">identitySecurityDefaultsEnforcementPolicy</span><span class="sxs-lookup"><span data-stu-id="b96b9-114">identitySecurityDefaultsEnforcementPolicy</span></span>](identitysecuritydefaultsenforcementpolicy.md) | <span data-ttu-id="b96b9-115">Ler as propriedades de um objeto **identitySecurityDefaultsEnforcementPolicy** .</span><span class="sxs-lookup"><span data-stu-id="b96b9-115">Read the properties of an **identitySecurityDefaultsEnforcementPolicy** object.</span></span> |
| [<span data-ttu-id="b96b9-116">Update</span><span class="sxs-lookup"><span data-stu-id="b96b9-116">Update</span></span>](../api/identitysecuritydefaultsenforcementpolicy-update.md) | [<span data-ttu-id="b96b9-117">identitySecurityDefaultsEnforcementPolicy</span><span class="sxs-lookup"><span data-stu-id="b96b9-117">identitySecurityDefaultsEnforcementPolicy</span></span>](identitysecuritydefaultsenforcementpolicy.md) | <span data-ttu-id="b96b9-118">Atualize um objeto **identitySecurityDefaultsEnforcementPolicy** .</span><span class="sxs-lookup"><span data-stu-id="b96b9-118">Update an **identitySecurityDefaultsEnforcementPolicy** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="b96b9-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b96b9-119">Properties</span></span>

| <span data-ttu-id="b96b9-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b96b9-120">Property</span></span>     | <span data-ttu-id="b96b9-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="b96b9-121">Type</span></span>        | <span data-ttu-id="b96b9-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="b96b9-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b96b9-123">description</span><span class="sxs-lookup"><span data-stu-id="b96b9-123">description</span></span>|<span data-ttu-id="b96b9-124">String</span><span class="sxs-lookup"><span data-stu-id="b96b9-124">String</span></span>|<span data-ttu-id="b96b9-125">Descrição da política.</span><span class="sxs-lookup"><span data-stu-id="b96b9-125">Description for this policy.</span></span> <span data-ttu-id="b96b9-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b96b9-126">Read-only.</span></span>|
|<span data-ttu-id="b96b9-127">displayName</span><span class="sxs-lookup"><span data-stu-id="b96b9-127">displayName</span></span>|<span data-ttu-id="b96b9-128">String</span><span class="sxs-lookup"><span data-stu-id="b96b9-128">String</span></span>|<span data-ttu-id="b96b9-129">Nome para exibição dessa política.</span><span class="sxs-lookup"><span data-stu-id="b96b9-129">Display name for this policy.</span></span> <span data-ttu-id="b96b9-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b96b9-130">Read-only.</span></span>|
|<span data-ttu-id="b96b9-131">id</span><span class="sxs-lookup"><span data-stu-id="b96b9-131">id</span></span>|<span data-ttu-id="b96b9-132">String</span><span class="sxs-lookup"><span data-stu-id="b96b9-132">String</span></span>|<span data-ttu-id="b96b9-133">Identificador para esta política.</span><span class="sxs-lookup"><span data-stu-id="b96b9-133">Identifier for this policy.</span></span> <span data-ttu-id="b96b9-134">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b96b9-134">Read-only.</span></span>|
|<span data-ttu-id="b96b9-135">isEnabled</span><span class="sxs-lookup"><span data-stu-id="b96b9-135">isEnabled</span></span>|<span data-ttu-id="b96b9-136">Booliano</span><span class="sxs-lookup"><span data-stu-id="b96b9-136">Boolean</span></span>|<span data-ttu-id="b96b9-137">Se definido como true, os padrões de segurança do Active Directory do Azure são habilitados para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b96b9-137">If set to true, Azure Active Directory security defaults is enabled for the tenant.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b96b9-138">Relações</span><span class="sxs-lookup"><span data-stu-id="b96b9-138">Relationships</span></span>

<span data-ttu-id="b96b9-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b96b9-139">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b96b9-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b96b9-140">JSON representation</span></span>

<span data-ttu-id="b96b9-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b96b9-141">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.identitySecurityDefaultsEnforcementPolicy",
  "baseType": "",
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