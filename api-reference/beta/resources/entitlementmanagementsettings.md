---
title: Tipo de recurso entitlementManagementSettings
description: Representa as configurações de todo o locatário para o gerenciamento de direitos do Azure AD.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: b4b6ee584e671e070955eb7c065c59cb8481c375
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440350"
---
# <a name="entitlementmanagementsettings-resource-type"></a><span data-ttu-id="2ec39-103">Tipo de recurso entitlementManagementSettings</span><span class="sxs-lookup"><span data-stu-id="2ec39-103">entitlementManagementSettings resource type</span></span>

<span data-ttu-id="2ec39-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ec39-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ec39-105">Representa configurações que controlam o comportamento do gerenciamento de direitos do [Azure AD.](entitlementmanagement-root.md)</span><span class="sxs-lookup"><span data-stu-id="2ec39-105">Represents settings that control the behavior of [Azure AD entitlement management](entitlementmanagement-root.md).</span></span>

## <a name="methods"></a><span data-ttu-id="2ec39-106">Methods</span><span class="sxs-lookup"><span data-stu-id="2ec39-106">Methods</span></span>

| <span data-ttu-id="2ec39-107">Método</span><span class="sxs-lookup"><span data-stu-id="2ec39-107">Method</span></span>       | <span data-ttu-id="2ec39-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2ec39-108">Return Type</span></span> | <span data-ttu-id="2ec39-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ec39-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="2ec39-110">Get</span><span class="sxs-lookup"><span data-stu-id="2ec39-110">Get</span></span>](../api/entitlementmanagementsettings-get.md) | [<span data-ttu-id="2ec39-111">entitlementManagementSettings</span><span class="sxs-lookup"><span data-stu-id="2ec39-111">entitlementManagementSettings</span></span>](entitlementmanagementsettings.md) | <span data-ttu-id="2ec39-112">Leia as propriedades de **um objeto entitlementManagementSettings.**</span><span class="sxs-lookup"><span data-stu-id="2ec39-112">Read the properties of an **entitlementManagementSettings** object.</span></span> |
| [<span data-ttu-id="2ec39-113">Atualização</span><span class="sxs-lookup"><span data-stu-id="2ec39-113">Update</span></span>](../api/entitlementmanagementsettings-update.md) | [<span data-ttu-id="2ec39-114">entitlementManagementSettings</span><span class="sxs-lookup"><span data-stu-id="2ec39-114">entitlementManagementSettings</span></span>](entitlementmanagementsettings.md) | <span data-ttu-id="2ec39-115">Atualize as propriedades de **um objeto entitlementManagementSettings.**</span><span class="sxs-lookup"><span data-stu-id="2ec39-115">Update the properties of an **entitlementManagementSettings** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="2ec39-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2ec39-116">Properties</span></span>

| <span data-ttu-id="2ec39-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2ec39-117">Property</span></span>     | <span data-ttu-id="2ec39-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="2ec39-118">Type</span></span>        | <span data-ttu-id="2ec39-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ec39-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2ec39-120">externalUserLifecycleAction</span><span class="sxs-lookup"><span data-stu-id="2ec39-120">externalUserLifecycleAction</span></span>|<span data-ttu-id="2ec39-121">String</span><span class="sxs-lookup"><span data-stu-id="2ec39-121">String</span></span>|<span data-ttu-id="2ec39-122">Um dos `None` , `BlockSignIn` ou `BlockSignInAndDelete` .</span><span class="sxs-lookup"><span data-stu-id="2ec39-122">One of `None`, `BlockSignIn`, or `BlockSignInAndDelete`.</span></span> |
|<span data-ttu-id="2ec39-123">daysUntilExternalUserDeletedAfterBlocked</span><span class="sxs-lookup"><span data-stu-id="2ec39-123">daysUntilExternalUserDeletedAfterBlocked</span></span>|<span data-ttu-id="2ec39-124">Int64</span><span class="sxs-lookup"><span data-stu-id="2ec39-124">Int64</span></span>|<span data-ttu-id="2ec39-125">Se for , o número de dias após um usuário externo ser bloqueado de `externalUserLifecycleAction` entrar antes que sua conta seja `BlockSignInAndDelete` excluída.</span><span class="sxs-lookup"><span data-stu-id="2ec39-125">If `externalUserLifecycleAction` is `BlockSignInAndDelete`, the number of days after an external user is blocked from sign in before their account is deleted.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2ec39-126">Relações</span><span class="sxs-lookup"><span data-stu-id="2ec39-126">Relationships</span></span>

<span data-ttu-id="2ec39-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2ec39-127">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2ec39-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2ec39-128">JSON representation</span></span>

<span data-ttu-id="2ec39-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2ec39-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.entitlementManagementSettings",
  "keyProperty": ""
}-->

```json
{
  "externalUserLifecycleAction": "String",
  "daysUntilExternalUserDeletedAfterBlocked": 1
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "entitlementManagementSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


