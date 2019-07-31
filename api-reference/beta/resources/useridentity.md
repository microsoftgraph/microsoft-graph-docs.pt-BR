---
title: tipo UserIdentity
description: 'Para as revisões do Azure AD Access, este tipo representa uma identidade de usuário do Azure AD para um revisor de uma revisão do Access.  '
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 21342efd10f5e6f66db795a781eb3f0e333975a2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007449"
---
# <a name="useridentity-type"></a><span data-ttu-id="b1aec-103">tipo UserIdentity</span><span class="sxs-lookup"><span data-stu-id="b1aec-103">userIdentity type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1aec-104">Para as revisões do Azure AD [Access](accessreviews-root.md), este tipo representa uma identidade de usuário do Azure ad para um criador ou revisor de uma revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="b1aec-104">For the Azure AD [access reviews](accessreviews-root.md), this type represents an Azure AD user identity for a creator or reviewer of an access review.</span></span>  
<span data-ttu-id="b1aec-105">No contexto de um log de auditoria do Azure AD, isso representa as informações do usuário que foram iniciadas ou foram afetadas por uma atividade de auditoria.</span><span class="sxs-lookup"><span data-stu-id="b1aec-105">In the context of an Azure AD audit log, this represents the user information that initiated or was affected by an audit activity.</span></span>

<span data-ttu-id="b1aec-106">Esse tipo herda de [Identity](identity.md) e tem uma propriedade adicional, o nome principal do usuário do usuário.</span><span class="sxs-lookup"><span data-stu-id="b1aec-106">This type inherits from [identity](identity.md) and has one additional property, the user principal name of the user.</span></span>

## <a name="methods"></a><span data-ttu-id="b1aec-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="b1aec-107">Methods</span></span>

<span data-ttu-id="b1aec-108">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b1aec-108">None.</span></span>  <span data-ttu-id="b1aec-109">Você deve incluir objetos desse tipo no corpo de uma solicitação ao [criar um accessReview](../api/accessreview-create.md).</span><span class="sxs-lookup"><span data-stu-id="b1aec-109">You would include objects of this type in the body of a request when [creating an accessReview](../api/accessreview-create.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b1aec-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b1aec-110">Properties</span></span>
| <span data-ttu-id="b1aec-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b1aec-111">Property</span></span>     | <span data-ttu-id="b1aec-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="b1aec-112">Type</span></span>   |<span data-ttu-id="b1aec-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1aec-113">Description</span></span>|
|:---------------|:--------|:----------|
| `displayName` | `String` | <span data-ttu-id="b1aec-114">Nome de exibição da identidade.</span><span class="sxs-lookup"><span data-stu-id="b1aec-114">The identity's display name.</span></span> <span data-ttu-id="b1aec-115">Observe que isso pode não estar sempre disponível ou atualizado.</span><span class="sxs-lookup"><span data-stu-id="b1aec-115">Note that this may not always be available or up-to-date.</span></span>    |
| `id`          | `String` | <span data-ttu-id="b1aec-116">Identificador exclusivo da identidade.</span><span class="sxs-lookup"><span data-stu-id="b1aec-116">Unique identifier for the identity.</span></span>  |
| `ipAddress`| `String`| <span data-ttu-id="b1aec-117">Indica o endereço IP do cliente usado pelo usuário que está executando a atividade (log de auditoria somente).</span><span class="sxs-lookup"><span data-stu-id="b1aec-117">Indicates the client IP address used by user performing the activity (audit log only).</span></span>|
| `userPrincipalName`|`String` | <span data-ttu-id="b1aec-118">O atributo userPrincipalName do usuário.</span><span class="sxs-lookup"><span data-stu-id="b1aec-118">The userPrincipalName attribute of the user.</span></span> |

## <a name="remarks"></a><span data-ttu-id="b1aec-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="b1aec-119">Remarks</span></span>

<span data-ttu-id="b1aec-p103">Em algumas circunstâncias, o identificador exclusivo para o ator pode não estar disponível. Nesse caso, a propriedade **displayName** para a identidade será retornada, mas a propriedade **id** estará ausente do recurso.</span><span class="sxs-lookup"><span data-stu-id="b1aec-p103">In some circumstances, the unique identifier for the actor may not be available. In this case, the **displayName** property for the identity will be returned, but the **id** property will be missing from the resource.</span></span>

## <a name="relationships"></a><span data-ttu-id="b1aec-122">Relações</span><span class="sxs-lookup"><span data-stu-id="b1aec-122">Relationships</span></span>

<span data-ttu-id="b1aec-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b1aec-123">None.</span></span>

## <a name="see-also"></a><span data-ttu-id="b1aec-124">Ver também</span><span class="sxs-lookup"><span data-stu-id="b1aec-124">See also</span></span>

| <span data-ttu-id="b1aec-125">Método</span><span class="sxs-lookup"><span data-stu-id="b1aec-125">Method</span></span>           | <span data-ttu-id="b1aec-126">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b1aec-126">Return Type</span></span>    |<span data-ttu-id="b1aec-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1aec-127">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b1aec-128">Obter revisores do accessReview</span><span class="sxs-lookup"><span data-stu-id="b1aec-128">Get accessReview reviewers</span></span>](../api/accessreview-listreviewers.md) |       <span data-ttu-id="b1aec-129">[](useridentity.md) coleção UserIdentity</span><span class="sxs-lookup"><span data-stu-id="b1aec-129">[userIdentity](useridentity.md) collection</span></span>| <span data-ttu-id="b1aec-130">Obter os revisores de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="b1aec-130">Get the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="b1aec-131">Adicionar revisor accessReview</span><span class="sxs-lookup"><span data-stu-id="b1aec-131">Add accessReview reviewer</span></span>](../api/accessreview-addreviewer.md) |      <span data-ttu-id="b1aec-132">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b1aec-132">None.</span></span>   |   <span data-ttu-id="b1aec-133">Adicionar um revisor a um accessReview.</span><span class="sxs-lookup"><span data-stu-id="b1aec-133">Add a reviewer to an accessReview.</span></span> |
|[<span data-ttu-id="b1aec-134">Remover revisor accessReview</span><span class="sxs-lookup"><span data-stu-id="b1aec-134">Remove accessReview reviewer</span></span>](../api/accessreview-removereviewer.md) | <span data-ttu-id="b1aec-135">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b1aec-135">None.</span></span>  |   <span data-ttu-id="b1aec-136">Remover um revisor de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="b1aec-136">Remove a reviewer from an accessReview.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b1aec-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b1aec-137">JSON representation</span></span>

<span data-ttu-id="b1aec-138">Veja a seguir uma representação JSON do tipo.</span><span class="sxs-lookup"><span data-stu-id="b1aec-138">Here is a JSON representation of the type.</span></span>

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
  "userPrincipalName": "String",
  "ipAddress": "string"
}

```

<!--
{
  "type": "#page.annotation",
  "description": "userIdentity type",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
