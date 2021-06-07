---
title: Tipo userIdentity
description: Representa uma identidade de usuário do Azure AD para um revistor de uma revisão de acesso.
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 94c0af9a5909966471594ab4c23003282f416849
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52750361"
---
# <a name="useridentity-type"></a><span data-ttu-id="cb978-103">Tipo userIdentity</span><span class="sxs-lookup"><span data-stu-id="cb978-103">userIdentity type</span></span>

<span data-ttu-id="cb978-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb978-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb978-105">Para as análises de acesso do Azure AD, esse tipo representa uma identidade de usuário do Azure AD para um criador ou [revistor](accessreviews-root.md)de uma revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="cb978-105">For the Azure AD [access reviews](accessreviews-root.md), this type represents an Azure AD user identity for a creator or reviewer of an access review.</span></span>
<span data-ttu-id="cb978-106">No contexto de um log de auditoria do Azure AD, isso representa as informações do usuário que iniciaram ou foram afetadas por uma atividade de auditoria.</span><span class="sxs-lookup"><span data-stu-id="cb978-106">In the context of an Azure AD audit log, this represents the user information that initiated or was affected by an audit activity.</span></span>

<span data-ttu-id="cb978-107">Esse tipo herda da [identidade](identity.md) e tem uma propriedade adicional, o nome principal do usuário.</span><span class="sxs-lookup"><span data-stu-id="cb978-107">This type inherits from [identity](identity.md) and has one additional property, the user principal name of the user.</span></span>

## <a name="methods"></a><span data-ttu-id="cb978-108">Methods</span><span class="sxs-lookup"><span data-stu-id="cb978-108">Methods</span></span>

<span data-ttu-id="cb978-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="cb978-109">None.</span></span>  <span data-ttu-id="cb978-110">Você incluiria objetos desse tipo no corpo de uma solicitação ao [criar um accessReview](../api/accessreview-create.md).</span><span class="sxs-lookup"><span data-stu-id="cb978-110">You would include objects of this type in the body of a request when [creating an accessReview](../api/accessreview-create.md).</span></span>

## <a name="properties"></a><span data-ttu-id="cb978-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cb978-111">Properties</span></span>

| <span data-ttu-id="cb978-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cb978-112">Property</span></span>          | <span data-ttu-id="cb978-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="cb978-113">Type</span></span>   | <span data-ttu-id="cb978-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb978-114">Description</span></span>                                                                            |
|:------------------|:-------|:---------------------------------------------------------------------------------------|
| <span data-ttu-id="cb978-115">displayName</span><span class="sxs-lookup"><span data-stu-id="cb978-115">displayName</span></span>       | <span data-ttu-id="cb978-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cb978-116">String</span></span> | <span data-ttu-id="cb978-117">Nome de exibição da identidade.</span><span class="sxs-lookup"><span data-stu-id="cb978-117">The identity's display name.</span></span> <span data-ttu-id="cb978-118">Observe que isso pode nem sempre estar disponível ou atualizado.</span><span class="sxs-lookup"><span data-stu-id="cb978-118">Note that this may not always be available or up-to-date.</span></span> |
| <span data-ttu-id="cb978-119">id</span><span class="sxs-lookup"><span data-stu-id="cb978-119">id</span></span>                | <span data-ttu-id="cb978-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cb978-120">String</span></span> | <span data-ttu-id="cb978-121">Identificador exclusivo da identidade.</span><span class="sxs-lookup"><span data-stu-id="cb978-121">Unique identifier for the identity.</span></span> <span data-ttu-id="cb978-122">Anulável.</span><span class="sxs-lookup"><span data-stu-id="cb978-122">Nullable.</span></span>                                                   |
| <span data-ttu-id="cb978-123">ipAddress</span><span class="sxs-lookup"><span data-stu-id="cb978-123">ipAddress</span></span>         | <span data-ttu-id="cb978-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cb978-124">String</span></span> | <span data-ttu-id="cb978-125">Indica o endereço IP do cliente usado pelo usuário executando a atividade (somente log de auditoria).</span><span class="sxs-lookup"><span data-stu-id="cb978-125">Indicates the client IP address used by user performing the activity (audit log only).</span></span> |
| <span data-ttu-id="cb978-126">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="cb978-126">userPrincipalName</span></span> | <span data-ttu-id="cb978-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cb978-127">String</span></span> | <span data-ttu-id="cb978-128">O atributo userPrincipalName do usuário.</span><span class="sxs-lookup"><span data-stu-id="cb978-128">The userPrincipalName attribute of the user.</span></span>                                           |

