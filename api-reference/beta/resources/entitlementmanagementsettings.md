---
title: Tipo de recurso entitlementManagementSettings
description: Representa as configurações de todo o locatário para o gerenciamento de direitos do Azure AD.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: d34a04d0f8eb3bdff16befd43870b75d473a8d0c
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2021
ms.locfileid: "53350975"
---
# <a name="entitlementmanagementsettings-resource-type"></a><span data-ttu-id="12359-103">Tipo de recurso entitlementManagementSettings</span><span class="sxs-lookup"><span data-stu-id="12359-103">entitlementManagementSettings resource type</span></span>

<span data-ttu-id="12359-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12359-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="12359-105">Representa configurações que controlam o comportamento do gerenciamento de direitos do [Azure AD.](entitlementmanagement-root.md)</span><span class="sxs-lookup"><span data-stu-id="12359-105">Represents settings that control the behavior of [Azure AD entitlement management](entitlementmanagement-root.md).</span></span>  <span data-ttu-id="12359-106">Esse recurso não inclui a configuração de criadores de catálogos; para exibir ou alterar a associação de função de criadores de catálogo, use a [API](unifiedroleassignment.md) de atribuições de função com o provedor RBAC de gerenciamento de direitos.</span><span class="sxs-lookup"><span data-stu-id="12359-106">This resource does not include the catalog creators setting; to view or change the catalog creators role membership, use the [role assignments](unifiedroleassignment.md) API with the entitlement management RBAC provider.</span></span>

## <a name="methods"></a><span data-ttu-id="12359-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="12359-107">Methods</span></span>

| <span data-ttu-id="12359-108">Método</span><span class="sxs-lookup"><span data-stu-id="12359-108">Method</span></span>       | <span data-ttu-id="12359-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="12359-109">Return Type</span></span> | <span data-ttu-id="12359-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="12359-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="12359-111">Get</span><span class="sxs-lookup"><span data-stu-id="12359-111">Get</span></span>](../api/entitlementmanagementsettings-get.md) | [<span data-ttu-id="12359-112">entitlementManagementSettings</span><span class="sxs-lookup"><span data-stu-id="12359-112">entitlementManagementSettings</span></span>](entitlementmanagementsettings.md) | <span data-ttu-id="12359-113">Leia as propriedades de **um objeto entitlementManagementSettings.**</span><span class="sxs-lookup"><span data-stu-id="12359-113">Read the properties of an **entitlementManagementSettings** object.</span></span> |
| [<span data-ttu-id="12359-114">Atualizar</span><span class="sxs-lookup"><span data-stu-id="12359-114">Update</span></span>](../api/entitlementmanagementsettings-update.md) | [<span data-ttu-id="12359-115">entitlementManagementSettings</span><span class="sxs-lookup"><span data-stu-id="12359-115">entitlementManagementSettings</span></span>](entitlementmanagementsettings.md) | <span data-ttu-id="12359-116">Atualize as propriedades de **um objeto entitlementManagementSettings.**</span><span class="sxs-lookup"><span data-stu-id="12359-116">Update the properties of an **entitlementManagementSettings** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="12359-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="12359-117">Properties</span></span>

| <span data-ttu-id="12359-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="12359-118">Property</span></span>     | <span data-ttu-id="12359-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="12359-119">Type</span></span>        | <span data-ttu-id="12359-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="12359-120">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="12359-121">externalUserLifecycleAction</span><span class="sxs-lookup"><span data-stu-id="12359-121">externalUserLifecycleAction</span></span>|<span data-ttu-id="12359-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="12359-122">String</span></span>|<span data-ttu-id="12359-123">Um dos `None` , `BlockSignIn` ou `BlockSignInAndDelete` .</span><span class="sxs-lookup"><span data-stu-id="12359-123">One of `None`, `BlockSignIn`, or `BlockSignInAndDelete`.</span></span> |
|<span data-ttu-id="12359-124">daysUntilExternalUserDeletedAfterBlocked</span><span class="sxs-lookup"><span data-stu-id="12359-124">daysUntilExternalUserDeletedAfterBlocked</span></span>|<span data-ttu-id="12359-125">Int64</span><span class="sxs-lookup"><span data-stu-id="12359-125">Int64</span></span>|<span data-ttu-id="12359-126">Se **externalUserLifecycleAction** for , o número de dias após um usuário externo ser bloqueado de entrar antes de `BlockSignInAndDelete` sua conta ser excluída.</span><span class="sxs-lookup"><span data-stu-id="12359-126">If **externalUserLifecycleAction** is `BlockSignInAndDelete`, the number of days after an external user is blocked from sign in before their account is deleted.</span></span>|

## <a name="relationships"></a><span data-ttu-id="12359-127">Relações</span><span class="sxs-lookup"><span data-stu-id="12359-127">Relationships</span></span>

<span data-ttu-id="12359-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="12359-128">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="12359-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="12359-129">JSON representation</span></span>

<span data-ttu-id="12359-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="12359-130">The following is a JSON representation of the resource.</span></span>

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


