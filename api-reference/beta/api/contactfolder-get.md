---
title: Obter contactFolder
description: Obtenha uma pasta de contatos usando a respectiva ID.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 86f2adf867737e31d96a75d40f50442b10a468b0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27985113"
---
# <a name="get-contactfolder"></a><span data-ttu-id="b9a8b-103">Obter contactFolder</span><span class="sxs-lookup"><span data-stu-id="b9a8b-103">Get contactFolder</span></span>

> <span data-ttu-id="b9a8b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b9a8b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b9a8b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b9a8b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b9a8b-106">Obtenha uma pasta de contatos usando a respectiva ID.</span><span class="sxs-lookup"><span data-stu-id="b9a8b-106">Get a contact folder by using the contact folder ID.</span></span>

<span data-ttu-id="b9a8b-107">Há dois cenários onde um aplicativo pode obter a pasta de contato do outro usuário:</span><span class="sxs-lookup"><span data-stu-id="b9a8b-107">There are two scenarios where an app can get another user's contact folder:</span></span>

* <span data-ttu-id="b9a8b-108">Se o aplicativo tem permissões de aplicativo, ou,</span><span class="sxs-lookup"><span data-stu-id="b9a8b-108">If the app has application permissions, or,</span></span>
* <span data-ttu-id="b9a8b-109">Se o aplicativo tiver apropriada [permissões](#permissions) delegadas de um usuário, e outro usuário compartilhou uma pasta de contato com que o usuário ou, tem acesso delegado a esse usuário.</span><span class="sxs-lookup"><span data-stu-id="b9a8b-109">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="b9a8b-110">Consulte os [detalhes e um exemplo](/graph/outlook-get-shared-contacts-folders).</span><span class="sxs-lookup"><span data-stu-id="b9a8b-110">See [details and an example](/graph/outlook-get-shared-contacts-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="b9a8b-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="b9a8b-111">Permissions</span></span>
<span data-ttu-id="b9a8b-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9a8b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9a8b-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b9a8b-114">Permission type</span></span>      | <span data-ttu-id="b9a8b-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b9a8b-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b9a8b-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b9a8b-116">Delegated (work or school account)</span></span> | <span data-ttu-id="b9a8b-117">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b9a8b-117">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="b9a8b-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b9a8b-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9a8b-119">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b9a8b-119">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="b9a8b-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b9a8b-120">Application</span></span> | <span data-ttu-id="b9a8b-121">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b9a8b-121">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b9a8b-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b9a8b-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b9a8b-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b9a8b-123">Optional query parameters</span></span>
<span data-ttu-id="b9a8b-124">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b9a8b-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b9a8b-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b9a8b-125">Request headers</span></span>
| <span data-ttu-id="b9a8b-126">Nome</span><span class="sxs-lookup"><span data-stu-id="b9a8b-126">Name</span></span>       | <span data-ttu-id="b9a8b-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="b9a8b-127">Type</span></span> | <span data-ttu-id="b9a8b-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9a8b-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b9a8b-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="b9a8b-129">Authorization</span></span>  | <span data-ttu-id="b9a8b-130">string</span><span class="sxs-lookup"><span data-stu-id="b9a8b-130">string</span></span>  | <span data-ttu-id="b9a8b-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b9a8b-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b9a8b-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b9a8b-133">Request body</span></span>
<span data-ttu-id="b9a8b-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b9a8b-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b9a8b-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9a8b-135">Response</span></span>

<span data-ttu-id="b9a8b-136">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [contactFolder](../resources/contactfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b9a8b-136">If successful, this method returns a `200 OK` response code and [contactFolder](../resources/contactfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b9a8b-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b9a8b-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b9a8b-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b9a8b-138">Request</span></span>
<span data-ttu-id="b9a8b-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b9a8b-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contactfolder"
}-->
```http
GET https://graph.microsoft.com/beta/me/contactFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="b9a8b-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9a8b-140">Response</span></span>
<span data-ttu-id="b9a8b-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b9a8b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "parentFolderId": "AAMkAGI2AAEOAAA=",
  "wellKnownName": null
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
