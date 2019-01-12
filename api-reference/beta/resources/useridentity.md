---
title: tipo de userIdentity
description: 'Para o Windows Azure AD avaliações de acesso, esse tipo representa uma identidade de usuário do Windows Azure AD por um revisor de uma revisão de acesso.  '
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 80e8cc68d4fc2f642be6c748b762fe47c7489d59
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932277"
---
# <a name="useridentity-type"></a><span data-ttu-id="9c126-103">tipo de userIdentity</span><span class="sxs-lookup"><span data-stu-id="9c126-103">userIdentity type</span></span>

> <span data-ttu-id="9c126-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9c126-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9c126-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9c126-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9c126-106">Para o Windows Azure AD [access analisa](accessreviews-root.md), esse tipo representa uma identidade de usuário do Windows Azure AD para um revisor de uma revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="9c126-106">For the Azure AD [access reviews](accessreviews-root.md), this type represents an Azure AD user identity for a reviewer of an access review.</span></span>  
<span data-ttu-id="9c126-107">No contexto de um log de auditoria do Azure AD, isso representa as informações de usuário que iniciou ou foi afetadas por uma atividade de auditoria.</span><span class="sxs-lookup"><span data-stu-id="9c126-107">In the context of an Azure AD audit log, this represents the user information that initiated or was affected by an audit activity.</span></span>

<span data-ttu-id="9c126-108">Esse tipo de herda de [identidade](identity.md) e tem uma propriedade adicional, o nome de usuário principal do usuário.</span><span class="sxs-lookup"><span data-stu-id="9c126-108">This type inherits from [identity](identity.md) and has one additional property, the user principal name of the user.</span></span>

## <a name="methods"></a><span data-ttu-id="9c126-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="9c126-109">Methods</span></span>

<span data-ttu-id="9c126-110">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9c126-110">None.</span></span>  <span data-ttu-id="9c126-111">Você incluiria objetos desse tipo no corpo de uma solicitação ao [criar um accessReview](../api/accessreview-create.md).</span><span class="sxs-lookup"><span data-stu-id="9c126-111">You would include objects of this type in the body of a request when [creating an accessReview](../api/accessreview-create.md).</span></span>

## <a name="properties"></a><span data-ttu-id="9c126-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9c126-112">Properties</span></span>
| <span data-ttu-id="9c126-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9c126-113">Property</span></span>     | <span data-ttu-id="9c126-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="9c126-114">Type</span></span>   |<span data-ttu-id="9c126-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c126-115">Description</span></span>|
|:---------------|:--------|:----------|
| `displayName` | `String` | <span data-ttu-id="9c126-116">Nome para exibição da identidade.</span><span class="sxs-lookup"><span data-stu-id="9c126-116">The identity's display name.</span></span> <span data-ttu-id="9c126-117">Observe que isso nem sempre pode ser disponível ou atualizadas.</span><span class="sxs-lookup"><span data-stu-id="9c126-117">Note that this may not always be available or up-to-date.</span></span>    |
| `id`          | `String` | <span data-ttu-id="9c126-118">Identificador exclusivo da identidade.</span><span class="sxs-lookup"><span data-stu-id="9c126-118">Unique identifier for the identity.</span></span>  |
| `ipAddress`| `String`| <span data-ttu-id="9c126-119">Indica o endereço IP do cliente usado pelo usuário que está executando a atividade (somente no log de auditoria).</span><span class="sxs-lookup"><span data-stu-id="9c126-119">Indicates the client IP address used by user performing the activity (audit log only).</span></span>|
| `userPrincipalName`|`String` | <span data-ttu-id="9c126-120">O atributo userPrincipalName do usuário.</span><span class="sxs-lookup"><span data-stu-id="9c126-120">The userPrincipalName attribute of the user.</span></span> |

## <a name="remarks"></a><span data-ttu-id="9c126-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="9c126-121">Remarks</span></span>

<span data-ttu-id="9c126-p104">Em algumas circunstâncias, o identificador exclusivo para o ator pode não estar disponível. Nesse caso, a propriedade **displayName** para a identidade será retornada, mas a propriedade **id** estará ausente do recurso.</span><span class="sxs-lookup"><span data-stu-id="9c126-p104">In some circumstances, the unique identifier for the actor may not be available. In this case, the **displayName** property for the identity will be returned, but the **id** property will be missing from the resource.</span></span>

## <a name="relationships"></a><span data-ttu-id="9c126-124">Relações</span><span class="sxs-lookup"><span data-stu-id="9c126-124">Relationships</span></span>

<span data-ttu-id="9c126-125">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9c126-125">None.</span></span>

## <a name="see-also"></a><span data-ttu-id="9c126-126">Ver também</span><span class="sxs-lookup"><span data-stu-id="9c126-126">See also</span></span>

| <span data-ttu-id="9c126-127">Método</span><span class="sxs-lookup"><span data-stu-id="9c126-127">Method</span></span>           | <span data-ttu-id="9c126-128">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9c126-128">Return Type</span></span>    |<span data-ttu-id="9c126-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c126-129">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9c126-130">Obter accessReview reviewers</span><span class="sxs-lookup"><span data-stu-id="9c126-130">Get accessReview reviewers</span></span>](../api/accessreview-listreviewers.md) |       <span data-ttu-id="9c126-131">coleção [userIdentity](useridentity.md)</span><span class="sxs-lookup"><span data-stu-id="9c126-131">[userIdentity](useridentity.md) collection</span></span>| <span data-ttu-id="9c126-132">Obtenha os revisores de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="9c126-132">Get the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="9c126-133">Adicionar Revisor accessReview</span><span class="sxs-lookup"><span data-stu-id="9c126-133">Add accessReview reviewer</span></span>](../api/accessreview-addreviewer.md) |      <span data-ttu-id="9c126-134">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9c126-134">None.</span></span>   |   <span data-ttu-id="9c126-135">Adicione um revisor a um accessReview.</span><span class="sxs-lookup"><span data-stu-id="9c126-135">Add a reviewer to an accessReview.</span></span> |
|[<span data-ttu-id="9c126-136">Remover accessReview revisor</span><span class="sxs-lookup"><span data-stu-id="9c126-136">Remove accessReview reviewer</span></span>](../api/accessreview-removereviewer.md) | <span data-ttu-id="9c126-137">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9c126-137">None.</span></span>  |   <span data-ttu-id="9c126-138">Remova um revisor de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="9c126-138">Remove a reviewer from an accessReview.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9c126-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9c126-139">JSON representation</span></span>

<span data-ttu-id="9c126-140">Aqui está uma representação JSON do tipo.</span><span class="sxs-lookup"><span data-stu-id="9c126-140">Here is a JSON representation of the type.</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "userIdentity type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
