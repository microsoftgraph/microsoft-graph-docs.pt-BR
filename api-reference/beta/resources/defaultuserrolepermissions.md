---
title: tipo de recurso defaultUserRolePermissions
description: Contém determinadas permissões personalizáveis de função de usuário padrão.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8ee3df9779d5c69ec35bdc4ac9d373554cb0728e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48049944"
---
# <a name="defaultuserrolepermissions-resource-type"></a><span data-ttu-id="f49d5-103">tipo de recurso defaultUserRolePermissions</span><span class="sxs-lookup"><span data-stu-id="f49d5-103">defaultUserRolePermissions resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f49d5-104">Contém determinadas permissões personalizáveis da função de usuário padrão no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f49d5-104">Contains certains customizable permissions of default user role in Azure AD.</span></span>

## <a name="properties"></a><span data-ttu-id="f49d5-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f49d5-105">Properties</span></span>

| <span data-ttu-id="f49d5-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f49d5-106">Property</span></span> | <span data-ttu-id="f49d5-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="f49d5-107">Type</span></span> | <span data-ttu-id="f49d5-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="f49d5-108">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="f49d5-109">allowedToCreateApps</span><span class="sxs-lookup"><span data-stu-id="f49d5-109">allowedToCreateApps</span></span> | <span data-ttu-id="f49d5-110">Booliano</span><span class="sxs-lookup"><span data-stu-id="f49d5-110">Boolean</span></span> | <span data-ttu-id="f49d5-111">Indica se a função de usuário padrão pode criar aplicativos.</span><span class="sxs-lookup"><span data-stu-id="f49d5-111">Indicates whether the default user role can create applications.</span></span> |  
| <span data-ttu-id="f49d5-112">allowedToCreateSecurityGroups</span><span class="sxs-lookup"><span data-stu-id="f49d5-112">allowedToCreateSecurityGroups</span></span> | <span data-ttu-id="f49d5-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="f49d5-113">Boolean</span></span> | <span data-ttu-id="f49d5-114">Indica se a função de usuário padrão pode criar grupos de segurança.</span><span class="sxs-lookup"><span data-stu-id="f49d5-114">Indicates whether the default user role can create security groups.</span></span> |  
| <span data-ttu-id="f49d5-115">allowedToReadOtherUsers</span><span class="sxs-lookup"><span data-stu-id="f49d5-115">allowedToReadOtherUsers</span></span> | <span data-ttu-id="f49d5-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="f49d5-116">Boolean</span></span> | <span data-ttu-id="f49d5-117">Indica se a função de usuário padrão pode ler outros usuários.</span><span class="sxs-lookup"><span data-stu-id="f49d5-117">Indicates whether the default user role can read other users.</span></span> |  

## <a name="relationships"></a><span data-ttu-id="f49d5-118">Relações</span><span class="sxs-lookup"><span data-stu-id="f49d5-118">Relationships</span></span>

<span data-ttu-id="f49d5-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f49d5-119">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f49d5-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f49d5-120">JSON representation</span></span>

<span data-ttu-id="f49d5-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f49d5-121">The following is a JSON representation of the resource.</span></span>

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


