---
title: Tipo de recurso defaultUserRolePermissions
description: Contém determinadas permissões personalizáveis da função de usuário padrão.
localization_priority: Normal
author: abhijeetsinha
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: b6ee2e8deccf73929b68079379efb0f6d93a3369
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135664"
---
# <a name="defaultuserrolepermissions-resource-type"></a><span data-ttu-id="1b260-103">Tipo de recurso defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="1b260-103">defaultUserRolePermissions resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b260-104">Contém determinadas permissões personalizáveis da função de usuário padrão no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="1b260-104">Contains certains customizable permissions of default user role in Azure AD.</span></span>

## <a name="properties"></a><span data-ttu-id="1b260-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1b260-105">Properties</span></span>

| <span data-ttu-id="1b260-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1b260-106">Property</span></span> | <span data-ttu-id="1b260-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="1b260-107">Type</span></span> | <span data-ttu-id="1b260-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b260-108">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="1b260-109">allowedToCreateApps</span><span class="sxs-lookup"><span data-stu-id="1b260-109">allowedToCreateApps</span></span> | <span data-ttu-id="1b260-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b260-110">Boolean</span></span> | <span data-ttu-id="1b260-111">Indica se a função de usuário padrão pode criar aplicativos.</span><span class="sxs-lookup"><span data-stu-id="1b260-111">Indicates whether the default user role can create applications.</span></span> |  
| <span data-ttu-id="1b260-112">allowedToCreateSecurityGroups</span><span class="sxs-lookup"><span data-stu-id="1b260-112">allowedToCreateSecurityGroups</span></span> | <span data-ttu-id="1b260-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b260-113">Boolean</span></span> | <span data-ttu-id="1b260-114">Indica se a função de usuário padrão pode criar grupos de segurança.</span><span class="sxs-lookup"><span data-stu-id="1b260-114">Indicates whether the default user role can create security groups.</span></span> |  
| <span data-ttu-id="1b260-115">allowedToReadOtherUsers</span><span class="sxs-lookup"><span data-stu-id="1b260-115">allowedToReadOtherUsers</span></span> | <span data-ttu-id="1b260-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b260-116">Boolean</span></span> | <span data-ttu-id="1b260-117">Indica se a função de usuário padrão pode ler outros usuários.</span><span class="sxs-lookup"><span data-stu-id="1b260-117">Indicates whether the default user role can read other users.</span></span> |  

## <a name="relationships"></a><span data-ttu-id="1b260-118">Relações</span><span class="sxs-lookup"><span data-stu-id="1b260-118">Relationships</span></span>

<span data-ttu-id="1b260-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1b260-119">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1b260-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1b260-120">JSON representation</span></span>

<span data-ttu-id="1b260-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1b260-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.defaultUserRolePermissions"
}-->

```json
{
  "allowedToCreateApps": true,
  "allowedToCreateSecurityGroups": true,
  "allowedToReadOtherUsers": true
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


