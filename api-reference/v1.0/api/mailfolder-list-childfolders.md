---
title: Listar childFolders
description: 'Obtenha a coleção de pastas sob a pasta especificada. Você pode usar o `.../me/MailFolders` atalho para acessar o nível superior '
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 35d1f95c1bd47d43bce8100732f4f4cbc3e928ab
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33612747"
---
# <a name="list-childfolders"></a><span data-ttu-id="20d3b-104">Listar childFolders</span><span class="sxs-lookup"><span data-stu-id="20d3b-104">List childFolders</span></span>

<span data-ttu-id="20d3b-p102">Obtenha a coleção de pastas sob a pasta especificada. Você pode usar o atalho `.../me/MailFolders` para obter a coleção de pastas de nível superior e navegar até outra pasta.</span><span class="sxs-lookup"><span data-stu-id="20d3b-p102">Get the folder collection under the specified folder. You can use the `.../me/MailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="20d3b-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="20d3b-107">Permissions</span></span>
<span data-ttu-id="20d3b-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20d3b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20d3b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="20d3b-110">Permission type</span></span>      | <span data-ttu-id="20d3b-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="20d3b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="20d3b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="20d3b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="20d3b-113">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="20d3b-113">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="20d3b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="20d3b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="20d3b-115">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="20d3b-115">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="20d3b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="20d3b-116">Application</span></span> | <span data-ttu-id="20d3b-117">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="20d3b-117">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="20d3b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="20d3b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="20d3b-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="20d3b-119">Optional query parameters</span></span>
<span data-ttu-id="20d3b-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="20d3b-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="20d3b-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="20d3b-121">Request headers</span></span>
| <span data-ttu-id="20d3b-122">Nome</span><span class="sxs-lookup"><span data-stu-id="20d3b-122">Name</span></span>       | <span data-ttu-id="20d3b-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="20d3b-123">Type</span></span> | <span data-ttu-id="20d3b-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="20d3b-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="20d3b-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="20d3b-125">Authorization</span></span>  | <span data-ttu-id="20d3b-126">string</span><span class="sxs-lookup"><span data-stu-id="20d3b-126">string</span></span>  | <span data-ttu-id="20d3b-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="20d3b-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="20d3b-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="20d3b-129">Request body</span></span>
<span data-ttu-id="20d3b-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="20d3b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="20d3b-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="20d3b-131">Response</span></span>

<span data-ttu-id="20d3b-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [MailFolder](../resources/mailfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="20d3b-132">If successful, this method returns a `200 OK` response code and collection of [MailFolder](../resources/mailfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="20d3b-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="20d3b-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="20d3b-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="20d3b-134">Request</span></span>
<span data-ttu-id="20d3b-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="20d3b-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_childfolders"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}/childFolders
```
##### <a name="response"></a><span data-ttu-id="20d3b-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="20d3b-136">Response</span></span>
<span data-ttu-id="20d3b-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="20d3b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 232

{
  "value": [
    {
      "displayName": "displayName-value",
      "parentFolderId": "parentFolderId-value",
      "childFolderCount": 99,
      "unreadItemCount": 99,
      "totalItemCount": 99,
      "id": "id-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="20d3b-140">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="20d3b-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="20d3b-141">C#</span><span class="sxs-lookup"><span data-stu-id="20d3b-141">C</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_childfolders-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="20d3b-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="20d3b-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_childfolders-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List childFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/mailfolder-list-childfolders.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/mailfolder-list-childfolders.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
