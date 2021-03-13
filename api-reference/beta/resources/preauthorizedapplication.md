---
title: Tipo de recurso preAuthorizedApplication
description: Lista os aplicativos cliente pré-autorizados
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 94a8dad23492ca7a145c5839410edf0fd4a34877
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761160"
---
# <a name="preauthorizedapplication-resource-type"></a><span data-ttu-id="5ec3a-103">Tipo de recurso preAuthorizedApplication</span><span class="sxs-lookup"><span data-stu-id="5ec3a-103">preAuthorizedApplication resource type</span></span>

<span data-ttu-id="5ec3a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ec3a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ec3a-105">Lista os aplicativos cliente pré-autorizados com as permissões especificadas para acessar as APIs desse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5ec3a-105">Lists the client applications that are pre-authorized with the specified permissions to access this application's APIs.</span></span> <span data-ttu-id="5ec3a-106">Os usuários não precisam consentir com nenhum aplicativo pré-autorizado (para as permissões especificadas).</span><span class="sxs-lookup"><span data-stu-id="5ec3a-106">Users are not required to consent to any pre-authorized application (for the permissions specified).</span></span> <span data-ttu-id="5ec3a-107">No entanto, quaisquer permissões adicionais não listadas em preAuthorizedApplications (solicitadas por meio do consentimento incremental, por exemplo) exigirão o consentimento do usuário.</span><span class="sxs-lookup"><span data-stu-id="5ec3a-107">However, any additional permissions not listed in preAuthorizedApplications (requested through incremental consent for example) will require user consent.</span></span>

## <a name="properties"></a><span data-ttu-id="5ec3a-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5ec3a-108">Properties</span></span>

| <span data-ttu-id="5ec3a-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5ec3a-109">Property</span></span> | <span data-ttu-id="5ec3a-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="5ec3a-110">Type</span></span> | <span data-ttu-id="5ec3a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ec3a-111">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="5ec3a-112">appId</span><span class="sxs-lookup"><span data-stu-id="5ec3a-112">appId</span></span>|<span data-ttu-id="5ec3a-113">String</span><span class="sxs-lookup"><span data-stu-id="5ec3a-113">String</span></span>| <span data-ttu-id="5ec3a-114">O identificador exclusivo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5ec3a-114">The unique identifier for the application.</span></span> |
|<span data-ttu-id="5ec3a-115">permissionIds</span><span class="sxs-lookup"><span data-stu-id="5ec3a-115">permissionIds</span></span>|<span data-ttu-id="5ec3a-116">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="5ec3a-116">String collection</span></span>| <span data-ttu-id="5ec3a-117">O identificador exclusivo para [o oauth2PermissionScopes](permissionscope.md) que o aplicativo requer.</span><span class="sxs-lookup"><span data-stu-id="5ec3a-117">The unique identifier for the [oauth2PermissionScopes](permissionscope.md) the application requires.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5ec3a-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5ec3a-118">JSON representation</span></span>
<span data-ttu-id="5ec3a-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5ec3a-119">Here is a JSON representation of the resource.</span></span>

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


