---
title: tipo de recurso Preauthorizedapplication e
description: Lista os aplicativos cliente pré autorizados
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: b883da18f862f91fa2e71a56dc18acb407f208fd
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937417"
---
# <a name="preauthorizedapplication-resource-type"></a><span data-ttu-id="c7a62-103">tipo de recurso Preauthorizedapplication e</span><span class="sxs-lookup"><span data-stu-id="c7a62-103">preAuthorizedApplication resource type</span></span>

<span data-ttu-id="c7a62-104">Lista os aplicativos clientes que são previamente autorizados com as permissões especificadas para acessar as APIs desse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c7a62-104">Lists the client applications that are pre-authorized with the specified permissions to access this application's APIs.</span></span> <span data-ttu-id="c7a62-105">Os usuários não precisam ser consentidos em qualquer aplicativo pré autorizado (para as permissões especificadas).</span><span class="sxs-lookup"><span data-stu-id="c7a62-105">Users are not required to consent to any pre-authorized application (for the permissions specified).</span></span> <span data-ttu-id="c7a62-106">No entanto, qualquer permissão adicional que não esteja listada no preAuthorizedApplications (solicitado por meio de consentimento incremental, por exemplo) exigirá o consentimento do usuário.</span><span class="sxs-lookup"><span data-stu-id="c7a62-106">However, any additional permissions not listed in preAuthorizedApplications (requested through incremental consent for example) will require user consent.</span></span>

## <a name="properties"></a><span data-ttu-id="c7a62-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c7a62-107">Properties</span></span>

| <span data-ttu-id="c7a62-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c7a62-108">Property</span></span> | <span data-ttu-id="c7a62-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="c7a62-109">Type</span></span> | <span data-ttu-id="c7a62-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7a62-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="c7a62-111">appId</span><span class="sxs-lookup"><span data-stu-id="c7a62-111">appId</span></span>|<span data-ttu-id="c7a62-112">String</span><span class="sxs-lookup"><span data-stu-id="c7a62-112">String</span></span>| <span data-ttu-id="c7a62-113">O identificador exclusivo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c7a62-113">The unique identifier for the application.</span></span> |
|<span data-ttu-id="c7a62-114">delegatedPermissionIds</span><span class="sxs-lookup"><span data-stu-id="c7a62-114">delegatedPermissionIds</span></span>|<span data-ttu-id="c7a62-115">String collection</span><span class="sxs-lookup"><span data-stu-id="c7a62-115">String collection</span></span>| <span data-ttu-id="c7a62-116">O identificador exclusivo para o [oauth2PermissionScopes](permissionscope.md) que o aplicativo exige.</span><span class="sxs-lookup"><span data-stu-id="c7a62-116">The unique identifier for the [oauth2PermissionScopes](permissionscope.md) the application requires.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c7a62-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c7a62-117">JSON representation</span></span>
<span data-ttu-id="c7a62-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c7a62-118">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.preAuthorizedApplication"
}-->

```json
{
  "appId": "String",
  "delegatedPermissionIds": ["String"]
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
