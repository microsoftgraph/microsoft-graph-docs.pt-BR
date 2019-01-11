---
title: Listar childFolders
description: 'Obter a coleção de pasta sob a pasta especificada. Você pode usar o `.../me/MailFolders` atalho para obter o nível superior '
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 3af208919b1f733e913d8ac374bb72608d8fa1aa
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837433"
---
# <a name="list-childfolders"></a><span data-ttu-id="14479-104">Listar childFolders</span><span class="sxs-lookup"><span data-stu-id="14479-104">List childFolders</span></span>

> <span data-ttu-id="14479-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="14479-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="14479-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="14479-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="14479-p103">Obtenha a coleção de pastas sob a pasta especificada. Você pode usar o atalho `.../me/MailFolders` para obter a coleção de pastas de nível superior e navegar até outra pasta.</span><span class="sxs-lookup"><span data-stu-id="14479-p103">Get the folder collection under the specified folder. You can use the `.../me/MailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="14479-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="14479-109">Permissions</span></span>
<span data-ttu-id="14479-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14479-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14479-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="14479-112">Permission type</span></span>      | <span data-ttu-id="14479-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="14479-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="14479-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="14479-114">Delegated (work or school account)</span></span> | <span data-ttu-id="14479-115">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="14479-115">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="14479-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="14479-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="14479-117">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="14479-117">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="14479-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="14479-118">Application</span></span> | <span data-ttu-id="14479-119">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="14479-119">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="14479-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="14479-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

## <a name="optional-query-parameters"></a><span data-ttu-id="14479-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="14479-121">Optional query parameters</span></span>
<span data-ttu-id="14479-122">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="14479-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="14479-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="14479-123">Request headers</span></span>
| <span data-ttu-id="14479-124">Nome</span><span class="sxs-lookup"><span data-stu-id="14479-124">Name</span></span>       | <span data-ttu-id="14479-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="14479-125">Type</span></span> | <span data-ttu-id="14479-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="14479-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="14479-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="14479-127">Authorization</span></span>  | <span data-ttu-id="14479-128">string</span><span class="sxs-lookup"><span data-stu-id="14479-128">string</span></span>  | <span data-ttu-id="14479-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="14479-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="14479-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="14479-131">Request body</span></span>
<span data-ttu-id="14479-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="14479-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="14479-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="14479-133">Response</span></span>
<span data-ttu-id="14479-134">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [MailFolder](../resources/mailfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="14479-134">If successful, this method returns a `200 OK` response code and collection of [MailFolder](../resources/mailfolder.md) objects in the response body.</span></span>

## <a name="example-1"></a><span data-ttu-id="14479-135">Exemplo 1</span><span class="sxs-lookup"><span data-stu-id="14479-135">Example 1</span></span>
#### <a name="request-1"></a><span data-ttu-id="14479-136">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="14479-136">Request 1</span></span>
<span data-ttu-id="14479-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="14479-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_childfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM/childFolders
```

#### <a name="response-1"></a><span data-ttu-id="14479-138">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="14479-138">Response 1</span></span>
<span data-ttu-id="14479-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="14479-139">The following is an example of the response.</span></span>
><span data-ttu-id="14479-140">**Observação:** no objeto response mostrado aqui pode ser reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="14479-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="14479-141">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="14479-141">All the properties will be returned from an actual call.</span></span>

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

## <a name="example-2"></a><span data-ttu-id="14479-142">Exemplo 2</span><span class="sxs-lookup"><span data-stu-id="14479-142">Example 2</span></span>
#### <a name="request-2"></a><span data-ttu-id="14479-143">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="14479-143">Request 2</span></span>
<span data-ttu-id="14479-144">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="14479-144">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_childfolders_of_searchfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailFolders/searchfolders/childFolders
```

#### <a name="response-2"></a><span data-ttu-id="14479-145">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="14479-145">Response 2</span></span>
<span data-ttu-id="14479-146">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="14479-146">The following is an example of the response.</span></span>
><span data-ttu-id="14479-147">**Observação:** no objeto response mostrado aqui pode ser reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="14479-147">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="14479-148">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="14479-148">All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "List childFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
