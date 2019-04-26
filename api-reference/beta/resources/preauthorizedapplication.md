---
title: tipo de recurso Preauthorizedapplication e
description: Representa um aplicativo e permissões solicitadas para o consentimento implícito. Requer um administrador para ter fornecido o consentimento para o aplicativo. o preAuthorizedApplications não exige que o usuário concorde com as permissões solicitadas. As permissões listadas no preAuthorizedApplications não exigem o consentimento do usuário. No enTanto, as permissões adicionais solicitadas não listadas no preAuthorizedApplications exigem o consentimento do usuário.
localization_priority: Normal
ms.openlocfilehash: f74ac0883c883bfbb2cb93c2da58e9fd8419dadd
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344213"
---
# <a name="preauthorizedapplication-resource-type"></a><span data-ttu-id="31f4a-107">tipo de recurso Preauthorizedapplication e</span><span class="sxs-lookup"><span data-stu-id="31f4a-107">preAuthorizedApplication resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31f4a-108">Representa um aplicativo e permissões solicitadas para o consentimento implícito.</span><span class="sxs-lookup"><span data-stu-id="31f4a-108">Represents an application and requested permissions for implicit consent.</span></span> <span data-ttu-id="31f4a-109">Requer um administrador para ter fornecido o consentimento para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="31f4a-109">Requires an admin to have provided consent to the application.</span></span> <span data-ttu-id="31f4a-110">o preAuthorizedApplications não exige que o usuário concorde com as permissões solicitadas.</span><span class="sxs-lookup"><span data-stu-id="31f4a-110">preAuthorizedApplications do not require the user to consent to the requested permissions.</span></span> <span data-ttu-id="31f4a-111">As permissões listadas no preAuthorizedApplications não exigem o consentimento do usuário.</span><span class="sxs-lookup"><span data-stu-id="31f4a-111">Permissions listed in preAuthorizedApplications do not require user consent.</span></span> <span data-ttu-id="31f4a-112">No enTanto, as permissões adicionais solicitadas não listadas no preAuthorizedApplications exigem o consentimento do usuário.</span><span class="sxs-lookup"><span data-stu-id="31f4a-112">However, any additional requested permissions not listed in preAuthorizedApplications require user consent.</span></span>

## <a name="properties"></a><span data-ttu-id="31f4a-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="31f4a-113">Properties</span></span>

| <span data-ttu-id="31f4a-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="31f4a-114">Property</span></span> | <span data-ttu-id="31f4a-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="31f4a-115">Type</span></span> | <span data-ttu-id="31f4a-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="31f4a-116">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="31f4a-117">appId</span><span class="sxs-lookup"><span data-stu-id="31f4a-117">appId</span></span>|<span data-ttu-id="31f4a-118">String</span><span class="sxs-lookup"><span data-stu-id="31f4a-118">String</span></span>| <span data-ttu-id="31f4a-119">O identificador exclusivo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="31f4a-119">The unique identifier for the application.</span></span> |
|<span data-ttu-id="31f4a-120">permissionIds</span><span class="sxs-lookup"><span data-stu-id="31f4a-120">permissionIds</span></span>|<span data-ttu-id="31f4a-121">Coleção String</span><span class="sxs-lookup"><span data-stu-id="31f4a-121">String collection</span></span>| <span data-ttu-id="31f4a-122">O identificador exclusivo do [publishedPermissionScope](permissionscope.md) ou do [appRole](approle.md) que o aplicativo exige.</span><span class="sxs-lookup"><span data-stu-id="31f4a-122">The unique identifier for either the [publishedPermissionScope](permissionscope.md) or [appRole](approle.md) the application requires.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="31f4a-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="31f4a-123">JSON representation</span></span>
<span data-ttu-id="31f4a-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="31f4a-124">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.preAuthorizedApplication"
}-->

```json
{
  "appId": "String",
  "permissionIds": ["String"]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "preAuthorizedApplication resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
