---
title: Listar childFolders
description: 'Obter a coleção de pasta sob a pasta especificada. Você pode usar o `.../me/MailFolders` atalho para obter o nível superior '
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 1d1a002bef6d1e16c48cc484211abe752e4adbe7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819912"
---
# <a name="list-childfolders"></a><span data-ttu-id="ab6f9-104">Listar childFolders</span><span class="sxs-lookup"><span data-stu-id="ab6f9-104">List childFolders</span></span>

<span data-ttu-id="ab6f9-p102">Obtenha a coleção de pastas sob a pasta especificada. Você pode usar o atalho `.../me/MailFolders` para obter a coleção de pastas de nível superior e navegar até outra pasta.</span><span class="sxs-lookup"><span data-stu-id="ab6f9-p102">Get the folder collection under the specified folder. You can use the `.../me/MailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="ab6f9-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="ab6f9-107">Permissions</span></span>
<span data-ttu-id="ab6f9-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab6f9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab6f9-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ab6f9-110">Permission type</span></span>      | <span data-ttu-id="ab6f9-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ab6f9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ab6f9-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ab6f9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ab6f9-113">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ab6f9-113">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ab6f9-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ab6f9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab6f9-115">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ab6f9-115">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ab6f9-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ab6f9-116">Application</span></span> | <span data-ttu-id="ab6f9-117">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ab6f9-117">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ab6f9-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ab6f9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ab6f9-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ab6f9-119">Optional query parameters</span></span>
<span data-ttu-id="ab6f9-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ab6f9-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ab6f9-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ab6f9-121">Request headers</span></span>
| <span data-ttu-id="ab6f9-122">Nome</span><span class="sxs-lookup"><span data-stu-id="ab6f9-122">Name</span></span>       | <span data-ttu-id="ab6f9-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="ab6f9-123">Type</span></span> | <span data-ttu-id="ab6f9-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab6f9-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ab6f9-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="ab6f9-125">Authorization</span></span>  | <span data-ttu-id="ab6f9-126">string</span><span class="sxs-lookup"><span data-stu-id="ab6f9-126">string</span></span>  | <span data-ttu-id="ab6f9-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ab6f9-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ab6f9-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ab6f9-129">Request body</span></span>
<span data-ttu-id="ab6f9-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ab6f9-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ab6f9-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab6f9-131">Response</span></span>

<span data-ttu-id="ab6f9-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [MailFolder](../resources/mailfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ab6f9-132">If successful, this method returns a `200 OK` response code and collection of [MailFolder](../resources/mailfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ab6f9-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ab6f9-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ab6f9-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ab6f9-134">Request</span></span>
<span data-ttu-id="ab6f9-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ab6f9-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_childfolders"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}/childFolders
```
##### <a name="response"></a><span data-ttu-id="ab6f9-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab6f9-136">Response</span></span>
<span data-ttu-id="ab6f9-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ab6f9-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List childFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
