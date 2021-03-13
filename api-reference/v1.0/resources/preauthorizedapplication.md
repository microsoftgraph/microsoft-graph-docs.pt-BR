---
title: Tipo de recurso preAuthorizedApplication
description: Lista os aplicativos cliente pré-autorizados
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 276b6f618b01d80fd66fda40c0b617a8fd01a6ac
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760971"
---
# <a name="preauthorizedapplication-resource-type"></a><span data-ttu-id="02116-103">Tipo de recurso preAuthorizedApplication</span><span class="sxs-lookup"><span data-stu-id="02116-103">preAuthorizedApplication resource type</span></span>

<span data-ttu-id="02116-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02116-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="02116-105">Lista os aplicativos cliente pré-autorizados com as permissões especificadas para acessar as APIs desse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="02116-105">Lists the client applications that are pre-authorized with the specified permissions to access this application's APIs.</span></span> <span data-ttu-id="02116-106">Os usuários não precisam consentir com nenhum aplicativo pré-autorizado (para as permissões especificadas).</span><span class="sxs-lookup"><span data-stu-id="02116-106">Users are not required to consent to any pre-authorized application (for the permissions specified).</span></span> <span data-ttu-id="02116-107">No entanto, quaisquer permissões adicionais não listadas em preAuthorizedApplications (solicitadas por meio do consentimento incremental, por exemplo) exigirão o consentimento do usuário.</span><span class="sxs-lookup"><span data-stu-id="02116-107">However, any additional permissions not listed in preAuthorizedApplications (requested through incremental consent for example) will require user consent.</span></span>

## <a name="properties"></a><span data-ttu-id="02116-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="02116-108">Properties</span></span>

| <span data-ttu-id="02116-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="02116-109">Property</span></span> | <span data-ttu-id="02116-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="02116-110">Type</span></span> | <span data-ttu-id="02116-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="02116-111">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="02116-112">appId</span><span class="sxs-lookup"><span data-stu-id="02116-112">appId</span></span>|<span data-ttu-id="02116-113">String</span><span class="sxs-lookup"><span data-stu-id="02116-113">String</span></span>| <span data-ttu-id="02116-114">O identificador exclusivo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="02116-114">The unique identifier for the application.</span></span> |
|<span data-ttu-id="02116-115">delegatedPermissionIds</span><span class="sxs-lookup"><span data-stu-id="02116-115">delegatedPermissionIds</span></span>|<span data-ttu-id="02116-116">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="02116-116">String collection</span></span>| <span data-ttu-id="02116-117">O identificador exclusivo para [o oauth2PermissionScopes](permissionscope.md) que o aplicativo requer.</span><span class="sxs-lookup"><span data-stu-id="02116-117">The unique identifier for the [oauth2PermissionScopes](permissionscope.md) the application requires.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="02116-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="02116-118">JSON representation</span></span>
<span data-ttu-id="02116-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="02116-119">Here is a JSON representation of the resource.</span></span>

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

