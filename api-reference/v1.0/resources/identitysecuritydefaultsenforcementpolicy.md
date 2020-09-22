---
title: tipo de recurso identitySecurityDefaultsEnforcementPolicy
description: Representa a política de padrões de segurança do Azure Active Directory. Os padrões de segurança contêm configurações de segurança pré-configuradas que protegem contra ataques comuns.
localization_priority: Normal
author: rohinigoyal1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 13c7fd24c7f7d96149821a8a4e506e32ae681c78
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48086694"
---
# <a name="identitysecuritydefaultsenforcementpolicy-resource-type"></a><span data-ttu-id="feb60-104">tipo de recurso identitySecurityDefaultsEnforcementPolicy</span><span class="sxs-lookup"><span data-stu-id="feb60-104">identitySecurityDefaultsEnforcementPolicy resource type</span></span>

<span data-ttu-id="feb60-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="feb60-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="feb60-106">Representa a política de [padrões de segurança](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="feb60-106">Represents the Azure Active Directory [security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) policy.</span></span> <span data-ttu-id="feb60-107">Os padrões de segurança contêm configurações de segurança pré-configuradas que protegem contra ataques comuns.</span><span class="sxs-lookup"><span data-stu-id="feb60-107">Security defaults contain preconfigured security settings that protect against common attacks.</span></span>

<span data-ttu-id="feb60-108">Herda de [policyBase](../resources/policybase.md).</span><span class="sxs-lookup"><span data-stu-id="feb60-108">Inherits from [policyBase](../resources/policybase.md).</span></span>

## <a name="methods"></a><span data-ttu-id="feb60-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="feb60-109">Methods</span></span>

| <span data-ttu-id="feb60-110">Método</span><span class="sxs-lookup"><span data-stu-id="feb60-110">Method</span></span>       | <span data-ttu-id="feb60-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="feb60-111">Return Type</span></span> | <span data-ttu-id="feb60-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="feb60-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="feb60-113">Get</span><span class="sxs-lookup"><span data-stu-id="feb60-113">Get</span></span>](../api/identitysecuritydefaultsenforcementpolicy-get.md) | [<span data-ttu-id="feb60-114">identitySecurityDefaultsEnforcementPolicy</span><span class="sxs-lookup"><span data-stu-id="feb60-114">identitySecurityDefaultsEnforcementPolicy</span></span>](identitysecuritydefaultsenforcementpolicy.md) | <span data-ttu-id="feb60-115">Ler as propriedades de um objeto **identitySecurityDefaultsEnforcementPolicy** .</span><span class="sxs-lookup"><span data-stu-id="feb60-115">Read the properties of an **identitySecurityDefaultsEnforcementPolicy** object.</span></span> |
| [<span data-ttu-id="feb60-116">Atualizar</span><span class="sxs-lookup"><span data-stu-id="feb60-116">Update</span></span>](../api/identitysecuritydefaultsenforcementpolicy-update.md) | [<span data-ttu-id="feb60-117">identitySecurityDefaultsEnforcementPolicy</span><span class="sxs-lookup"><span data-stu-id="feb60-117">identitySecurityDefaultsEnforcementPolicy</span></span>](identitysecuritydefaultsenforcementpolicy.md) | <span data-ttu-id="feb60-118">Atualize um objeto **identitySecurityDefaultsEnforcementPolicy** .</span><span class="sxs-lookup"><span data-stu-id="feb60-118">Update an **identitySecurityDefaultsEnforcementPolicy** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="feb60-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="feb60-119">Properties</span></span>

| <span data-ttu-id="feb60-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="feb60-120">Property</span></span>     | <span data-ttu-id="feb60-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="feb60-121">Type</span></span>        | <span data-ttu-id="feb60-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="feb60-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="feb60-123">description</span><span class="sxs-lookup"><span data-stu-id="feb60-123">description</span></span>|<span data-ttu-id="feb60-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="feb60-124">String</span></span>|<span data-ttu-id="feb60-125">Descrição da política.</span><span class="sxs-lookup"><span data-stu-id="feb60-125">Description for this policy.</span></span> <span data-ttu-id="feb60-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="feb60-126">Read-only.</span></span>|
|<span data-ttu-id="feb60-127">displayName</span><span class="sxs-lookup"><span data-stu-id="feb60-127">displayName</span></span>|<span data-ttu-id="feb60-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="feb60-128">String</span></span>|<span data-ttu-id="feb60-129">Nome para exibição dessa política.</span><span class="sxs-lookup"><span data-stu-id="feb60-129">Display name for this policy.</span></span> <span data-ttu-id="feb60-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="feb60-130">Read-only.</span></span>|
|<span data-ttu-id="feb60-131">id</span><span class="sxs-lookup"><span data-stu-id="feb60-131">id</span></span>|<span data-ttu-id="feb60-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="feb60-132">String</span></span>|<span data-ttu-id="feb60-133">Identificador para esta política.</span><span class="sxs-lookup"><span data-stu-id="feb60-133">Identifier for this policy.</span></span> <span data-ttu-id="feb60-134">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="feb60-134">Read-only.</span></span>|
|<span data-ttu-id="feb60-135">isEnabled</span><span class="sxs-lookup"><span data-stu-id="feb60-135">isEnabled</span></span>|<span data-ttu-id="feb60-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="feb60-136">Boolean</span></span>|<span data-ttu-id="feb60-137">Se definido como true, os padrões de segurança do Active Directory do Azure são habilitados para o locatário.</span><span class="sxs-lookup"><span data-stu-id="feb60-137">If set to true, Azure Active Directory security defaults is enabled for the tenant.</span></span>|

## <a name="relationships"></a><span data-ttu-id="feb60-138">Relações</span><span class="sxs-lookup"><span data-stu-id="feb60-138">Relationships</span></span>

<span data-ttu-id="feb60-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="feb60-139">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="feb60-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="feb60-140">JSON representation</span></span>

<span data-ttu-id="feb60-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="feb60-141">The following is a JSON representation of the resource.</span></span>

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

