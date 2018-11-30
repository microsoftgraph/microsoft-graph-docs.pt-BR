---
title: Excluir inferenceClassificationOverride
description: Exclua uma substituição especificada de acordo com sua ID.
ms.openlocfilehash: ef4ff995e0e7f4392d9ca13835976076b3fdbe59
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004534"
---
# <a name="delete-inferenceclassificationoverride"></a><span data-ttu-id="cebcb-103">Excluir inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="cebcb-103">Delete inferenceClassificationOverride</span></span>

<span data-ttu-id="cebcb-104">Exclua uma substituição especificada de acordo com sua ID.</span><span class="sxs-lookup"><span data-stu-id="cebcb-104">Delete an override specified by its ID.</span></span>
## <a name="permissions"></a><span data-ttu-id="cebcb-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="cebcb-105">Permissions</span></span>
<span data-ttu-id="cebcb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cebcb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cebcb-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cebcb-108">Permission type</span></span>      | <span data-ttu-id="cebcb-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cebcb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cebcb-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cebcb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cebcb-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cebcb-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="cebcb-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cebcb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cebcb-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cebcb-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="cebcb-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cebcb-114">Application</span></span> | <span data-ttu-id="cebcb-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cebcb-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="cebcb-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cebcb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/inferenceClassification/overrides/{id}
DELETE /users/{id}/inferenceClassification/overrides/{id}
```
## <a name="request-headers"></a><span data-ttu-id="cebcb-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cebcb-117">Request headers</span></span>
| <span data-ttu-id="cebcb-118">Nome</span><span class="sxs-lookup"><span data-stu-id="cebcb-118">Name</span></span>       | <span data-ttu-id="cebcb-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="cebcb-119">Type</span></span> | <span data-ttu-id="cebcb-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="cebcb-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="cebcb-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="cebcb-121">Authorization</span></span>  | <span data-ttu-id="cebcb-122">string</span><span class="sxs-lookup"><span data-stu-id="cebcb-122">string</span></span>  | <span data-ttu-id="cebcb-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cebcb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cebcb-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cebcb-125">Request body</span></span>
<span data-ttu-id="cebcb-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cebcb-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cebcb-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="cebcb-127">Response</span></span>

<span data-ttu-id="cebcb-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cebcb-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cebcb-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cebcb-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cebcb-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cebcb-131">Request</span></span>
<span data-ttu-id="cebcb-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cebcb-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["98f5bdef-576a-404d-a2ea-07a3cf34af4r"],
  "name": "delete_inferenceclassificationoverride"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/inferenceClassification/overrides/98f5bdef-576a-404d-a2ea-07a3cf34af4r
```
##### <a name="response"></a><span data-ttu-id="cebcb-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="cebcb-133">Response</span></span>
<span data-ttu-id="cebcb-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cebcb-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Delete inferenceClassificationOverride",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->