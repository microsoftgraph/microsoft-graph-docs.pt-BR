---
title: Tipo de recurso entitlementManagementSettings
description: Representa as configurações de todo o locatário para o gerenciamento de direitos do Azure AD.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9d5cc340837f173924802196bf12c9a63f26949a
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159119"
---
# <a name="entitlementmanagementsettings-resource-type"></a><span data-ttu-id="6b4b2-103">Tipo de recurso entitlementManagementSettings</span><span class="sxs-lookup"><span data-stu-id="6b4b2-103">entitlementManagementSettings resource type</span></span>

<span data-ttu-id="6b4b2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b4b2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b4b2-105">Representa configurações que controlam o comportamento do gerenciamento de direitos do [Azure AD.](entitlementmanagement-root.md)</span><span class="sxs-lookup"><span data-stu-id="6b4b2-105">Represents settings that control the behavior of [Azure AD entitlement management](entitlementmanagement-root.md).</span></span>

## <a name="methods"></a><span data-ttu-id="6b4b2-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="6b4b2-106">Methods</span></span>

| <span data-ttu-id="6b4b2-107">Método</span><span class="sxs-lookup"><span data-stu-id="6b4b2-107">Method</span></span>       | <span data-ttu-id="6b4b2-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6b4b2-108">Return Type</span></span> | <span data-ttu-id="6b4b2-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b4b2-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="6b4b2-110">Get</span><span class="sxs-lookup"><span data-stu-id="6b4b2-110">Get</span></span>](../api/entitlementmanagementsettings-get.md) | [<span data-ttu-id="6b4b2-111">entitlementManagementSettings</span><span class="sxs-lookup"><span data-stu-id="6b4b2-111">entitlementManagementSettings</span></span>](entitlementmanagementsettings.md) | <span data-ttu-id="6b4b2-112">Leia as propriedades de um **objeto entitlementManagementSettings.**</span><span class="sxs-lookup"><span data-stu-id="6b4b2-112">Read the properties of an **entitlementManagementSettings** object.</span></span> |
| [<span data-ttu-id="6b4b2-113">Update</span><span class="sxs-lookup"><span data-stu-id="6b4b2-113">Update</span></span>](../api/entitlementmanagementsettings-update.md) | [<span data-ttu-id="6b4b2-114">entitlementManagementSettings</span><span class="sxs-lookup"><span data-stu-id="6b4b2-114">entitlementManagementSettings</span></span>](entitlementmanagementsettings.md) | <span data-ttu-id="6b4b2-115">Atualizar as propriedades de um **objeto entitlementManagementSettings.**</span><span class="sxs-lookup"><span data-stu-id="6b4b2-115">Update the properties of an **entitlementManagementSettings** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="6b4b2-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6b4b2-116">Properties</span></span>

| <span data-ttu-id="6b4b2-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6b4b2-117">Property</span></span>     | <span data-ttu-id="6b4b2-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="6b4b2-118">Type</span></span>        | <span data-ttu-id="6b4b2-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b4b2-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6b4b2-120">externalUserLifecycleAction</span><span class="sxs-lookup"><span data-stu-id="6b4b2-120">externalUserLifecycleAction</span></span>|<span data-ttu-id="6b4b2-121">String</span><span class="sxs-lookup"><span data-stu-id="6b4b2-121">String</span></span>|<span data-ttu-id="6b4b2-122">Um dos `None` , `BlockSignIn` ou `BlockSignInAndDelete` .</span><span class="sxs-lookup"><span data-stu-id="6b4b2-122">One of `None`, `BlockSignIn`, or `BlockSignInAndDelete`.</span></span> |
|<span data-ttu-id="6b4b2-123">daysUntilExternalUserDeletedAfterBlocked</span><span class="sxs-lookup"><span data-stu-id="6b4b2-123">daysUntilExternalUserDeletedAfterBlocked</span></span>|<span data-ttu-id="6b4b2-124">Int64</span><span class="sxs-lookup"><span data-stu-id="6b4b2-124">Int64</span></span>|<span data-ttu-id="6b4b2-125">Se for , o número de dias após um usuário externo ser impedido `externalUserLifecycleAction` de entrar antes de sua conta ser `BlockSignInAndDelete` excluída.</span><span class="sxs-lookup"><span data-stu-id="6b4b2-125">If `externalUserLifecycleAction` is `BlockSignInAndDelete`, the number of days after an external user is blocked from sign in before their account is deleted.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6b4b2-126">Relações</span><span class="sxs-lookup"><span data-stu-id="6b4b2-126">Relationships</span></span>

<span data-ttu-id="6b4b2-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6b4b2-127">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6b4b2-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6b4b2-128">JSON representation</span></span>

<span data-ttu-id="6b4b2-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6b4b2-129">The following is a JSON representation of the resource.</span></span>

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


