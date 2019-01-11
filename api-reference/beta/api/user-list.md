---
title: Listar usuários
description: Recupera uma lista de objetos de usuário.
author: dkershaw10
localization_priority: Priority
ms.openlocfilehash: 48b63f5a9ccc3616bd8ecee986cbf26dfedfb8d8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27890528"
---
# <a name="list-users"></a><span data-ttu-id="80476-103">Listar usuários</span><span class="sxs-lookup"><span data-stu-id="80476-103">List users</span></span>

> <span data-ttu-id="80476-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="80476-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="80476-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="80476-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="80476-106">Recuperar uma lista de objetos user.</span><span class="sxs-lookup"><span data-stu-id="80476-106">Retrieve a list of user objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="80476-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="80476-107">Permissions</span></span>

<span data-ttu-id="80476-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80476-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80476-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="80476-110">Permission type</span></span>      | <span data-ttu-id="80476-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="80476-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="80476-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="80476-112">Delegated (work or school account)</span></span> | <span data-ttu-id="80476-113">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="80476-113">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="80476-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="80476-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="80476-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="80476-115">Not supported.</span></span>    |
|<span data-ttu-id="80476-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="80476-116">Application</span></span> | <span data-ttu-id="80476-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80476-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="80476-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="80476-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="80476-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="80476-119">Optional query parameters</span></span>

<span data-ttu-id="80476-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="80476-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="80476-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="80476-121">Request headers</span></span>
| <span data-ttu-id="80476-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="80476-122">Header</span></span>        | <span data-ttu-id="80476-123">Valor</span><span class="sxs-lookup"><span data-stu-id="80476-123">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="80476-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="80476-124">Authorization</span></span> | <span data-ttu-id="80476-125">{token} do portador (obrigatório)</span><span class="sxs-lookup"><span data-stu-id="80476-125">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="80476-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="80476-126">Content-Type</span></span>  | <span data-ttu-id="80476-127">application/json</span><span class="sxs-lookup"><span data-stu-id="80476-127">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="80476-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="80476-128">Request body</span></span>

<span data-ttu-id="80476-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="80476-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="80476-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="80476-130">Response</span></span>

<span data-ttu-id="80476-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [user](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="80476-131">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80476-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="80476-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="80476-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="80476-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```http
GET https://graph.microsoft.com/beta/users
```

##### <a name="response"></a><span data-ttu-id="80476-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="80476-134">Response</span></span>

<span data-ttu-id="80476-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="80476-135">Here is an example of the response.</span></span> <span data-ttu-id="80476-136">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="80476-136">Note: The response object shown here may be truncated for brevity.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 608

{
  "value": [
    {
      "businessPhones": [
        "businessPhones-value"
      ],
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "jobTitle": "jobTitle-value",
      "mail": "mail-value",
      "mobilePhone": "mobilePhone-value",
      "officeLocation": "officeLocation-value",
      "preferredLanguage": "preferredLanguage-value",
      "surname": "surname-value",
      "userPrincipalName": "userPrincipalName-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List users",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