### <a name="remarks"></a><span data-ttu-id="cb978-129">Comentários</span><span class="sxs-lookup"><span data-stu-id="cb978-129">Remarks</span></span>

<span data-ttu-id="cb978-p105">Em algumas circunstâncias, o identificador exclusivo para o ator pode não estar disponível. Nesse caso, a propriedade **displayName** para a identidade será retornada, mas a propriedade **id** estará ausente do recurso.</span><span class="sxs-lookup"><span data-stu-id="cb978-p105">In some circumstances, the unique identifier for the actor may not be available. In this case, the **displayName** property for the identity will be returned, but the **id** property will be missing from the resource.</span></span>

## <a name="relationships"></a><span data-ttu-id="cb978-132">Relações</span><span class="sxs-lookup"><span data-stu-id="cb978-132">Relationships</span></span>

<span data-ttu-id="cb978-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cb978-133">None.</span></span>

## <a name="see-also"></a><span data-ttu-id="cb978-134">Ver também</span><span class="sxs-lookup"><span data-stu-id="cb978-134">See also</span></span>

| <span data-ttu-id="cb978-135">Método</span><span class="sxs-lookup"><span data-stu-id="cb978-135">Method</span></span>                                                                | <span data-ttu-id="cb978-136">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="cb978-136">Return Type</span></span>                                | <span data-ttu-id="cb978-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb978-137">Description</span></span>                             |
|:----------------------------------------------------------------------|:-------------------------------------------|:----------------------------------------|
| [<span data-ttu-id="cb978-138">Obter revisores do accessReview</span><span class="sxs-lookup"><span data-stu-id="cb978-138">Get accessReview reviewers</span></span>](../api/accessreview-listreviewers.md)    | <span data-ttu-id="cb978-139">[Coleção userIdentity](useridentity.md)</span><span class="sxs-lookup"><span data-stu-id="cb978-139">[userIdentity](useridentity.md) collection</span></span> | <span data-ttu-id="cb978-140">Obter os revisores de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="cb978-140">Get the reviewers of an accessReview.</span></span>   |
| [<span data-ttu-id="cb978-141">Adicionar o revisor accessReview</span><span class="sxs-lookup"><span data-stu-id="cb978-141">Add accessReview reviewer</span></span>](../api/accessreview-addreviewer.md)       | <span data-ttu-id="cb978-142">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="cb978-142">None.</span></span>                                      | <span data-ttu-id="cb978-143">Adicione um revisor a um accessReview.</span><span class="sxs-lookup"><span data-stu-id="cb978-143">Add a reviewer to an accessReview.</span></span>      |
| [<span data-ttu-id="cb978-144">Remover o revisor accessReview</span><span class="sxs-lookup"><span data-stu-id="cb978-144">Remove accessReview reviewer</span></span>](../api/accessreview-removereviewer.md) | <span data-ttu-id="cb978-145">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="cb978-145">None.</span></span>                                      | <span data-ttu-id="cb978-146">Remova um revisor de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="cb978-146">Remove a reviewer from an accessReview.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="cb978-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cb978-147">JSON representation</span></span>

<span data-ttu-id="cb978-148">Aqui está uma representação JSON do tipo.</span><span class="sxs-lookup"><span data-stu-id="cb978-148">Here is a JSON representation of the type.</span></span>

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


