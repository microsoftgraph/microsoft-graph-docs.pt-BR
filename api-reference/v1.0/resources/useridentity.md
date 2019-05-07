---
title: tipo de recurso UserIdentity
description: No contexto de um log de auditoria do Azure AD, isso representa as informações do usuário que foram iniciadas ou foram afetadas por uma atividade de auditoria.
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 018bc8ca3713822295d0acef66e8ec075d276cfe
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629226"
---
# <a name="useridentity-resource-type"></a><span data-ttu-id="41eb1-103">tipo de recurso UserIdentity</span><span class="sxs-lookup"><span data-stu-id="41eb1-103">userIdentity resource type</span></span>

<span data-ttu-id="41eb1-104">No contexto de um log de auditoria do Azure AD, isso representa as informações do usuário que foram iniciadas ou foram afetadas por uma atividade de auditoria.</span><span class="sxs-lookup"><span data-stu-id="41eb1-104">In the context of an Azure AD audit log, this represents the user information that initiated or was affected by an audit activity.</span></span>

## <a name="properties"></a><span data-ttu-id="41eb1-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="41eb1-105">Properties</span></span>

| <span data-ttu-id="41eb1-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="41eb1-106">Property</span></span>     | <span data-ttu-id="41eb1-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="41eb1-107">Type</span></span>   |<span data-ttu-id="41eb1-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="41eb1-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="41eb1-109">displayName</span><span class="sxs-lookup"><span data-stu-id="41eb1-109">displayName</span></span> | <span data-ttu-id="41eb1-110">String</span><span class="sxs-lookup"><span data-stu-id="41eb1-110">String</span></span> | <span data-ttu-id="41eb1-111">Nome de exibição da identidade.</span><span class="sxs-lookup"><span data-stu-id="41eb1-111">The identity's display name.</span></span> <span data-ttu-id="41eb1-112">Observe que isso pode não estar sempre disponível ou atualizado.</span><span class="sxs-lookup"><span data-stu-id="41eb1-112">Note that this may not always be available or up-to-date.</span></span>    |
| <span data-ttu-id="41eb1-113">id</span><span class="sxs-lookup"><span data-stu-id="41eb1-113">id</span></span>          | <span data-ttu-id="41eb1-114">String</span><span class="sxs-lookup"><span data-stu-id="41eb1-114">String</span></span> | <span data-ttu-id="41eb1-115">Identificador exclusivo da identidade.</span><span class="sxs-lookup"><span data-stu-id="41eb1-115">Unique identifier for the identity.</span></span>  |
| <span data-ttu-id="41eb1-116">ipAddress</span><span class="sxs-lookup"><span data-stu-id="41eb1-116">ipAddress</span></span>   | <span data-ttu-id="41eb1-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="41eb1-117">String</span></span>| <span data-ttu-id="41eb1-118">Indica o endereço IP do cliente usado pelo usuário que está executando a atividade (log de auditoria somente).</span><span class="sxs-lookup"><span data-stu-id="41eb1-118">Indicates the client IP address used by user performing the activity (audit log only).</span></span>|
| <span data-ttu-id="41eb1-119">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="41eb1-119">userPrincipalName</span></span> | <span data-ttu-id="41eb1-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="41eb1-120">String</span></span>  | <span data-ttu-id="41eb1-121">O atributo userPrincipalName do usuário.</span><span class="sxs-lookup"><span data-stu-id="41eb1-121">The userPrincipalName attribute of the user.</span></span> |

><span data-ttu-id="41eb1-122">**Observação:** Em alguns casos, o identificador exclusivo pode não estar disponível.</span><span class="sxs-lookup"><span data-stu-id="41eb1-122">**Note:** In some cases, the unique identifier might not be available.</span></span> <span data-ttu-id="41eb1-123">Nesse caso, a propriedade **displayName** para a identidade será retornada, mas a propriedade **id** estará ausente do recurso.</span><span class="sxs-lookup"><span data-stu-id="41eb1-123">In this case, the **displayName** property for the identity will be returned, but the **id** property will be missing from the resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="41eb1-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="41eb1-124">JSON representation</span></span>

<span data-ttu-id="41eb1-125">Veja a seguir uma representação JSON do tipo.</span><span class="sxs-lookup"><span data-stu-id="41eb1-125">Here is a JSON representation of the type.</span></span>

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
