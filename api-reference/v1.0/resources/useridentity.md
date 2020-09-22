---
title: tipo de recurso UserIdentity
description: No contexto de um log de auditoria do Azure AD, isso representa as informações do usuário que foram iniciadas ou foram afetadas por uma atividade de auditoria.
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 32bfb6d7a92ce566d10809277f19f82e45ffc1a1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48015383"
---
# <a name="useridentity-resource-type"></a><span data-ttu-id="27c0f-103">tipo de recurso UserIdentity</span><span class="sxs-lookup"><span data-stu-id="27c0f-103">userIdentity resource type</span></span>

<span data-ttu-id="27c0f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="27c0f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="27c0f-105">No contexto de um log de auditoria do Azure AD, isso representa as informações do usuário que foram iniciadas ou foram afetadas por uma atividade de auditoria.</span><span class="sxs-lookup"><span data-stu-id="27c0f-105">In the context of an Azure AD audit log, this represents the user information that initiated or was affected by an audit activity.</span></span>

## <a name="properties"></a><span data-ttu-id="27c0f-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="27c0f-106">Properties</span></span>

| <span data-ttu-id="27c0f-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="27c0f-107">Property</span></span>     | <span data-ttu-id="27c0f-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="27c0f-108">Type</span></span>   |<span data-ttu-id="27c0f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="27c0f-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="27c0f-110">displayName</span><span class="sxs-lookup"><span data-stu-id="27c0f-110">displayName</span></span> | <span data-ttu-id="27c0f-111">String</span><span class="sxs-lookup"><span data-stu-id="27c0f-111">String</span></span> | <span data-ttu-id="27c0f-112">Nome de exibição da identidade.</span><span class="sxs-lookup"><span data-stu-id="27c0f-112">The identity's display name.</span></span> <span data-ttu-id="27c0f-113">Observe que isso pode não estar sempre disponível ou atualizado.</span><span class="sxs-lookup"><span data-stu-id="27c0f-113">Note that this may not always be available or up-to-date.</span></span>    |
| <span data-ttu-id="27c0f-114">id</span><span class="sxs-lookup"><span data-stu-id="27c0f-114">id</span></span>          | <span data-ttu-id="27c0f-115">String</span><span class="sxs-lookup"><span data-stu-id="27c0f-115">String</span></span> | <span data-ttu-id="27c0f-116">Identificador exclusivo da identidade.</span><span class="sxs-lookup"><span data-stu-id="27c0f-116">Unique identifier for the identity.</span></span>  |
| <span data-ttu-id="27c0f-117">ipAddress</span><span class="sxs-lookup"><span data-stu-id="27c0f-117">ipAddress</span></span>   | <span data-ttu-id="27c0f-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="27c0f-118">String</span></span>| <span data-ttu-id="27c0f-119">Indica o endereço IP do cliente usado pelo usuário que está executando a atividade (log de auditoria somente).</span><span class="sxs-lookup"><span data-stu-id="27c0f-119">Indicates the client IP address used by user performing the activity (audit log only).</span></span>|
| <span data-ttu-id="27c0f-120">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="27c0f-120">userPrincipalName</span></span> | <span data-ttu-id="27c0f-121">String</span><span class="sxs-lookup"><span data-stu-id="27c0f-121">String</span></span>  | <span data-ttu-id="27c0f-122">O atributo userPrincipalName do usuário.</span><span class="sxs-lookup"><span data-stu-id="27c0f-122">The userPrincipalName attribute of the user.</span></span> |

><span data-ttu-id="27c0f-123">**Observação:** Em alguns casos, o identificador exclusivo pode não estar disponível.</span><span class="sxs-lookup"><span data-stu-id="27c0f-123">**Note:** In some cases, the unique identifier might not be available.</span></span> <span data-ttu-id="27c0f-124">Nesse caso, a propriedade **displayName** para a identidade será retornada, mas a propriedade **id** estará ausente do recurso.</span><span class="sxs-lookup"><span data-stu-id="27c0f-124">In this case, the **displayName** property for the identity will be returned, but the **id** property will be missing from the resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="27c0f-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="27c0f-125">JSON representation</span></span>

<span data-ttu-id="27c0f-126">Veja a seguir uma representação JSON do tipo.</span><span class="sxs-lookup"><span data-stu-id="27c0f-126">Here is a JSON representation of the type.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
"displayName", "thumbnails"
  ],
  "@odata.type": "microsoft.graph.userIdentity"
}-->

```json
{
  "displayName": "string",
  "id": "string",
  "ipAddress": "string",
  "userPrincipalName": "string"
}

```

<!--
{
  "type": "#page.annotation",
  "description": "userIdentity type",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/useridentity.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

