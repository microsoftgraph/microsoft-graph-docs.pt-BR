---
title: Aplicar accessReview
description: 'No Windows Azure AD para acessar o recurso de revisões, aplique as decisões de um accessReview concluída.  O objeto de destino pode ser uma revisão de acesso de uma única vez, ou uma instância de uma análise mais acesso recorrente.  '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9612f3bcb8a032ee32cd7b058d3f21950c9b120f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512210"
---
# <a name="apply-accessreview"></a><span data-ttu-id="1920b-104">Aplicar accessReview</span><span class="sxs-lookup"><span data-stu-id="1920b-104">Apply accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1920b-105">O recurso [acesso analisa](../resources/accessreviews-root.md) Azure AD, aplica as decisões de um concluídas [accessReview](../resources/accessreview.md).</span><span class="sxs-lookup"><span data-stu-id="1920b-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, apply the decisions of a completed [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="1920b-106">O objeto de destino pode ser uma revisão de acesso de uma única vez, ou uma instância de uma análise mais acesso recorrente.</span><span class="sxs-lookup"><span data-stu-id="1920b-106">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span>  


<span data-ttu-id="1920b-107">Depois que uma revisão do access for concluída, um porque atingiu a data de término ou um administrador parou de manualmente e aplicar auto não foi configurado para a revisão, é possível chamar Apply para aplicar as alterações.</span><span class="sxs-lookup"><span data-stu-id="1920b-107">After an access review is finished, either because it reached the end date or an administrator stopped it manually, and auto-apply wasn't configured for the review, you can call Apply to apply the changes.</span></span> <span data-ttu-id="1920b-108">Até aplicar ocorre, as decisões para remover os direitos de acesso não aparecem no recurso de código-fonte, os usuários por exemplo mantêm suas associações de grupo.</span><span class="sxs-lookup"><span data-stu-id="1920b-108">Until apply occurs, the decisions to remove access rights do not appear on the source resource, the users for instance retain their group memberships.</span></span> <span data-ttu-id="1920b-109">Chamando aplicar, o resultado da revisão é implementado, atualizando o grupo ou o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1920b-109">By calling apply, the outcome of the review is implemented by updating the group or application.</span></span> <span data-ttu-id="1920b-110">Se o acesso do usuário foi negado na revisão, quando um administrador chama este API, o Azure AD remove a atribuição de seus aplicativos ou da associação.</span><span class="sxs-lookup"><span data-stu-id="1920b-110">If a user's access was denied in the review, when an administrator calls this API, Azure AD removes their membership or application assignment.</span></span> 

<span data-ttu-id="1920b-111">Depois que uma revisão do access for concluída e aplicação de automática foi configurado, em seguida, o status da revisão deixará de ser concluído em estados intermediários e finalmente será alterado para o estado aplicado.</span><span class="sxs-lookup"><span data-stu-id="1920b-111">After an access review is finished, and auto-apply was configured, then the status of the review will change from Completed through intermediate states and finally will change to state Applied.</span></span> <span data-ttu-id="1920b-112">Você deve esperar consulte negados users, se houver, que está sendo removido do recurso Agrupar atribuição de aplicativo ou associação em poucos minutos.</span><span class="sxs-lookup"><span data-stu-id="1920b-112">You should expect to see denied users, if any, being removed from the resource group membership or app assignment in a few minutes.</span></span>

<span data-ttu-id="1920b-113">Um automático configurado a aplicação de revisão ou selecionando aplicar não tem efeito em um grupo que se origina de um diretório local ou um grupo dinâmico.</span><span class="sxs-lookup"><span data-stu-id="1920b-113">A configured auto applying review, or selecting Apply doesn't have an effect on a group that originates in an on-premises directory or a dynamic group.</span></span> <span data-ttu-id="1920b-114">Se você quiser alterar um grupo local de originado, baixe os resultados e aplicar essas alterações para a representação do grupo nesse diretório.</span><span class="sxs-lookup"><span data-stu-id="1920b-114">If you want to change a group that originates on-premises, download the results and apply those changes to the representation of the group in that directory.</span></span>


## <a name="permissions"></a><span data-ttu-id="1920b-115">Permissões</span><span class="sxs-lookup"><span data-stu-id="1920b-115">Permissions</span></span>
<span data-ttu-id="1920b-p106">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1920b-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1920b-118">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1920b-118">Permission type</span></span>                        | <span data-ttu-id="1920b-119">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1920b-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="1920b-120">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1920b-120">Delegated (work or school account)</span></span>     | <span data-ttu-id="1920b-121">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1920b-121">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="1920b-122">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1920b-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1920b-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1920b-123">Not supported.</span></span> |
|<span data-ttu-id="1920b-124">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1920b-124">Application</span></span>                            | <span data-ttu-id="1920b-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1920b-125">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1920b-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1920b-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/applyDecisions()
```
## <a name="request-headers"></a><span data-ttu-id="1920b-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1920b-127">Request headers</span></span>
| <span data-ttu-id="1920b-128">Nome</span><span class="sxs-lookup"><span data-stu-id="1920b-128">Name</span></span>         | <span data-ttu-id="1920b-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="1920b-129">Type</span></span>        | <span data-ttu-id="1920b-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="1920b-130">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="1920b-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="1920b-131">Authorization</span></span> | <span data-ttu-id="1920b-132">string</span><span class="sxs-lookup"><span data-stu-id="1920b-132">string</span></span> | <span data-ttu-id="1920b-133">Token de portador</span><span class="sxs-lookup"><span data-stu-id="1920b-133">Bearer \{token\}.</span></span> <span data-ttu-id="1920b-134">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1920b-134">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1920b-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1920b-135">Request body</span></span>
<span data-ttu-id="1920b-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1920b-136">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="1920b-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="1920b-137">Response</span></span>
<span data-ttu-id="1920b-p108">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1920b-p108">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="see-also"></a><span data-ttu-id="1920b-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="1920b-140">See also</span></span>

- [<span data-ttu-id="1920b-141">Como concluir uma revisão do access</span><span class="sxs-lookup"><span data-stu-id="1920b-141">How to complete an access review</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-azure-ad-controls-complete-access-review)

## <a name="example"></a><span data-ttu-id="1920b-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1920b-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1920b-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1920b-143">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "apply_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews('2975E9B5-44CE-4E71-93D3-30F03B5AA992')/applyDecisions()
```
##### <a name="response"></a><span data-ttu-id="1920b-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="1920b-144">Response</span></span>
><span data-ttu-id="1920b-p109">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1920b-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Apply accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-apply.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
