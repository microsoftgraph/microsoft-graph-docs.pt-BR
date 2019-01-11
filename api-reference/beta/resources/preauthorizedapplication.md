---
title: tipo de recurso de preAuthorizedApplication
description: Representa um aplicativo e as permissões solicitadas para consentimento implícito. Requer um administrador tenha fornecido a consentimento para o aplicativo. preAuthorizedApplications não exigem o usuário concorda com as permissões solicitadas. Permissões listadas na preAuthorizedApplications não exigem consentimento do usuário. No entanto, qualquer permissões solicitadas adicionais não listados no preAuthorizedApplications exigem o consentimento do usuário.
localization_priority: Normal
ms.openlocfilehash: fa26b8046b81db70300b8ff40abcbd2b84f3f0c8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832792"
---
# <a name="preauthorizedapplication-resource-type"></a><span data-ttu-id="71afb-107">tipo de recurso de preAuthorizedApplication</span><span class="sxs-lookup"><span data-stu-id="71afb-107">preAuthorizedApplication resource type</span></span>

> <span data-ttu-id="71afb-108">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="71afb-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="71afb-109">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="71afb-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="71afb-110">Representa um aplicativo e as permissões solicitadas para consentimento implícito.</span><span class="sxs-lookup"><span data-stu-id="71afb-110">Represents an application and requested permissions for implicit consent.</span></span> <span data-ttu-id="71afb-111">Requer um administrador tenha fornecido a consentimento para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="71afb-111">Requires an admin to have provided consent to the application.</span></span> <span data-ttu-id="71afb-112">preAuthorizedApplications não exigem o usuário concorda com as permissões solicitadas.</span><span class="sxs-lookup"><span data-stu-id="71afb-112">preAuthorizedApplications do not require the user to consent to the requested permissions.</span></span> <span data-ttu-id="71afb-113">Permissões listadas na preAuthorizedApplications não exigem consentimento do usuário.</span><span class="sxs-lookup"><span data-stu-id="71afb-113">Permissions listed in preAuthorizedApplications do not require user consent.</span></span> <span data-ttu-id="71afb-114">No entanto, qualquer permissões solicitadas adicionais não listados no preAuthorizedApplications exigem o consentimento do usuário.</span><span class="sxs-lookup"><span data-stu-id="71afb-114">However, any additional requested permissions not listed in preAuthorizedApplications require user consent.</span></span>

## <a name="properties"></a><span data-ttu-id="71afb-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="71afb-115">Properties</span></span>

| <span data-ttu-id="71afb-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="71afb-116">Property</span></span> | <span data-ttu-id="71afb-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="71afb-117">Type</span></span> | <span data-ttu-id="71afb-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="71afb-118">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="71afb-119">appId</span><span class="sxs-lookup"><span data-stu-id="71afb-119">appId</span></span>|<span data-ttu-id="71afb-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="71afb-120">String</span></span>| <span data-ttu-id="71afb-121">O identificador exclusivo para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="71afb-121">The unique identifier for the application.</span></span> |
|<span data-ttu-id="71afb-122">permissionIds</span><span class="sxs-lookup"><span data-stu-id="71afb-122">permissionIds</span></span>|<span data-ttu-id="71afb-123">String collection</span><span class="sxs-lookup"><span data-stu-id="71afb-123">String collection</span></span>| <span data-ttu-id="71afb-124">O identificador exclusivo para o [publishedPermissionScope](permissionscope.md) ou [appRole](approle.md) o aplicativo requer.</span><span class="sxs-lookup"><span data-stu-id="71afb-124">The unique identifier for either the [publishedPermissionScope](permissionscope.md) or [appRole](approle.md) the application requires.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="71afb-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="71afb-125">JSON representation</span></span>
<span data-ttu-id="71afb-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="71afb-126">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "preAuthorizedApplication resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
