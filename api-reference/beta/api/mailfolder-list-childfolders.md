---
title: Listar childFolders
description: 'Obter a coleção de pasta sob a pasta especificada. Você pode usar o `.../me/MailFolders` atalho para obter o nível superior '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 9d54828b97bb82c9ce0ee9eceeee86a4aa975c3d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512546"
---
# <a name="list-childfolders"></a><span data-ttu-id="54986-104">Listar childFolders</span><span class="sxs-lookup"><span data-stu-id="54986-104">List childFolders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="54986-p102">Obtenha a coleção de pastas sob a pasta especificada. Você pode usar o atalho `.../me/MailFolders` para obter a coleção de pastas de nível superior e navegar até outra pasta.</span><span class="sxs-lookup"><span data-stu-id="54986-p102">Get the folder collection under the specified folder. You can use the `.../me/MailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="54986-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="54986-107">Permissions</span></span>
<span data-ttu-id="54986-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54986-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54986-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="54986-110">Permission type</span></span>      | <span data-ttu-id="54986-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="54986-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="54986-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="54986-112">Delegated (work or school account)</span></span> | <span data-ttu-id="54986-113">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="54986-113">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="54986-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="54986-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="54986-115">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="54986-115">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="54986-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="54986-116">Application</span></span> | <span data-ttu-id="54986-117">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="54986-117">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="54986-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="54986-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

## <a name="optional-query-parameters"></a><span data-ttu-id="54986-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="54986-119">Optional query parameters</span></span>
<span data-ttu-id="54986-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="54986-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="54986-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="54986-121">Request headers</span></span>
| <span data-ttu-id="54986-122">Nome</span><span class="sxs-lookup"><span data-stu-id="54986-122">Name</span></span>       | <span data-ttu-id="54986-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="54986-123">Type</span></span> | <span data-ttu-id="54986-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="54986-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="54986-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="54986-125">Authorization</span></span>  | <span data-ttu-id="54986-126">string</span><span class="sxs-lookup"><span data-stu-id="54986-126">string</span></span>  | <span data-ttu-id="54986-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="54986-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="54986-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="54986-129">Request body</span></span>
<span data-ttu-id="54986-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="54986-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="54986-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="54986-131">Response</span></span>
<span data-ttu-id="54986-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [MailFolder](../resources/mailfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="54986-132">If successful, this method returns a `200 OK` response code and collection of [MailFolder](../resources/mailfolder.md) objects in the response body.</span></span>

## <a name="example-1"></a><span data-ttu-id="54986-133">Exemplo 1</span><span class="sxs-lookup"><span data-stu-id="54986-133">Example 1</span></span>
#### <a name="request-1"></a><span data-ttu-id="54986-134">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="54986-134">Request 1</span></span>
<span data-ttu-id="54986-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="54986-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_childfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM/childFolders
```

#### <a name="response-1"></a><span data-ttu-id="54986-136">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="54986-136">Response 1</span></span>
<span data-ttu-id="54986-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="54986-137">The following is an example of the response.</span></span>
><span data-ttu-id="54986-138">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="54986-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="54986-139">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="54986-139">All the properties will be returned from an actual call.</span></span>

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
        "id": "AAMkAGVmMDEzA",
        "displayName": "Internal Screens",
        "parentFolderId": "AAMkAGVmMDEzM",
        "childFolderCount": 0,
        "unreadItemCount": 2,
        "totalItemCount": 2,
        "wellKnownName": null
    },
    {
        "id": "AAMkAGVmMDEzB",
        "displayName": "Project Falcon",
        "parentFolderId": "AAMkAGVmMDEzM",
        "childFolderCount": 0,
        "unreadItemCount": 5,
        "totalItemCount": 5,
        "wellKnownName": null
    },
    {
        "id": "AAMkAGVmMDEzMA",
        "displayName": "Finder",
        "parentFolderId": "AAMkAGVmMDEzM",
        "childFolderCount": 4,
        "unreadItemCount": 0,
        "totalItemCount": 0,
        "wellKnownName": "searchfolders"
    }
  ]
}
```

## <a name="example-2"></a><span data-ttu-id="54986-140">Exemplo 2</span><span class="sxs-lookup"><span data-stu-id="54986-140">Example 2</span></span>
#### <a name="request-2"></a><span data-ttu-id="54986-141">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="54986-141">Request 2</span></span>
<span data-ttu-id="54986-142">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="54986-142">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_childfolders_of_searchfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailFolders/searchfolders/childFolders
```

#### <a name="response-2"></a><span data-ttu-id="54986-143">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="54986-143">Response 2</span></span>
<span data-ttu-id="54986-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="54986-144">The following is an example of the response.</span></span>
><span data-ttu-id="54986-145">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="54986-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="54986-146">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="54986-146">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailSearchFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 232

{
  "value": [
    {
        "id": "AAMkAGVmMDEzA",
        "displayName": "Internal Screens",
        "parentFolderId": "AAMkAGVmMDEzM",
        "childFolderCount": 0,
        "unreadItemCount": 2,
        "totalItemCount": 2,
        "wellKnownName": null
    },
    {
        "id": "AAMkAGVmMDEzB",
        "displayName": "Project Falcon",
        "parentFolderId": "AAMkAGVmMDEzM",
        "childFolderCount": 0,
        "unreadItemCount": 5,
        "totalItemCount": 5,
        "wellKnownName": null
    },
    {
        "id": "AAMkAGVmMDEzMA",
        "displayName": "Finder",
        "parentFolderId": "AAMkAGVmMDEzM",
        "childFolderCount": 4,
        "unreadItemCount": 0,
        "totalItemCount": 0,
        "wellKnownName": "searchfolders"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List childFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/mailfolder-list-childfolders.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
