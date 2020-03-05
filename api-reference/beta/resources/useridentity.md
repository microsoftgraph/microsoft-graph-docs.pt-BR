---
title: tipo UserIdentity
description: 'Para as revisões do Azure AD Access, este tipo representa uma identidade de usuário do Azure AD para um revisor de uma revisão do Access.  '
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 466b39a52f2bc2b9e20f313f3f80926855f492f9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519523"
---
# <a name="useridentity-type"></a><span data-ttu-id="ac624-103">tipo UserIdentity</span><span class="sxs-lookup"><span data-stu-id="ac624-103">userIdentity type</span></span>

<span data-ttu-id="ac624-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ac624-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac624-105">Para as revisões do Azure AD [Access](accessreviews-root.md), este tipo representa uma identidade de usuário do Azure ad para um criador ou revisor de uma revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="ac624-105">For the Azure AD [access reviews](accessreviews-root.md), this type represents an Azure AD user identity for a creator or reviewer of an access review.</span></span>  
<span data-ttu-id="ac624-106">No contexto de um log de auditoria do Azure AD, isso representa as informações do usuário que foram iniciadas ou foram afetadas por uma atividade de auditoria.</span><span class="sxs-lookup"><span data-stu-id="ac624-106">In the context of an Azure AD audit log, this represents the user information that initiated or was affected by an audit activity.</span></span>

<span data-ttu-id="ac624-107">Esse tipo herda de [Identity](identity.md) e tem uma propriedade adicional, o nome principal do usuário do usuário.</span><span class="sxs-lookup"><span data-stu-id="ac624-107">This type inherits from [identity](identity.md) and has one additional property, the user principal name of the user.</span></span>

## <a name="methods"></a><span data-ttu-id="ac624-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="ac624-108">Methods</span></span>

<span data-ttu-id="ac624-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ac624-109">None.</span></span>  <span data-ttu-id="ac624-110">Você deve incluir objetos desse tipo no corpo de uma solicitação ao [criar um accessReview](../api/accessreview-create.md).</span><span class="sxs-lookup"><span data-stu-id="ac624-110">You would include objects of this type in the body of a request when [creating an accessReview](../api/accessreview-create.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ac624-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ac624-111">Properties</span></span>
| <span data-ttu-id="ac624-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ac624-112">Property</span></span>     | <span data-ttu-id="ac624-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="ac624-113">Type</span></span>   |<span data-ttu-id="ac624-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac624-114">Description</span></span>|
|:---------------|:--------|:----------|
| `displayName` | `String` | <span data-ttu-id="ac624-115">Nome de exibição da identidade.</span><span class="sxs-lookup"><span data-stu-id="ac624-115">The identity's display name.</span></span> <span data-ttu-id="ac624-116">Observe que isso pode não estar sempre disponível ou atualizado.</span><span class="sxs-lookup"><span data-stu-id="ac624-116">Note that this may not always be available or up-to-date.</span></span>    |
| `id`          | `String` | <span data-ttu-id="ac624-117">Identificador exclusivo da identidade.</span><span class="sxs-lookup"><span data-stu-id="ac624-117">Unique identifier for the identity.</span></span>  |
| `ipAddress`| `String`| <span data-ttu-id="ac624-118">Indica o endereço IP do cliente usado pelo usuário que está executando a atividade (log de auditoria somente).</span><span class="sxs-lookup"><span data-stu-id="ac624-118">Indicates the client IP address used by user performing the activity (audit log only).</span></span>|
| `userPrincipalName`|`String` | <span data-ttu-id="ac624-119">O atributo userPrincipalName do usuário.</span><span class="sxs-lookup"><span data-stu-id="ac624-119">The userPrincipalName attribute of the user.</span></span> |

## <a name="remarks"></a><span data-ttu-id="ac624-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="ac624-120">Remarks</span></span>

<span data-ttu-id="ac624-p103">Em algumas circunstâncias, o identificador exclusivo para o ator pode não estar disponível. Nesse caso, a propriedade **displayName** para a identidade será retornada, mas a propriedade **id** estará ausente do recurso.</span><span class="sxs-lookup"><span data-stu-id="ac624-p103">In some circumstances, the unique identifier for the actor may not be available. In this case, the **displayName** property for the identity will be returned, but the **id** property will be missing from the resource.</span></span>

## <a name="relationships"></a><span data-ttu-id="ac624-123">Relações</span><span class="sxs-lookup"><span data-stu-id="ac624-123">Relationships</span></span>

<span data-ttu-id="ac624-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ac624-124">None.</span></span>

## <a name="see-also"></a><span data-ttu-id="ac624-125">Ver também</span><span class="sxs-lookup"><span data-stu-id="ac624-125">See also</span></span>

| <span data-ttu-id="ac624-126">Método</span><span class="sxs-lookup"><span data-stu-id="ac624-126">Method</span></span>           | <span data-ttu-id="ac624-127">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ac624-127">Return Type</span></span>    |<span data-ttu-id="ac624-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac624-128">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ac624-129">Obter revisores do accessReview</span><span class="sxs-lookup"><span data-stu-id="ac624-129">Get accessReview reviewers</span></span>](../api/accessreview-listreviewers.md) |       <span data-ttu-id="ac624-130">coleção [UserIdentity](useridentity.md)</span><span class="sxs-lookup"><span data-stu-id="ac624-130">[userIdentity](useridentity.md) collection</span></span>| <span data-ttu-id="ac624-131">Obter os revisores de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="ac624-131">Get the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="ac624-132">Adicionar revisor accessReview</span><span class="sxs-lookup"><span data-stu-id="ac624-132">Add accessReview reviewer</span></span>](../api/accessreview-addreviewer.md) |      <span data-ttu-id="ac624-133">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ac624-133">None.</span></span>   |   <span data-ttu-id="ac624-134">Adicionar um revisor a um accessReview.</span><span class="sxs-lookup"><span data-stu-id="ac624-134">Add a reviewer to an accessReview.</span></span> |
|[<span data-ttu-id="ac624-135">Remover revisor accessReview</span><span class="sxs-lookup"><span data-stu-id="ac624-135">Remove accessReview reviewer</span></span>](../api/accessreview-removereviewer.md) | <span data-ttu-id="ac624-136">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ac624-136">None.</span></span>  |   <span data-ttu-id="ac624-137">Remover um revisor de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="ac624-137">Remove a reviewer from an accessReview.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ac624-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ac624-138">JSON representation</span></span>

<span data-ttu-id="ac624-139">Veja a seguir uma representação JSON do tipo.</span><span class="sxs-lookup"><span data-stu-id="ac624-139">Here is a JSON representation of the type.</span></span>

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
