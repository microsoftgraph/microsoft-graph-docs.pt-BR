---
title: Obter contactFolder
description: Obtenha uma pasta de contatos usando a respectiva ID.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 5ab29eb96f900404f035442605047bd2df3e37e2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32455657"
---
# <a name="get-contactfolder"></a><span data-ttu-id="958f7-103">Obter contactFolder</span><span class="sxs-lookup"><span data-stu-id="958f7-103">Get contactFolder</span></span>

<span data-ttu-id="958f7-104">Obtenha uma pasta de contatos usando a respectiva ID.</span><span class="sxs-lookup"><span data-stu-id="958f7-104">Get a contact folder by using the contact folder ID.</span></span>

<span data-ttu-id="958f7-105">Há dois cenários em que um aplicativo pode obter a pasta de contatos de outro usuário:</span><span class="sxs-lookup"><span data-stu-id="958f7-105">There are two scenarios where an app can get another user's contact folder:</span></span>

* <span data-ttu-id="958f7-106">Se o aplicativo tiver permissões de aplicativo ou</span><span class="sxs-lookup"><span data-stu-id="958f7-106">If the app has application permissions, or,</span></span>
* <span data-ttu-id="958f7-107">Se o aplicativo tiver as [permissões](#permissions) delegadas apropriadas de um usuário, e outro usuário tiver compartilhado uma pasta de contatos com esse usuário, ou tiver concedido acesso delegado a esse usuário.</span><span class="sxs-lookup"><span data-stu-id="958f7-107">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="958f7-108">Confira [detalhes e um exemplo](/graph/outlook-get-shared-contacts-folders).</span><span class="sxs-lookup"><span data-stu-id="958f7-108">See [details and an example](/graph/outlook-get-shared-contacts-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="958f7-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="958f7-109">Permissions</span></span>
<span data-ttu-id="958f7-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="958f7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="958f7-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="958f7-112">Permission type</span></span>      | <span data-ttu-id="958f7-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="958f7-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="958f7-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="958f7-114">Delegated (work or school account)</span></span> | <span data-ttu-id="958f7-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="958f7-115">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="958f7-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="958f7-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="958f7-117">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="958f7-117">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="958f7-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="958f7-118">Application</span></span> | <span data-ttu-id="958f7-119">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="958f7-119">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="958f7-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="958f7-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="958f7-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="958f7-121">Optional query parameters</span></span>
<span data-ttu-id="958f7-122">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="958f7-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="958f7-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="958f7-123">Request headers</span></span>
| <span data-ttu-id="958f7-124">Nome</span><span class="sxs-lookup"><span data-stu-id="958f7-124">Name</span></span>       | <span data-ttu-id="958f7-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="958f7-125">Type</span></span> | <span data-ttu-id="958f7-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="958f7-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="958f7-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="958f7-127">Authorization</span></span>  | <span data-ttu-id="958f7-128">string</span><span class="sxs-lookup"><span data-stu-id="958f7-128">string</span></span>  | <span data-ttu-id="958f7-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="958f7-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="958f7-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="958f7-131">Request body</span></span>
<span data-ttu-id="958f7-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="958f7-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="958f7-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="958f7-133">Response</span></span>

<span data-ttu-id="958f7-134">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [contactFolder](../resources/contactfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="958f7-134">If successful, this method returns a `200 OK` response code and [contactFolder](../resources/contactfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="958f7-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="958f7-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="958f7-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="958f7-136">Request</span></span>
<span data-ttu-id="958f7-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="958f7-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contactfolder"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contactFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="958f7-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="958f7-138">Response</span></span>
<span data-ttu-id="958f7-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="958f7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 104

{
  "displayName": "Finance",
  "id": "AAMkAGI2TKI5AAA=",
  "parentFolderId": "AAMkAGI2AAEOAAA="
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get contactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
