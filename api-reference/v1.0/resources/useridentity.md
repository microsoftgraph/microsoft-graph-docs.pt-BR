---
title: tipo de recurso UserIdentity
description: No contexto de um log de auditoria do Azure AD, isso representa as informações do usuário que foram iniciadas ou foram afetadas por uma atividade de auditoria.
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0e72f5338f7281188b7023aed342dd34ee57595e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033499"
---
# <a name="useridentity-resource-type"></a><span data-ttu-id="70e79-103">tipo de recurso UserIdentity</span><span class="sxs-lookup"><span data-stu-id="70e79-103">userIdentity resource type</span></span>

<span data-ttu-id="70e79-104">No contexto de um log de auditoria do Azure AD, isso representa as informações do usuário que foram iniciadas ou foram afetadas por uma atividade de auditoria.</span><span class="sxs-lookup"><span data-stu-id="70e79-104">In the context of an Azure AD audit log, this represents the user information that initiated or was affected by an audit activity.</span></span>

## <a name="properties"></a><span data-ttu-id="70e79-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="70e79-105">Properties</span></span>

| <span data-ttu-id="70e79-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="70e79-106">Property</span></span>     | <span data-ttu-id="70e79-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="70e79-107">Type</span></span>   |<span data-ttu-id="70e79-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="70e79-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="70e79-109">displayName</span><span class="sxs-lookup"><span data-stu-id="70e79-109">displayName</span></span> | <span data-ttu-id="70e79-110">String</span><span class="sxs-lookup"><span data-stu-id="70e79-110">String</span></span> | <span data-ttu-id="70e79-111">Nome de exibição da identidade.</span><span class="sxs-lookup"><span data-stu-id="70e79-111">The identity's display name.</span></span> <span data-ttu-id="70e79-112">Observe que isso pode não estar sempre disponível ou atualizado.</span><span class="sxs-lookup"><span data-stu-id="70e79-112">Note that this may not always be available or up-to-date.</span></span>    |
| <span data-ttu-id="70e79-113">id</span><span class="sxs-lookup"><span data-stu-id="70e79-113">id</span></span>          | <span data-ttu-id="70e79-114">String</span><span class="sxs-lookup"><span data-stu-id="70e79-114">String</span></span> | <span data-ttu-id="70e79-115">Identificador exclusivo da identidade.</span><span class="sxs-lookup"><span data-stu-id="70e79-115">Unique identifier for the identity.</span></span>  |
| <span data-ttu-id="70e79-116">ipAddress</span><span class="sxs-lookup"><span data-stu-id="70e79-116">ipAddress</span></span>   | <span data-ttu-id="70e79-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="70e79-117">String</span></span>| <span data-ttu-id="70e79-118">Indica o endereço IP do cliente usado pelo usuário que está executando a atividade (log de auditoria somente).</span><span class="sxs-lookup"><span data-stu-id="70e79-118">Indicates the client IP address used by user performing the activity (audit log only).</span></span>|
| <span data-ttu-id="70e79-119">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="70e79-119">userPrincipalName</span></span> | <span data-ttu-id="70e79-120">String</span><span class="sxs-lookup"><span data-stu-id="70e79-120">String</span></span>  | <span data-ttu-id="70e79-121">O atributo userPrincipalName do usuário.</span><span class="sxs-lookup"><span data-stu-id="70e79-121">The userPrincipalName attribute of the user.</span></span> |

><span data-ttu-id="70e79-122">**Observação:** Em alguns casos, o identificador exclusivo pode não estar disponível.</span><span class="sxs-lookup"><span data-stu-id="70e79-122">**Note:** In some cases, the unique identifier might not be available.</span></span> <span data-ttu-id="70e79-123">Nesse caso, a propriedade **displayName** para a identidade será retornada, mas a propriedade **id** estará ausente do recurso.</span><span class="sxs-lookup"><span data-stu-id="70e79-123">In this case, the **displayName** property for the identity will be returned, but the **id** property will be missing from the resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="70e79-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="70e79-124">JSON representation</span></span>

<span data-ttu-id="70e79-125">Veja a seguir uma representação JSON do tipo.</span><span class="sxs-lookup"><span data-stu-id="70e79-125">Here is a JSON representation of the type.</span></span>

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
