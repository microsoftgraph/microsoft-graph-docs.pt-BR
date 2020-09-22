---
title: tipo de recurso Preauthorizedapplication e
description: Lista os aplicativos cliente pré autorizados
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: fdc6b9692076040a4495074456f1b847e3af3c69
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037245"
---
# <a name="preauthorizedapplication-resource-type"></a><span data-ttu-id="e06db-103">tipo de recurso Preauthorizedapplication e</span><span class="sxs-lookup"><span data-stu-id="e06db-103">preAuthorizedApplication resource type</span></span>

<span data-ttu-id="e06db-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e06db-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e06db-105">Lista os aplicativos clientes que são previamente autorizados com as permissões especificadas para acessar as APIs desse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e06db-105">Lists the client applications that are pre-authorized with the specified permissions to access this application's APIs.</span></span> <span data-ttu-id="e06db-106">Os usuários não precisam ser consentidos em qualquer aplicativo pré autorizado (para as permissões especificadas).</span><span class="sxs-lookup"><span data-stu-id="e06db-106">Users are not required to consent to any pre-authorized application (for the permissions specified).</span></span> <span data-ttu-id="e06db-107">No entanto, qualquer permissão adicional que não esteja listada no preAuthorizedApplications (solicitado por meio de consentimento incremental, por exemplo) exigirá o consentimento do usuário.</span><span class="sxs-lookup"><span data-stu-id="e06db-107">However, any additional permissions not listed in preAuthorizedApplications (requested through incremental consent for example) will require user consent.</span></span>

## <a name="properties"></a><span data-ttu-id="e06db-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e06db-108">Properties</span></span>

| <span data-ttu-id="e06db-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e06db-109">Property</span></span> | <span data-ttu-id="e06db-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="e06db-110">Type</span></span> | <span data-ttu-id="e06db-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e06db-111">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="e06db-112">appId</span><span class="sxs-lookup"><span data-stu-id="e06db-112">appId</span></span>|<span data-ttu-id="e06db-113">String</span><span class="sxs-lookup"><span data-stu-id="e06db-113">String</span></span>| <span data-ttu-id="e06db-114">O identificador exclusivo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e06db-114">The unique identifier for the application.</span></span> |
|<span data-ttu-id="e06db-115">delegatedPermissionIds</span><span class="sxs-lookup"><span data-stu-id="e06db-115">delegatedPermissionIds</span></span>|<span data-ttu-id="e06db-116">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e06db-116">String collection</span></span>| <span data-ttu-id="e06db-117">O identificador exclusivo para o [oauth2PermissionScopes](permissionscope.md) que o aplicativo exige.</span><span class="sxs-lookup"><span data-stu-id="e06db-117">The unique identifier for the [oauth2PermissionScopes](permissionscope.md) the application requires.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e06db-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e06db-118">JSON representation</span></span>
<span data-ttu-id="e06db-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e06db-119">Here is a JSON representation of the resource.</span></span>

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

