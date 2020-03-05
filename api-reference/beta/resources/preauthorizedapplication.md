---
title: tipo de recurso Preauthorizedapplication e
description: Lista os aplicativos cliente pré autorizados
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: b84e9a49d293978754a06bdae229806f529690ba
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521576"
---
# <a name="preauthorizedapplication-resource-type"></a><span data-ttu-id="ffbf5-103">tipo de recurso Preauthorizedapplication e</span><span class="sxs-lookup"><span data-stu-id="ffbf5-103">preAuthorizedApplication resource type</span></span>

<span data-ttu-id="ffbf5-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ffbf5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ffbf5-105">Lista os aplicativos clientes que são previamente autorizados com as permissões especificadas para acessar as APIs desse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ffbf5-105">Lists the client applications that are pre-authorized with the specified permissions to access this application's APIs.</span></span> <span data-ttu-id="ffbf5-106">Os usuários não precisam ser consentidos em qualquer aplicativo pré autorizado (para as permissões especificadas).</span><span class="sxs-lookup"><span data-stu-id="ffbf5-106">Users are not required to consent to any pre-authorized application (for the permissions specified).</span></span> <span data-ttu-id="ffbf5-107">No entanto, qualquer permissão adicional que não esteja listada no preAuthorizedApplications (solicitado por meio de consentimento incremental, por exemplo) exigirá o consentimento do usuário.</span><span class="sxs-lookup"><span data-stu-id="ffbf5-107">However, any additional permissions not listed in preAuthorizedApplications (requested through incremental consent for example) will require user consent.</span></span>

## <a name="properties"></a><span data-ttu-id="ffbf5-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ffbf5-108">Properties</span></span>

| <span data-ttu-id="ffbf5-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ffbf5-109">Property</span></span> | <span data-ttu-id="ffbf5-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="ffbf5-110">Type</span></span> | <span data-ttu-id="ffbf5-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ffbf5-111">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="ffbf5-112">appId</span><span class="sxs-lookup"><span data-stu-id="ffbf5-112">appId</span></span>|<span data-ttu-id="ffbf5-113">String</span><span class="sxs-lookup"><span data-stu-id="ffbf5-113">String</span></span>| <span data-ttu-id="ffbf5-114">O identificador exclusivo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ffbf5-114">The unique identifier for the application.</span></span> |
|<span data-ttu-id="ffbf5-115">permissionIds</span><span class="sxs-lookup"><span data-stu-id="ffbf5-115">permissionIds</span></span>|<span data-ttu-id="ffbf5-116">String collection</span><span class="sxs-lookup"><span data-stu-id="ffbf5-116">String collection</span></span>| <span data-ttu-id="ffbf5-117">O identificador exclusivo para o [oauth2PermissionScopes](permissionscope.md) que o aplicativo exige.</span><span class="sxs-lookup"><span data-stu-id="ffbf5-117">The unique identifier for the [oauth2PermissionScopes](permissionscope.md) the application requires.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ffbf5-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ffbf5-118">JSON representation</span></span>
<span data-ttu-id="ffbf5-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ffbf5-119">Here is a JSON representation of the resource.</span></span>

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
