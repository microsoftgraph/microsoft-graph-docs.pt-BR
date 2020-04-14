---
title: tipo UserIdentity
description: Representa uma identidade de usuário do Azure AD para um revisor de uma revisão do Access.
localization_priority: Normal
author: krbain
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0cb40f4d9815ed0c95f319fd5f112dfd5802f10a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43384967"
---
# <a name="useridentity-type"></a><span data-ttu-id="a0291-103">tipo UserIdentity</span><span class="sxs-lookup"><span data-stu-id="a0291-103">userIdentity type</span></span>

<span data-ttu-id="a0291-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0291-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0291-105">Para as revisões do Azure AD [Access](accessreviews-root.md), este tipo representa uma identidade de usuário do Azure ad para um criador ou revisor de uma revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="a0291-105">For the Azure AD [access reviews](accessreviews-root.md), this type represents an Azure AD user identity for a creator or reviewer of an access review.</span></span>  
<span data-ttu-id="a0291-106">No contexto de um log de auditoria do Azure AD, isso representa as informações do usuário que foram iniciadas ou foram afetadas por uma atividade de auditoria.</span><span class="sxs-lookup"><span data-stu-id="a0291-106">In the context of an Azure AD audit log, this represents the user information that initiated or was affected by an audit activity.</span></span>

<span data-ttu-id="a0291-107">Esse tipo herda de [Identity](identity.md) e tem uma propriedade adicional, o nome principal do usuário do usuário.</span><span class="sxs-lookup"><span data-stu-id="a0291-107">This type inherits from [identity](identity.md) and has one additional property, the user principal name of the user.</span></span>

## <a name="methods"></a><span data-ttu-id="a0291-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="a0291-108">Methods</span></span>

<span data-ttu-id="a0291-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a0291-109">None.</span></span>  <span data-ttu-id="a0291-110">Você deve incluir objetos desse tipo no corpo de uma solicitação ao [criar um accessReview](../api/accessreview-create.md).</span><span class="sxs-lookup"><span data-stu-id="a0291-110">You would include objects of this type in the body of a request when [creating an accessReview](../api/accessreview-create.md).</span></span>

## <a name="properties"></a><span data-ttu-id="a0291-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a0291-111">Properties</span></span>
| <span data-ttu-id="a0291-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a0291-112">Property</span></span>     | <span data-ttu-id="a0291-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="a0291-113">Type</span></span>   |<span data-ttu-id="a0291-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0291-114">Description</span></span>|
|:---------------|:--------|:----------|
| `displayName` | `String` | <span data-ttu-id="a0291-115">Nome de exibição da identidade.</span><span class="sxs-lookup"><span data-stu-id="a0291-115">The identity's display name.</span></span> <span data-ttu-id="a0291-116">Observe que isso pode não estar sempre disponível ou atualizado.</span><span class="sxs-lookup"><span data-stu-id="a0291-116">Note that this may not always be available or up-to-date.</span></span>    |
| `id`          | `String` | <span data-ttu-id="a0291-117">Identificador exclusivo da identidade.</span><span class="sxs-lookup"><span data-stu-id="a0291-117">Unique identifier for the identity.</span></span>  |
| `ipAddress`| `String`| <span data-ttu-id="a0291-118">Indica o endereço IP do cliente usado pelo usuário que está executando a atividade (log de auditoria somente).</span><span class="sxs-lookup"><span data-stu-id="a0291-118">Indicates the client IP address used by user performing the activity (audit log only).</span></span>|
| `userPrincipalName`|`String` | <span data-ttu-id="a0291-119">O atributo userPrincipalName do usuário.</span><span class="sxs-lookup"><span data-stu-id="a0291-119">The userPrincipalName attribute of the user.</span></span> |

## <a name="remarks"></a><span data-ttu-id="a0291-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="a0291-120">Remarks</span></span>

<span data-ttu-id="a0291-p103">Em algumas circunstâncias, o identificador exclusivo para o ator pode não estar disponível. Nesse caso, a propriedade **displayName** para a identidade será retornada, mas a propriedade **id** estará ausente do recurso.</span><span class="sxs-lookup"><span data-stu-id="a0291-p103">In some circumstances, the unique identifier for the actor may not be available. In this case, the **displayName** property for the identity will be returned, but the **id** property will be missing from the resource.</span></span>

## <a name="relationships"></a><span data-ttu-id="a0291-123">Relações</span><span class="sxs-lookup"><span data-stu-id="a0291-123">Relationships</span></span>

<span data-ttu-id="a0291-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a0291-124">None.</span></span>

## <a name="see-also"></a><span data-ttu-id="a0291-125">Ver também</span><span class="sxs-lookup"><span data-stu-id="a0291-125">See also</span></span>

| <span data-ttu-id="a0291-126">Método</span><span class="sxs-lookup"><span data-stu-id="a0291-126">Method</span></span>           | <span data-ttu-id="a0291-127">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a0291-127">Return Type</span></span>    |<span data-ttu-id="a0291-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0291-128">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a0291-129">Obter revisores do accessReview</span><span class="sxs-lookup"><span data-stu-id="a0291-129">Get accessReview reviewers</span></span>](../api/accessreview-listreviewers.md) |       <span data-ttu-id="a0291-130">coleção [UserIdentity](useridentity.md)</span><span class="sxs-lookup"><span data-stu-id="a0291-130">[userIdentity](useridentity.md) collection</span></span>| <span data-ttu-id="a0291-131">Obter os revisores de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="a0291-131">Get the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="a0291-132">Adicionar revisor accessReview</span><span class="sxs-lookup"><span data-stu-id="a0291-132">Add accessReview reviewer</span></span>](../api/accessreview-addreviewer.md) |      <span data-ttu-id="a0291-133">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a0291-133">None.</span></span>   |   <span data-ttu-id="a0291-134">Adicionar um revisor a um accessReview.</span><span class="sxs-lookup"><span data-stu-id="a0291-134">Add a reviewer to an accessReview.</span></span> |
|[<span data-ttu-id="a0291-135">Remover revisor accessReview</span><span class="sxs-lookup"><span data-stu-id="a0291-135">Remove accessReview reviewer</span></span>](../api/accessreview-removereviewer.md) | <span data-ttu-id="a0291-136">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a0291-136">None.</span></span>  |   <span data-ttu-id="a0291-137">Remover um revisor de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="a0291-137">Remove a reviewer from an accessReview.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a0291-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a0291-138">JSON representation</span></span>

<span data-ttu-id="a0291-139">Veja a seguir uma representação JSON do tipo.</span><span class="sxs-lookup"><span data-stu-id="a0291-139">Here is a JSON representation of the type.</span></span>

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
