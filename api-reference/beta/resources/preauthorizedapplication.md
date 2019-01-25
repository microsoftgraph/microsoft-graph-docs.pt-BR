---
title: tipo de recurso de preAuthorizedApplication
description: Representa um aplicativo e as permissões solicitadas para consentimento implícito. Requer um administrador tenha fornecido a consentimento para o aplicativo. preAuthorizedApplications não exigem o usuário concorda com as permissões solicitadas. Permissões listadas na preAuthorizedApplications não exigem consentimento do usuário. No entanto, qualquer permissões solicitadas adicionais não listados no preAuthorizedApplications exigem o consentimento do usuário.
localization_priority: Normal
ms.openlocfilehash: 22945589341066f4609d47773cb04426774648fd
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524545"
---
# <a name="preauthorizedapplication-resource-type"></a><span data-ttu-id="9bd15-107">tipo de recurso de preAuthorizedApplication</span><span class="sxs-lookup"><span data-stu-id="9bd15-107">preAuthorizedApplication resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9bd15-108">Representa um aplicativo e as permissões solicitadas para consentimento implícito.</span><span class="sxs-lookup"><span data-stu-id="9bd15-108">Represents an application and requested permissions for implicit consent.</span></span> <span data-ttu-id="9bd15-109">Requer um administrador tenha fornecido a consentimento para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9bd15-109">Requires an admin to have provided consent to the application.</span></span> <span data-ttu-id="9bd15-110">preAuthorizedApplications não exigem o usuário concorda com as permissões solicitadas.</span><span class="sxs-lookup"><span data-stu-id="9bd15-110">preAuthorizedApplications do not require the user to consent to the requested permissions.</span></span> <span data-ttu-id="9bd15-111">Permissões listadas na preAuthorizedApplications não exigem consentimento do usuário.</span><span class="sxs-lookup"><span data-stu-id="9bd15-111">Permissions listed in preAuthorizedApplications do not require user consent.</span></span> <span data-ttu-id="9bd15-112">No entanto, qualquer permissões solicitadas adicionais não listados no preAuthorizedApplications exigem o consentimento do usuário.</span><span class="sxs-lookup"><span data-stu-id="9bd15-112">However, any additional requested permissions not listed in preAuthorizedApplications require user consent.</span></span>

## <a name="properties"></a><span data-ttu-id="9bd15-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9bd15-113">Properties</span></span>

| <span data-ttu-id="9bd15-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9bd15-114">Property</span></span> | <span data-ttu-id="9bd15-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="9bd15-115">Type</span></span> | <span data-ttu-id="9bd15-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="9bd15-116">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="9bd15-117">appId</span><span class="sxs-lookup"><span data-stu-id="9bd15-117">appId</span></span>|<span data-ttu-id="9bd15-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9bd15-118">String</span></span>| <span data-ttu-id="9bd15-119">O identificador exclusivo para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9bd15-119">The unique identifier for the application.</span></span> |
|<span data-ttu-id="9bd15-120">permissionIds</span><span class="sxs-lookup"><span data-stu-id="9bd15-120">permissionIds</span></span>|<span data-ttu-id="9bd15-121">String collection</span><span class="sxs-lookup"><span data-stu-id="9bd15-121">String collection</span></span>| <span data-ttu-id="9bd15-122">O identificador exclusivo para o [publishedPermissionScope](permissionscope.md) ou [appRole](approle.md) o aplicativo requer.</span><span class="sxs-lookup"><span data-stu-id="9bd15-122">The unique identifier for either the [publishedPermissionScope](permissionscope.md) or [appRole](approle.md) the application requires.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9bd15-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9bd15-123">JSON representation</span></span>
<span data-ttu-id="9bd15-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9bd15-124">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/preauthorizedapplication.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
