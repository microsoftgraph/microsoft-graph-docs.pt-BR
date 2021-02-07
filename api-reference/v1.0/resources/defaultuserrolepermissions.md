---
title: Tipo de recurso defaultUserRolePermissions
description: Contém determinadas permissões personalizáveis da função de usuário padrão.
localization_priority: Normal
author: abhijeetsinha
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 0e89f175a62615efe172646613897222a9ae75fa
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137554"
---
# <a name="defaultuserrolepermissions-resource-type"></a><span data-ttu-id="84b03-103">Tipo de recurso defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="84b03-103">defaultUserRolePermissions resource type</span></span>

<span data-ttu-id="84b03-104">Contém determinadas permissões personalizáveis da função de usuário padrão no Azure Active Directory (AD).</span><span class="sxs-lookup"><span data-stu-id="84b03-104">Contains certain customizable permissions of default user role in Azure Active Directory (AD).</span></span>

## <a name="properties"></a><span data-ttu-id="84b03-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="84b03-105">Properties</span></span>

| <span data-ttu-id="84b03-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="84b03-106">Property</span></span> | <span data-ttu-id="84b03-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="84b03-107">Type</span></span> | <span data-ttu-id="84b03-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="84b03-108">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="84b03-109">allowedToCreateApps</span><span class="sxs-lookup"><span data-stu-id="84b03-109">allowedToCreateApps</span></span> | <span data-ttu-id="84b03-110">Booliano</span><span class="sxs-lookup"><span data-stu-id="84b03-110">Boolean</span></span> | <span data-ttu-id="84b03-111">Indica se a função de usuário padrão pode criar aplicativos.</span><span class="sxs-lookup"><span data-stu-id="84b03-111">Indicates whether the default user role can create applications.</span></span> |  
| <span data-ttu-id="84b03-112">allowedToCreateSecurityGroups</span><span class="sxs-lookup"><span data-stu-id="84b03-112">allowedToCreateSecurityGroups</span></span> | <span data-ttu-id="84b03-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="84b03-113">Boolean</span></span> | <span data-ttu-id="84b03-114">Indica se a função de usuário padrão pode criar grupos de segurança.</span><span class="sxs-lookup"><span data-stu-id="84b03-114">Indicates whether the default user role can create security groups.</span></span> |  
| <span data-ttu-id="84b03-115">allowedToReadOtherUsers</span><span class="sxs-lookup"><span data-stu-id="84b03-115">allowedToReadOtherUsers</span></span> | <span data-ttu-id="84b03-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="84b03-116">Boolean</span></span> | <span data-ttu-id="84b03-117">Indica se a função de usuário padrão pode ler outros usuários.</span><span class="sxs-lookup"><span data-stu-id="84b03-117">Indicates whether the default user role can read other users.</span></span> |
|<span data-ttu-id="84b03-118">permissionGrantPoliciesAssigned</span><span class="sxs-lookup"><span data-stu-id="84b03-118">permissionGrantPoliciesAssigned</span></span>|<span data-ttu-id="84b03-119">String collection</span><span class="sxs-lookup"><span data-stu-id="84b03-119">String collection</span></span>|<span data-ttu-id="84b03-120">Indica se o consentimento do usuário para aplicativos é permitido e, se for, qual permissão para conceder consentimento e qual política de consentimento do aplicativo (permissionGrantPolicy) regem a permissão para que os usuários concedam consentimento.</span><span class="sxs-lookup"><span data-stu-id="84b03-120">Indicates if user consent to apps is allowed, and if it is, which permission to grant consent and which app consent policy (permissionGrantPolicy) govern the permission for users to grant consent.</span></span> <span data-ttu-id="84b03-121">Value should be in the format `managePermissionGrantsForSelf.{id}` , where is the `{id}` **id** of a built-in or custom [app consent policy](/azure/active-directory/manage-apps/manage-app-consent-policies).</span><span class="sxs-lookup"><span data-stu-id="84b03-121">Value should be in the format `managePermissionGrantsForSelf.{id}`, where `{id}` is the **id** of a built-in or custom [app consent policy](/azure/active-directory/manage-apps/manage-app-consent-policies).</span></span> <span data-ttu-id="84b03-122">Uma lista vazia indica que o consentimento do usuário para aplicativos está desabilitado.</span><span class="sxs-lookup"><span data-stu-id="84b03-122">An empty list indicates user consent to apps is disabled.</span></span> |

## <a name="relationships"></a><span data-ttu-id="84b03-123">Relações</span><span class="sxs-lookup"><span data-stu-id="84b03-123">Relationships</span></span>

<span data-ttu-id="84b03-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="84b03-124">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="84b03-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="84b03-125">JSON representation</span></span>

<span data-ttu-id="84b03-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="84b03-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.defaultUserRolePermissions"
}-->

```json
{
  "allowedToCreateApps": true,
  "allowedToCreateSecurityGroups": true,
  "allowedToReadOtherUsers": true,
  "permissionGrantPoliciesAssigned": ["String"]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "defaultUserRolePermissions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
