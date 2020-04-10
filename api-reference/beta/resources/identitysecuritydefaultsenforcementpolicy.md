---
title: tipo de recurso identitySecurityDefaultsEnforcementPolicy
description: Representa a política de padrões de segurança do Azure Active Directory. Os padrões de segurança contêm configurações de segurança pré-configuradas que protegem contra ataques comuns.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4771af4502df2154435ae6b403fa12e3e265217a
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218461"
---
# <a name="identitysecuritydefaultsenforcementpolicy-resource-type"></a><span data-ttu-id="b423b-104">tipo de recurso identitySecurityDefaultsEnforcementPolicy</span><span class="sxs-lookup"><span data-stu-id="b423b-104">identitySecurityDefaultsEnforcementPolicy resource type</span></span>

<span data-ttu-id="b423b-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b423b-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b423b-106">Representa a política de [padrões de segurança](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b423b-106">Represents the Azure Active Directory [security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) policy.</span></span> <span data-ttu-id="b423b-107">Os padrões de segurança contêm configurações de segurança pré-configuradas que protegem contra ataques comuns.</span><span class="sxs-lookup"><span data-stu-id="b423b-107">Security defaults contain preconfigured security settings that protect against common attacks.</span></span>

<span data-ttu-id="b423b-108">Herda de [policyBase](../resources/policybase.md).</span><span class="sxs-lookup"><span data-stu-id="b423b-108">Inherits from [policyBase](../resources/policybase.md).</span></span>

## <a name="methods"></a><span data-ttu-id="b423b-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="b423b-109">Methods</span></span>

| <span data-ttu-id="b423b-110">Método</span><span class="sxs-lookup"><span data-stu-id="b423b-110">Method</span></span>       | <span data-ttu-id="b423b-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b423b-111">Return Type</span></span> | <span data-ttu-id="b423b-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="b423b-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="b423b-113">Get</span><span class="sxs-lookup"><span data-stu-id="b423b-113">Get</span></span>](../api/identitysecuritydefaultsenforcementpolicy-get.md) | [<span data-ttu-id="b423b-114">identitySecurityDefaultsEnforcementPolicy</span><span class="sxs-lookup"><span data-stu-id="b423b-114">identitySecurityDefaultsEnforcementPolicy</span></span>](identitysecuritydefaultsenforcementpolicy.md) | <span data-ttu-id="b423b-115">Ler as propriedades de um objeto **identitySecurityDefaultsEnforcementPolicy** .</span><span class="sxs-lookup"><span data-stu-id="b423b-115">Read the properties of an **identitySecurityDefaultsEnforcementPolicy** object.</span></span> |
| [<span data-ttu-id="b423b-116">Update</span><span class="sxs-lookup"><span data-stu-id="b423b-116">Update</span></span>](../api/identitysecuritydefaultsenforcementpolicy-update.md) | [<span data-ttu-id="b423b-117">identitySecurityDefaultsEnforcementPolicy</span><span class="sxs-lookup"><span data-stu-id="b423b-117">identitySecurityDefaultsEnforcementPolicy</span></span>](identitysecuritydefaultsenforcementpolicy.md) | <span data-ttu-id="b423b-118">Atualize um objeto **identitySecurityDefaultsEnforcementPolicy** .</span><span class="sxs-lookup"><span data-stu-id="b423b-118">Update an **identitySecurityDefaultsEnforcementPolicy** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="b423b-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b423b-119">Properties</span></span>

| <span data-ttu-id="b423b-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b423b-120">Property</span></span>     | <span data-ttu-id="b423b-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="b423b-121">Type</span></span>        | <span data-ttu-id="b423b-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="b423b-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b423b-123">description</span><span class="sxs-lookup"><span data-stu-id="b423b-123">description</span></span>|<span data-ttu-id="b423b-124">String</span><span class="sxs-lookup"><span data-stu-id="b423b-124">String</span></span>|<span data-ttu-id="b423b-125">Descrição da política.</span><span class="sxs-lookup"><span data-stu-id="b423b-125">Description for this policy.</span></span> <span data-ttu-id="b423b-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b423b-126">Read-only.</span></span>|
|<span data-ttu-id="b423b-127">displayName</span><span class="sxs-lookup"><span data-stu-id="b423b-127">displayName</span></span>|<span data-ttu-id="b423b-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b423b-128">String</span></span>|<span data-ttu-id="b423b-129">Nome para exibição dessa política.</span><span class="sxs-lookup"><span data-stu-id="b423b-129">Display name for this policy.</span></span> <span data-ttu-id="b423b-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b423b-130">Read-only.</span></span>|
|<span data-ttu-id="b423b-131">id</span><span class="sxs-lookup"><span data-stu-id="b423b-131">id</span></span>|<span data-ttu-id="b423b-132">String</span><span class="sxs-lookup"><span data-stu-id="b423b-132">String</span></span>|<span data-ttu-id="b423b-133">Identificador para esta política.</span><span class="sxs-lookup"><span data-stu-id="b423b-133">Identifier for this policy.</span></span> <span data-ttu-id="b423b-134">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b423b-134">Read-only.</span></span>|
|<span data-ttu-id="b423b-135">isEnabled</span><span class="sxs-lookup"><span data-stu-id="b423b-135">isEnabled</span></span>|<span data-ttu-id="b423b-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="b423b-136">Boolean</span></span>|<span data-ttu-id="b423b-137">Se definido como true, os padrões de segurança do Active Directory do Azure são habilitados para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b423b-137">If set to true, Azure Active Directory security defaults is enabled for the tenant.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b423b-138">Relações</span><span class="sxs-lookup"><span data-stu-id="b423b-138">Relationships</span></span>

<span data-ttu-id="b423b-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b423b-139">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b423b-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b423b-140">JSON representation</span></span>

<span data-ttu-id="b423b-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b423b-141">The following is a JSON representation of the resource.</span></span>

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
