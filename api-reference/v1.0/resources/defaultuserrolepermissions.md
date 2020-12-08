---
title: tipo de recurso defaultUserRolePermissions
description: Contém determinadas permissões personalizáveis de função de usuário padrão.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3f2b4fbc4b4a496905f8199b065ecd94e849365e
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581179"
---
# <a name="defaultuserrolepermissions-resource-type"></a><span data-ttu-id="63f50-103">tipo de recurso defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="63f50-103">defaultUserRolePermissions resource type</span></span>

<span data-ttu-id="63f50-104">Contém determinadas permissões personalizáveis de função de usuário padrão no Azure Active Directory (AD).</span><span class="sxs-lookup"><span data-stu-id="63f50-104">Contains certain customizable permissions of default user role in Azure Active Directory (AD).</span></span>

## <a name="properties"></a><span data-ttu-id="63f50-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="63f50-105">Properties</span></span>

| <span data-ttu-id="63f50-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="63f50-106">Property</span></span> | <span data-ttu-id="63f50-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="63f50-107">Type</span></span> | <span data-ttu-id="63f50-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="63f50-108">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="63f50-109">allowedToCreateApps</span><span class="sxs-lookup"><span data-stu-id="63f50-109">allowedToCreateApps</span></span> | <span data-ttu-id="63f50-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="63f50-110">Boolean</span></span> | <span data-ttu-id="63f50-111">Indica se a função de usuário padrão pode criar aplicativos.</span><span class="sxs-lookup"><span data-stu-id="63f50-111">Indicates whether the default user role can create applications.</span></span> |  
| <span data-ttu-id="63f50-112">allowedToCreateSecurityGroups</span><span class="sxs-lookup"><span data-stu-id="63f50-112">allowedToCreateSecurityGroups</span></span> | <span data-ttu-id="63f50-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="63f50-113">Boolean</span></span> | <span data-ttu-id="63f50-114">Indica se a função de usuário padrão pode criar grupos de segurança.</span><span class="sxs-lookup"><span data-stu-id="63f50-114">Indicates whether the default user role can create security groups.</span></span> |  
| <span data-ttu-id="63f50-115">allowedToReadOtherUsers</span><span class="sxs-lookup"><span data-stu-id="63f50-115">allowedToReadOtherUsers</span></span> | <span data-ttu-id="63f50-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="63f50-116">Boolean</span></span> | <span data-ttu-id="63f50-117">Indica se a função de usuário padrão pode ler outros usuários.</span><span class="sxs-lookup"><span data-stu-id="63f50-117">Indicates whether the default user role can read other users.</span></span> |
|<span data-ttu-id="63f50-118">permissionGrantPoliciesAssigned</span><span class="sxs-lookup"><span data-stu-id="63f50-118">permissionGrantPoliciesAssigned</span></span>|<span data-ttu-id="63f50-119">Conjunto de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="63f50-119">String collection</span></span>|<span data-ttu-id="63f50-120">Indica se o consentimento do usuário para os aplicativos é permitido e, se for, qual permissão para conceder consentimento e qual política de consentimento de aplicativo (permissionGrantPolicy) governará a permissão para os usuários concederem o consentimento.</span><span class="sxs-lookup"><span data-stu-id="63f50-120">Indicates if user consent to apps is allowed, and if it is, which permission to grant consent and which app consent policy (permissionGrantPolicy) govern the permission for users to grant consent.</span></span> <span data-ttu-id="63f50-121">O valor deve estar no formato `managePermissionGrantsForSelf.{id}` , onde `{id}` é a **ID** de uma [política de consentimento de aplicativo](/azure/active-directory/manage-apps/manage-app-consent-policies)interna ou personalizada.</span><span class="sxs-lookup"><span data-stu-id="63f50-121">Value should be in the format `managePermissionGrantsForSelf.{id}`, where `{id}` is the **id** of a built-in or custom [app consent policy](/azure/active-directory/manage-apps/manage-app-consent-policies).</span></span> <span data-ttu-id="63f50-122">Uma lista vazia indica que o consentimento do usuário para os aplicativos está desabilitado.</span><span class="sxs-lookup"><span data-stu-id="63f50-122">An empty list indicates user consent to apps is disabled.</span></span> |

## <a name="relationships"></a><span data-ttu-id="63f50-123">Relações</span><span class="sxs-lookup"><span data-stu-id="63f50-123">Relationships</span></span>

<span data-ttu-id="63f50-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="63f50-124">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="63f50-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="63f50-125">JSON representation</span></span>

<span data-ttu-id="63f50-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="63f50-126">The following is a JSON representation of the resource.</span></span>

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
