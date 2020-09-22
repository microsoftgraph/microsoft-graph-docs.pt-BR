---
title: tipo de recurso entitlementManagementSettings
description: Representa as configurações de todos os locatários para o gerenciamento de qualificação do Azure AD.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 84f34740bd5e16bb001cd3618edf4c4b669155f2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48052879"
---
# <a name="entitlementmanagementsettings-resource-type"></a><span data-ttu-id="66ac1-103">tipo de recurso entitlementManagementSettings</span><span class="sxs-lookup"><span data-stu-id="66ac1-103">entitlementManagementSettings resource type</span></span>

<span data-ttu-id="66ac1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66ac1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66ac1-105">Representa as configurações que controlam o comportamento do [Gerenciamento de qualificação do Azure ad](entitlementmanagement-root.md).</span><span class="sxs-lookup"><span data-stu-id="66ac1-105">Represents settings that control the behavior of [Azure AD entitlement management](entitlementmanagement-root.md).</span></span>

## <a name="methods"></a><span data-ttu-id="66ac1-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="66ac1-106">Methods</span></span>

| <span data-ttu-id="66ac1-107">Método</span><span class="sxs-lookup"><span data-stu-id="66ac1-107">Method</span></span>       | <span data-ttu-id="66ac1-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="66ac1-108">Return Type</span></span> | <span data-ttu-id="66ac1-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="66ac1-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="66ac1-110">Get</span><span class="sxs-lookup"><span data-stu-id="66ac1-110">Get</span></span>](../api/entitlementmanagementsettings-get.md) | [<span data-ttu-id="66ac1-111">entitlementManagementSettings</span><span class="sxs-lookup"><span data-stu-id="66ac1-111">entitlementManagementSettings</span></span>](entitlementmanagementsettings.md) | <span data-ttu-id="66ac1-112">Ler as propriedades de um objeto **entitlementManagementSettings** .</span><span class="sxs-lookup"><span data-stu-id="66ac1-112">Read the properties of an **entitlementManagementSettings** object.</span></span> |
| [<span data-ttu-id="66ac1-113">Atualizar</span><span class="sxs-lookup"><span data-stu-id="66ac1-113">Update</span></span>](../api/entitlementmanagementsettings-update.md) | [<span data-ttu-id="66ac1-114">entitlementManagementSettings</span><span class="sxs-lookup"><span data-stu-id="66ac1-114">entitlementManagementSettings</span></span>](entitlementmanagementsettings.md) | <span data-ttu-id="66ac1-115">Atualiza as propriedades de um objeto **entitlementManagementSettings** .</span><span class="sxs-lookup"><span data-stu-id="66ac1-115">Update the properties of an **entitlementManagementSettings** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="66ac1-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="66ac1-116">Properties</span></span>

| <span data-ttu-id="66ac1-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="66ac1-117">Property</span></span>     | <span data-ttu-id="66ac1-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="66ac1-118">Type</span></span>        | <span data-ttu-id="66ac1-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="66ac1-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="66ac1-120">externalUserLifecycleAction</span><span class="sxs-lookup"><span data-stu-id="66ac1-120">externalUserLifecycleAction</span></span>|<span data-ttu-id="66ac1-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="66ac1-121">String</span></span>|<span data-ttu-id="66ac1-122">Um de `None` , `BlockSignIn` ou `BlockSignInAndDelete` .</span><span class="sxs-lookup"><span data-stu-id="66ac1-122">One of `None`, `BlockSignIn`, or `BlockSignInAndDelete`.</span></span> |
|<span data-ttu-id="66ac1-123">daysUntilExternalUserDeletedAfterBlocked</span><span class="sxs-lookup"><span data-stu-id="66ac1-123">daysUntilExternalUserDeletedAfterBlocked</span></span>|<span data-ttu-id="66ac1-124">Int64</span><span class="sxs-lookup"><span data-stu-id="66ac1-124">Int64</span></span>|<span data-ttu-id="66ac1-125">Se `externalUserLifecycleAction` for `BlockSignInAndDelete` , o número de dias após o qual um usuário externo é bloqueado de entrar antes que sua conta seja excluída.</span><span class="sxs-lookup"><span data-stu-id="66ac1-125">If `externalUserLifecycleAction` is `BlockSignInAndDelete`, the number of days after an external user is blocked from sign in before their account is deleted.</span></span>|

## <a name="relationships"></a><span data-ttu-id="66ac1-126">Relações</span><span class="sxs-lookup"><span data-stu-id="66ac1-126">Relationships</span></span>

<span data-ttu-id="66ac1-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="66ac1-127">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="66ac1-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="66ac1-128">JSON representation</span></span>

<span data-ttu-id="66ac1-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="66ac1-129">The following is a JSON representation of the resource.</span></span>

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


