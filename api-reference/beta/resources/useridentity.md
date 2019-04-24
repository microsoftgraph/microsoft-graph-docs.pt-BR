---
title: tipo userIdentity
description: 'Para as revisões do Azure AD Access, este tipo representa uma identidade de usuário do Azure AD para um revisor de uma revisão do Access.  '
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ab8076c5ff24e20006b5a5569dacf4c45d987512
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32453975"
---
# <a name="useridentity-type"></a><span data-ttu-id="c18c3-103">tipo userIdentity</span><span class="sxs-lookup"><span data-stu-id="c18c3-103">userIdentity type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c18c3-104">Para as revisões do Azure AD [Access](accessreviews-root.md), este tipo representa uma identidade de usuário do Azure ad para um revisor de uma revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="c18c3-104">For the Azure AD [access reviews](accessreviews-root.md), this type represents an Azure AD user identity for a reviewer of an access review.</span></span>  
<span data-ttu-id="c18c3-105">No contexto de um log de auditoria do Azure AD, isso representa as informações do usuário que foram iniciadas ou foram afetadas por uma atividade de auditoria.</span><span class="sxs-lookup"><span data-stu-id="c18c3-105">In the context of an Azure AD audit log, this represents the user information that initiated or was affected by an audit activity.</span></span>

<span data-ttu-id="c18c3-106">Esse tipo herda de [Identity](identity.md) e tem uma propriedade adicional, o nome principal do usuário do usuário.</span><span class="sxs-lookup"><span data-stu-id="c18c3-106">This type inherits from [identity](identity.md) and has one additional property, the user principal name of the user.</span></span>

## <a name="methods"></a><span data-ttu-id="c18c3-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="c18c3-107">Methods</span></span>

<span data-ttu-id="c18c3-108">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c18c3-108">None.</span></span>  <span data-ttu-id="c18c3-109">Você deve incluir objetos desse tipo no corpo de uma solicitação ao [criar um accessReview](../api/accessreview-create.md).</span><span class="sxs-lookup"><span data-stu-id="c18c3-109">You would include objects of this type in the body of a request when [creating an accessReview](../api/accessreview-create.md).</span></span>

## <a name="properties"></a><span data-ttu-id="c18c3-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c18c3-110">Properties</span></span>
| <span data-ttu-id="c18c3-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c18c3-111">Property</span></span>     | <span data-ttu-id="c18c3-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="c18c3-112">Type</span></span>   |<span data-ttu-id="c18c3-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="c18c3-113">Description</span></span>|
|:---------------|:--------|:----------|
| `displayName` | `String` | <span data-ttu-id="c18c3-114">Nome de exibição da identidade.</span><span class="sxs-lookup"><span data-stu-id="c18c3-114">The identity's display name.</span></span> <span data-ttu-id="c18c3-115">Observe que isso pode não estar sempre disponível ou atualizado.</span><span class="sxs-lookup"><span data-stu-id="c18c3-115">Note that this may not always be available or up-to-date.</span></span>    |
| `id`          | `String` | <span data-ttu-id="c18c3-116">Identificador exclusivo da identidade.</span><span class="sxs-lookup"><span data-stu-id="c18c3-116">Unique identifier for the identity.</span></span>  |
| `ipAddress`| `String`| <span data-ttu-id="c18c3-117">Indica o endereço IP do cliente usado pelo usuário que está executando a atividade (log de auditoria somente).</span><span class="sxs-lookup"><span data-stu-id="c18c3-117">Indicates the client IP address used by user performing the activity (audit log only).</span></span>|
| `userPrincipalName`|`String` | <span data-ttu-id="c18c3-118">O atributo userPrincipalName do usuário.</span><span class="sxs-lookup"><span data-stu-id="c18c3-118">The userPrincipalName attribute of the user.</span></span> |

## <a name="remarks"></a><span data-ttu-id="c18c3-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="c18c3-119">Remarks</span></span>

<span data-ttu-id="c18c3-p103">Em algumas circunstâncias, o identificador exclusivo para o ator pode não estar disponível. Nesse caso, a propriedade **displayName** para a identidade será retornada, mas a propriedade **id** estará ausente do recurso.</span><span class="sxs-lookup"><span data-stu-id="c18c3-p103">In some circumstances, the unique identifier for the actor may not be available. In this case, the **displayName** property for the identity will be returned, but the **id** property will be missing from the resource.</span></span>

## <a name="relationships"></a><span data-ttu-id="c18c3-122">Relações</span><span class="sxs-lookup"><span data-stu-id="c18c3-122">Relationships</span></span>

<span data-ttu-id="c18c3-123">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c18c3-123">None.</span></span>

## <a name="see-also"></a><span data-ttu-id="c18c3-124">Ver também</span><span class="sxs-lookup"><span data-stu-id="c18c3-124">See also</span></span>

| <span data-ttu-id="c18c3-125">Método</span><span class="sxs-lookup"><span data-stu-id="c18c3-125">Method</span></span>           | <span data-ttu-id="c18c3-126">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c18c3-126">Return Type</span></span>    |<span data-ttu-id="c18c3-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="c18c3-127">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c18c3-128">Obter revisores do accessReview</span><span class="sxs-lookup"><span data-stu-id="c18c3-128">Get accessReview reviewers</span></span>](../api/accessreview-listreviewers.md) |       <span data-ttu-id="c18c3-129">[](useridentity.md) coleção UserIdentity</span><span class="sxs-lookup"><span data-stu-id="c18c3-129">[userIdentity](useridentity.md) collection</span></span>| <span data-ttu-id="c18c3-130">Obter os revisores de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="c18c3-130">Get the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="c18c3-131">Adicionar revisor accessReview</span><span class="sxs-lookup"><span data-stu-id="c18c3-131">Add accessReview reviewer</span></span>](../api/accessreview-addreviewer.md) |      <span data-ttu-id="c18c3-132">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c18c3-132">None.</span></span>   |   <span data-ttu-id="c18c3-133">Adicionar um revisor a um accessReview.</span><span class="sxs-lookup"><span data-stu-id="c18c3-133">Add a reviewer to an accessReview.</span></span> |
|[<span data-ttu-id="c18c3-134">Remover revisor accessReview</span><span class="sxs-lookup"><span data-stu-id="c18c3-134">Remove accessReview reviewer</span></span>](../api/accessreview-removereviewer.md) | <span data-ttu-id="c18c3-135">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c18c3-135">None.</span></span>  |   <span data-ttu-id="c18c3-136">Remover um revisor de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="c18c3-136">Remove a reviewer from an accessReview.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c18c3-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c18c3-137">JSON representation</span></span>

<span data-ttu-id="c18c3-138">Veja a seguir uma representação JSON do tipo.</span><span class="sxs-lookup"><span data-stu-id="c18c3-138">Here is a JSON representation of the type.</span></span>

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
 "userPrincipalName": "String"
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
