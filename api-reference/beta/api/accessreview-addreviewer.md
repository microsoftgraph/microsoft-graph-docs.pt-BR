---
title: Adicionar Revisor accessReview
description: 'No recurso de avaliações de acesso do Azure AD, atualize um objeto accessReview existente para adicionar outro usuário como um revisor.  Essa operação só é permitida para uma revisão de acesso que ainda não foi concluída e apenas para uma revisão de acesso onde os revisores são explicitamente especificados. Essa operação não é permitida para uma revisão do access no qual os usuários revisam sua próprias acesso e não foi projetada para uma revisão de acesso na qual os proprietários do grupo são atribuídos como os revisores. '
ms.openlocfilehash: ac7722d1bea30659db6f6defe26c0a08ecd67caf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035643"
---
# <a name="add-accessreview-reviewer"></a><span data-ttu-id="3c69f-105">Adicionar Revisor accessReview</span><span class="sxs-lookup"><span data-stu-id="3c69f-105">Add accessReview reviewer</span></span>

> <span data-ttu-id="3c69f-106">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3c69f-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3c69f-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3c69f-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3c69f-108">No recurso [acesso analisa](../resources/accessreviews-root.md) Azure AD, atualize um objeto [accessReview](../resources/accessreview.md) existente para adicionar outro usuário como um revisor.</span><span class="sxs-lookup"><span data-stu-id="3c69f-108">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to add another user as a reviewer.</span></span>  <span data-ttu-id="3c69f-109">Essa operação só é permitida para uma revisão de acesso que ainda não foi concluída e apenas para uma revisão de acesso onde os revisores são explicitamente especificados.</span><span class="sxs-lookup"><span data-stu-id="3c69f-109">This operation is only permitted for an access review that is not yet completed, and only for an access review where the reviewers are explicitly specified.</span></span> <span data-ttu-id="3c69f-110">Essa operação não é permitida para uma revisão do access no qual os usuários revisam sua próprias acesso e não foi projetada para uma revisão de acesso na qual os proprietários do grupo são atribuídos como os revisores.</span><span class="sxs-lookup"><span data-stu-id="3c69f-110">This operation is not permitted for an access review in which users review their own access, and not intended for an access review in which the group owners are assigned as the reviewers.</span></span> 


## <a name="permissions"></a><span data-ttu-id="3c69f-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="3c69f-111">Permissions</span></span>
<span data-ttu-id="3c69f-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c69f-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c69f-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3c69f-114">Permission type</span></span>                        | <span data-ttu-id="3c69f-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3c69f-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="3c69f-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3c69f-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="3c69f-117">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c69f-117">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="3c69f-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3c69f-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c69f-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3c69f-119">Not supported.</span></span> |
|<span data-ttu-id="3c69f-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3c69f-120">Application</span></span>                            | <span data-ttu-id="3c69f-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3c69f-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3c69f-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3c69f-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('{reviewId}')/reviewers
```
## <a name="request-headers"></a><span data-ttu-id="3c69f-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3c69f-123">Request headers</span></span>
| <span data-ttu-id="3c69f-124">Nome</span><span class="sxs-lookup"><span data-stu-id="3c69f-124">Name</span></span>         | <span data-ttu-id="3c69f-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="3c69f-125">Type</span></span>        | <span data-ttu-id="3c69f-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c69f-126">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="3c69f-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="3c69f-127">Authorization</span></span> | <span data-ttu-id="3c69f-128">string</span><span class="sxs-lookup"><span data-stu-id="3c69f-128">string</span></span> | <span data-ttu-id="3c69f-129">Portador \{token\}.</span><span class="sxs-lookup"><span data-stu-id="3c69f-129">Bearer \{token\}.</span></span> <span data-ttu-id="3c69f-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3c69f-130">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3c69f-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3c69f-131">Request body</span></span>
<span data-ttu-id="3c69f-132">No corpo da solicitação, fornece uma representação JSON da ID de um usuário que será um revisor.</span><span class="sxs-lookup"><span data-stu-id="3c69f-132">In the request body, supply a JSON representation of the ID of a user who will be a reviewer.</span></span>

<span data-ttu-id="3c69f-133">A tabela a seguir mostra as propriedades que podem ser fornecidas quando você atualiza um accessReview.</span><span class="sxs-lookup"><span data-stu-id="3c69f-133">The following table shows the properties that can be supplied when you update an accessReview.</span></span>

| <span data-ttu-id="3c69f-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3c69f-134">Property</span></span>     | <span data-ttu-id="3c69f-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="3c69f-135">Type</span></span>        | <span data-ttu-id="3c69f-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c69f-136">Description</span></span> |
|:-------------|:------------|:------------|
| `id`             |`String`                                                        | <span data-ttu-id="3c69f-137">ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="3c69f-137">The user ID.</span></span>  |


## <a name="response"></a><span data-ttu-id="3c69f-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c69f-138">Response</span></span>
<span data-ttu-id="3c69f-139">Se tiver êxito, este método retornará um `201, Created` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="3c69f-139">If successful, this method returns a `201, Created` response code .</span></span>

## <a name="example"></a><span data-ttu-id="3c69f-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3c69f-140">Example</span></span>

<span data-ttu-id="3c69f-141">Este é um exemplo de como atualizar uma revisão de acesso (não recorrentes) ocasional com um revisor adicional.</span><span class="sxs-lookup"><span data-stu-id="3c69f-141">This is an example of updating a one-time (not reoccurring) access review with an additional reviewer.</span></span>

##### <a name="request"></a><span data-ttu-id="3c69f-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3c69f-142">Request</span></span>
<span data-ttu-id="3c69f-143">No corpo da solicitação, fornece uma representação JSON da id do objeto de usuário.</span><span class="sxs-lookup"><span data-stu-id="3c69f-143">In the request body, supply a JSON representation of the id of the user object.</span></span>

<!-- {
  "blockType": "request",
  "name": "add_accessReview_reviewer"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/reviewers
Content-type: application/json

{
    "id":"006111db-0810-4494-a6df-904d368bd81b"
}
```

##### <a name="response"></a><span data-ttu-id="3c69f-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c69f-144">Response</span></span>
><span data-ttu-id="3c69f-p106">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3c69f-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 201 Created

```

<!-- {
  "type": "#page.annotation",
  "description": "Add accessReview reviewer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
