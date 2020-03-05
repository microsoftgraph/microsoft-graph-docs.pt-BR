---
title: tipo de recurso Preauthorizedapplication e
description: Lista os aplicativos cliente pré autorizados
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 69ff3d775d4cf3aa767e5e226e688334fcc9f542
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447077"
---
# <a name="preauthorizedapplication-resource-type"></a><span data-ttu-id="e1ced-103">tipo de recurso Preauthorizedapplication e</span><span class="sxs-lookup"><span data-stu-id="e1ced-103">preAuthorizedApplication resource type</span></span>

<span data-ttu-id="e1ced-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e1ced-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e1ced-105">Lista os aplicativos clientes que são previamente autorizados com as permissões especificadas para acessar as APIs desse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e1ced-105">Lists the client applications that are pre-authorized with the specified permissions to access this application's APIs.</span></span> <span data-ttu-id="e1ced-106">Os usuários não precisam ser consentidos em qualquer aplicativo pré autorizado (para as permissões especificadas).</span><span class="sxs-lookup"><span data-stu-id="e1ced-106">Users are not required to consent to any pre-authorized application (for the permissions specified).</span></span> <span data-ttu-id="e1ced-107">No entanto, qualquer permissão adicional que não esteja listada no preAuthorizedApplications (solicitado por meio de consentimento incremental, por exemplo) exigirá o consentimento do usuário.</span><span class="sxs-lookup"><span data-stu-id="e1ced-107">However, any additional permissions not listed in preAuthorizedApplications (requested through incremental consent for example) will require user consent.</span></span>

## <a name="properties"></a><span data-ttu-id="e1ced-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e1ced-108">Properties</span></span>

| <span data-ttu-id="e1ced-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e1ced-109">Property</span></span> | <span data-ttu-id="e1ced-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="e1ced-110">Type</span></span> | <span data-ttu-id="e1ced-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1ced-111">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="e1ced-112">appId</span><span class="sxs-lookup"><span data-stu-id="e1ced-112">appId</span></span>|<span data-ttu-id="e1ced-113">String</span><span class="sxs-lookup"><span data-stu-id="e1ced-113">String</span></span>| <span data-ttu-id="e1ced-114">O identificador exclusivo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e1ced-114">The unique identifier for the application.</span></span> |
|<span data-ttu-id="e1ced-115">delegatedPermissionIds</span><span class="sxs-lookup"><span data-stu-id="e1ced-115">delegatedPermissionIds</span></span>|<span data-ttu-id="e1ced-116">String collection</span><span class="sxs-lookup"><span data-stu-id="e1ced-116">String collection</span></span>| <span data-ttu-id="e1ced-117">O identificador exclusivo para o [oauth2PermissionScopes](permissionscope.md) que o aplicativo exige.</span><span class="sxs-lookup"><span data-stu-id="e1ced-117">The unique identifier for the [oauth2PermissionScopes](permissionscope.md) the application requires.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e1ced-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e1ced-118">JSON representation</span></span>
<span data-ttu-id="e1ced-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e1ced-119">Here is a JSON representation of the resource.</span></span>

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
