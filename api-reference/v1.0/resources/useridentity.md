---
title: Tipo de recurso userIdentity
description: No contexto de um log de auditoria do Azure AD, isso representa as informações do usuário que iniciaram ou foram afetadas por uma atividade de auditoria.
localization_priority: Normal
author: dhanyahk
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 1abc846321e59434053a7a33b3aa8b993a0f9edc
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136959"
---
# <a name="useridentity-resource-type"></a><span data-ttu-id="b75b6-103">Tipo de recurso userIdentity</span><span class="sxs-lookup"><span data-stu-id="b75b6-103">userIdentity resource type</span></span>

<span data-ttu-id="b75b6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b75b6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b75b6-105">No contexto de um log de auditoria do Azure AD, isso representa as informações do usuário que iniciaram ou foram afetadas por uma atividade de auditoria.</span><span class="sxs-lookup"><span data-stu-id="b75b6-105">In the context of an Azure AD audit log, this represents the user information that initiated or was affected by an audit activity.</span></span>

## <a name="properties"></a><span data-ttu-id="b75b6-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b75b6-106">Properties</span></span>

| <span data-ttu-id="b75b6-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b75b6-107">Property</span></span>     | <span data-ttu-id="b75b6-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="b75b6-108">Type</span></span>   |<span data-ttu-id="b75b6-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b75b6-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b75b6-110">displayName</span><span class="sxs-lookup"><span data-stu-id="b75b6-110">displayName</span></span> | <span data-ttu-id="b75b6-111">String</span><span class="sxs-lookup"><span data-stu-id="b75b6-111">String</span></span> | <span data-ttu-id="b75b6-112">Nome de exibição da identidade.</span><span class="sxs-lookup"><span data-stu-id="b75b6-112">The identity's display name.</span></span> <span data-ttu-id="b75b6-113">Observe que isso pode nem sempre estar disponível ou atualizado.</span><span class="sxs-lookup"><span data-stu-id="b75b6-113">Note that this may not always be available or up-to-date.</span></span>    |
| <span data-ttu-id="b75b6-114">id</span><span class="sxs-lookup"><span data-stu-id="b75b6-114">id</span></span>          | <span data-ttu-id="b75b6-115">String</span><span class="sxs-lookup"><span data-stu-id="b75b6-115">String</span></span> | <span data-ttu-id="b75b6-116">Identificador exclusivo da identidade.</span><span class="sxs-lookup"><span data-stu-id="b75b6-116">Unique identifier for the identity.</span></span>  |
| <span data-ttu-id="b75b6-117">ipAddress</span><span class="sxs-lookup"><span data-stu-id="b75b6-117">ipAddress</span></span>   | <span data-ttu-id="b75b6-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b75b6-118">String</span></span>| <span data-ttu-id="b75b6-119">Indica o endereço IP do cliente usado pelo usuário executando a atividade (somente log de auditoria).</span><span class="sxs-lookup"><span data-stu-id="b75b6-119">Indicates the client IP address used by user performing the activity (audit log only).</span></span>|
| <span data-ttu-id="b75b6-120">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b75b6-120">userPrincipalName</span></span> | <span data-ttu-id="b75b6-121">String</span><span class="sxs-lookup"><span data-stu-id="b75b6-121">String</span></span>  | <span data-ttu-id="b75b6-122">O atributo userPrincipalName do usuário.</span><span class="sxs-lookup"><span data-stu-id="b75b6-122">The userPrincipalName attribute of the user.</span></span> |

><span data-ttu-id="b75b6-123">**Observação:** Em alguns casos, o identificador exclusivo pode não estar disponível.</span><span class="sxs-lookup"><span data-stu-id="b75b6-123">**Note:** In some cases, the unique identifier might not be available.</span></span> <span data-ttu-id="b75b6-124">Nesse caso, a propriedade **displayName** para a identidade será retornada, mas a propriedade **id** estará ausente do recurso.</span><span class="sxs-lookup"><span data-stu-id="b75b6-124">In this case, the **displayName** property for the identity will be returned, but the **id** property will be missing from the resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b75b6-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b75b6-125">JSON representation</span></span>

<span data-ttu-id="b75b6-126">Aqui está uma representação JSON do tipo.</span><span class="sxs-lookup"><span data-stu-id="b75b6-126">Here is a JSON representation of the type.</span></span>

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

