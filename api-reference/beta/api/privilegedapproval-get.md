---
title: Get privilegedApproval
description: Recupere as propriedades e os relacionamentos do objeto privilegedapproval.
localization_priority: Normal
ms.openlocfilehash: d66424622f30ecd91788e9135585921a6af44330
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33594935"
---
# <a name="get-privilegedapproval"></a><span data-ttu-id="274a5-103">Get privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="274a5-103">Get privilegedApproval</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="274a5-104">Recupere as propriedades e os relacionamentos do objeto privilegedapproval.</span><span class="sxs-lookup"><span data-stu-id="274a5-104">Retrieve the properties and relationships of privilegedapproval object.</span></span>
## <a name="permissions"></a><span data-ttu-id="274a5-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="274a5-105">Permissions</span></span>
<span data-ttu-id="274a5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="274a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="274a5-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="274a5-108">Permission type</span></span>      | <span data-ttu-id="274a5-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="274a5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="274a5-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="274a5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="274a5-111">PrivilegedAccess. ReadWrite. AzureAD, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="274a5-111">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="274a5-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="274a5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="274a5-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="274a5-113">Not supported.</span></span>    |
|<span data-ttu-id="274a5-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="274a5-114">Application</span></span> | <span data-ttu-id="274a5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="274a5-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="274a5-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="274a5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedApproval/<id>
```
## <a name="optional-query-parameters"></a><span data-ttu-id="274a5-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="274a5-117">Optional query parameters</span></span>
<span data-ttu-id="274a5-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="274a5-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="274a5-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="274a5-119">Request headers</span></span>
| <span data-ttu-id="274a5-120">Nome</span><span class="sxs-lookup"><span data-stu-id="274a5-120">Name</span></span>      |<span data-ttu-id="274a5-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="274a5-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="274a5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="274a5-122">Authorization</span></span>  | <span data-ttu-id="274a5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="274a5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="274a5-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="274a5-125">Request body</span></span>
<span data-ttu-id="274a5-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="274a5-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="274a5-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="274a5-127">Response</span></span>

<span data-ttu-id="274a5-128">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [privilegedApproval](../resources/privilegedapproval.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="274a5-128">If successful, this method returns a `200 OK` response code and [privilegedApproval](../resources/privilegedapproval.md) object in the response body.</span></span>

<span data-ttu-id="274a5-129">Observe que o locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="274a5-129">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="274a5-130">Caso contrário, o código de status HTTP 403 proibido será retornado.</span><span class="sxs-lookup"><span data-stu-id="274a5-130">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="274a5-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="274a5-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="274a5-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="274a5-132">Request</span></span>
<span data-ttu-id="274a5-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="274a5-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedapproval"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedApproval/<id>
```
##### <a name="response"></a><span data-ttu-id="274a5-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="274a5-134">Response</span></span>
<span data-ttu-id="274a5-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="274a5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedApproval"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 193

{
  "id": "id-value",
  "userId": "userId-value",
  "roleId": "roleId-value",
  "approvalType": "approvalType-value",
  "approvalState": "approvalState-value",
  "approvalDuration": "datetime-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="274a5-138">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="274a5-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="274a5-139">Basic</span><span class="sxs-lookup"><span data-stu-id="274a5-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_privilegedapproval-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="274a5-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="274a5-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_privilegedapproval-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get privilegedApproval",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedapproval-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/privilegedapproval-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
