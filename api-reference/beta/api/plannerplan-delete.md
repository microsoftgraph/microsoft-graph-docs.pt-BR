---
title: Excluir plannerPlan
description: Exclua **plannerPlan**.
ms.openlocfilehash: 6395d51eaed38b26d07f9b1ba8b0d78e52394404
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039580"
---
# <a name="delete-plannerplan"></a><span data-ttu-id="d164f-103">Excluir plannerPlan</span><span class="sxs-lookup"><span data-stu-id="d164f-103">Delete plannerPlan</span></span>

> <span data-ttu-id="d164f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d164f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d164f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d164f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d164f-106">Exclua **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="d164f-106">Delete **plannerPlan**.</span></span>
## <a name="permissions"></a><span data-ttu-id="d164f-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="d164f-107">Permissions</span></span>
<span data-ttu-id="d164f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d164f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d164f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d164f-110">Permission type</span></span>      | <span data-ttu-id="d164f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d164f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d164f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d164f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d164f-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d164f-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d164f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d164f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d164f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d164f-115">Not supported.</span></span>    |
|<span data-ttu-id="d164f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d164f-116">Application</span></span> | <span data-ttu-id="d164f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d164f-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d164f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d164f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /planner/plans/<id>

```
## <a name="request-headers"></a><span data-ttu-id="d164f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d164f-119">Request headers</span></span>
| <span data-ttu-id="d164f-120">Nome</span><span class="sxs-lookup"><span data-stu-id="d164f-120">Name</span></span>       | <span data-ttu-id="d164f-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="d164f-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d164f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d164f-122">Authorization</span></span>  | <span data-ttu-id="d164f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d164f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d164f-125">If-Match</span><span class="sxs-lookup"><span data-stu-id="d164f-125">If-Match</span></span>  | <span data-ttu-id="d164f-p104">O último valor ETag conhecido do objeto **plannerPlan** a ser excluído. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d164f-p104">Last known ETag value for the **plannerPlan** to be deleted. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d164f-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d164f-128">Request body</span></span>
<span data-ttu-id="d164f-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d164f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d164f-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="d164f-130">Response</span></span>

<span data-ttu-id="d164f-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d164f-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="d164f-p106">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 400, 403, 404, 409 e 412. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="d164f-p106">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="d164f-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d164f-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d164f-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d164f-137">Request</span></span>
<span data-ttu-id="d164f-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d164f-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_plannerplan"
}-->
```http
DELETE https://graph.microsoft.com/beta/planner/plans/<id>
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="
```
##### <a name="response"></a><span data-ttu-id="d164f-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="d164f-139">Response</span></span>
<span data-ttu-id="d164f-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d164f-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete plannerPlan",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->