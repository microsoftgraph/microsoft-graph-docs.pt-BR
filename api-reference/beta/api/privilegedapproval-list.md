---
title: List privilegedApproval
description: Recupere uma lista de objetos privilegedapproval.
localization_priority: Normal
ms.openlocfilehash: 2e3adb6a85906c234ff64cf18b193a1156e35d14
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33596426"
---
# <a name="list-privilegedapproval"></a><span data-ttu-id="87320-103">List privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="87320-103">List privilegedApproval</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="87320-104">Recupere uma lista de objetos privilegedapproval.</span><span class="sxs-lookup"><span data-stu-id="87320-104">Retrieve a list of privilegedapproval objects.</span></span>

<span data-ttu-id="87320-105">Para filtrar os resultados da consulta, use as expressões ``$filter`` padrão do OData nos URIs.</span><span class="sxs-lookup"><span data-stu-id="87320-105">To filter the results from the query, use the standard OData ``$filter`` expressions in the URIs.</span></span>
## <a name="permissions"></a><span data-ttu-id="87320-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="87320-106">Permissions</span></span>
<span data-ttu-id="87320-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87320-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="87320-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="87320-109">Permission type</span></span>      | <span data-ttu-id="87320-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="87320-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="87320-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="87320-111">Delegated (work or school account)</span></span> | <span data-ttu-id="87320-112">PrivilegedAccess. ReadWrite. AzureAD, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="87320-112">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="87320-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="87320-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="87320-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="87320-114">Not supported.</span></span>    |
|<span data-ttu-id="87320-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="87320-115">Application</span></span> | <span data-ttu-id="87320-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="87320-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="87320-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="87320-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedApproval
```
## <a name="optional-query-parameters"></a><span data-ttu-id="87320-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="87320-118">Optional query parameters</span></span>
<span data-ttu-id="87320-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="87320-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="87320-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="87320-120">Request headers</span></span>
| <span data-ttu-id="87320-121">Nome</span><span class="sxs-lookup"><span data-stu-id="87320-121">Name</span></span>      |<span data-ttu-id="87320-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="87320-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="87320-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="87320-123">Authorization</span></span>  | <span data-ttu-id="87320-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="87320-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="87320-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="87320-126">Request body</span></span>
<span data-ttu-id="87320-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="87320-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="87320-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="87320-128">Response</span></span>

<span data-ttu-id="87320-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [privilegedApproval](../resources/privilegedapproval.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="87320-129">If successful, this method returns a `200 OK` response code and collection of [privilegedApproval](../resources/privilegedapproval.md) objects in the response body.</span></span>

<span data-ttu-id="87320-130">Observe que o locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="87320-130">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="87320-131">Caso contrário, o código de status HTTP 403 proibido será retornado.</span><span class="sxs-lookup"><span data-stu-id="87320-131">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="87320-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="87320-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="87320-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="87320-133">Request</span></span>
<span data-ttu-id="87320-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="87320-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedapproval"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedApproval
```
##### <a name="response"></a><span data-ttu-id="87320-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="87320-135">Response</span></span>
<span data-ttu-id="87320-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="87320-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedApproval",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 246

{
  "value": [
    {
      "id": "id-value",
      "userId": "userId-value",
      "roleId": "roleId-value",
      "approvalType": "approvalType-value",
      "approvalState": "approvalState-value",
      "approvalDuration": "datetime-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="87320-139">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="87320-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="87320-140">Basic</span><span class="sxs-lookup"><span data-stu-id="87320-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_privilegedapproval-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="87320-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="87320-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_privilegedapproval-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List privilegedApproval",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedapproval-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/privilegedapproval-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
