---
title: tipo de recurso entitlementManagementSettings
description: Representa as configurações de todos os locatários para o gerenciamento de qualificação do Azure AD.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b183466b102b480913c3841585ea3349e7ac2386
ms.sourcegitcommit: 0545b031585e605dc3a0fde481015f51f79819c4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/22/2020
ms.locfileid: "45225059"
---
# <a name="entitlementmanagementsettings-resource-type"></a><span data-ttu-id="62e3c-103">tipo de recurso entitlementManagementSettings</span><span class="sxs-lookup"><span data-stu-id="62e3c-103">entitlementManagementSettings resource type</span></span>

<span data-ttu-id="62e3c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62e3c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="62e3c-105">Representa as configurações que controlam o comportamento do [Gerenciamento de qualificação do Azure ad](entitlementmanagement-root.md).</span><span class="sxs-lookup"><span data-stu-id="62e3c-105">Represents settings that control the behavior of [Azure AD entitlement management](entitlementmanagement-root.md).</span></span>

## <a name="methods"></a><span data-ttu-id="62e3c-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="62e3c-106">Methods</span></span>

| <span data-ttu-id="62e3c-107">Método</span><span class="sxs-lookup"><span data-stu-id="62e3c-107">Method</span></span>       | <span data-ttu-id="62e3c-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="62e3c-108">Return Type</span></span> | <span data-ttu-id="62e3c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="62e3c-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="62e3c-110">Get</span><span class="sxs-lookup"><span data-stu-id="62e3c-110">Get</span></span>](../api/entitlementmanagementsettings-get.md) | [<span data-ttu-id="62e3c-111">entitlementManagementSettings</span><span class="sxs-lookup"><span data-stu-id="62e3c-111">entitlementManagementSettings</span></span>](entitlementmanagementsettings.md) | <span data-ttu-id="62e3c-112">Ler as propriedades de um objeto **entitlementManagementSettings** .</span><span class="sxs-lookup"><span data-stu-id="62e3c-112">Read the properties of an **entitlementManagementSettings** object.</span></span> |
| [<span data-ttu-id="62e3c-113">Update</span><span class="sxs-lookup"><span data-stu-id="62e3c-113">Update</span></span>](../api/entitlementmanagementsettings-update.md) | [<span data-ttu-id="62e3c-114">entitlementManagementSettings</span><span class="sxs-lookup"><span data-stu-id="62e3c-114">entitlementManagementSettings</span></span>](entitlementmanagementsettings.md) | <span data-ttu-id="62e3c-115">Atualiza as propriedades de um objeto **entitlementManagementSettings** .</span><span class="sxs-lookup"><span data-stu-id="62e3c-115">Update the properties of an **entitlementManagementSettings** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="62e3c-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="62e3c-116">Properties</span></span>

| <span data-ttu-id="62e3c-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="62e3c-117">Property</span></span>     | <span data-ttu-id="62e3c-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="62e3c-118">Type</span></span>        | <span data-ttu-id="62e3c-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="62e3c-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="62e3c-120">externalUserLifecycleAction</span><span class="sxs-lookup"><span data-stu-id="62e3c-120">externalUserLifecycleAction</span></span>|<span data-ttu-id="62e3c-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="62e3c-121">String</span></span>|<span data-ttu-id="62e3c-122">Um de `None` , `BlockSignIn` ou `BlockSignInAndDelete` .</span><span class="sxs-lookup"><span data-stu-id="62e3c-122">One of `None`, `BlockSignIn`, or `BlockSignInAndDelete`.</span></span> |
|<span data-ttu-id="62e3c-123">daysUntilExternalUserDeletedAfterBlocked</span><span class="sxs-lookup"><span data-stu-id="62e3c-123">daysUntilExternalUserDeletedAfterBlocked</span></span>|<span data-ttu-id="62e3c-124">Int64</span><span class="sxs-lookup"><span data-stu-id="62e3c-124">Int64</span></span>|<span data-ttu-id="62e3c-125">Se `externalUserLifecycleAction` for `BlockSignInAndDelete` , o número de dias após o qual um usuário externo é bloqueado de entrar antes que sua conta seja excluída.</span><span class="sxs-lookup"><span data-stu-id="62e3c-125">If `externalUserLifecycleAction` is `BlockSignInAndDelete`, the number of days after an external user is blocked from sign in before their account is deleted.</span></span>|

## <a name="relationships"></a><span data-ttu-id="62e3c-126">Relações</span><span class="sxs-lookup"><span data-stu-id="62e3c-126">Relationships</span></span>

<span data-ttu-id="62e3c-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="62e3c-127">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="62e3c-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="62e3c-128">JSON representation</span></span>

<span data-ttu-id="62e3c-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="62e3c-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.entitlementManagementSettings",
  "baseType": "",
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
