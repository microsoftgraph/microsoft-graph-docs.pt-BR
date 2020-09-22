---
title: Listar gerente
description: Obtenha o gerente do usuário. Retorna o usuário ou contato atribuído como gerente do usuário.
localization_priority: Normal
author: krbain
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 178da2aee1dcc25dbd29a32c2041f6d8150caed6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016874"
---
# <a name="list-manager"></a><span data-ttu-id="0fd87-104">Listar gerente</span><span class="sxs-lookup"><span data-stu-id="0fd87-104">List manager</span></span>

<span data-ttu-id="0fd87-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0fd87-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0fd87-106">Obtenha o gerente do usuário.</span><span class="sxs-lookup"><span data-stu-id="0fd87-106">Get user's manager.</span></span> <span data-ttu-id="0fd87-107">Retorna o usuário ou contato atribuído como gerente do usuário.</span><span class="sxs-lookup"><span data-stu-id="0fd87-107">Returns the user or contact assigned as the user's manager.</span></span>
## <a name="permissions"></a><span data-ttu-id="0fd87-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="0fd87-108">Permissions</span></span>
<span data-ttu-id="0fd87-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0fd87-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0fd87-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0fd87-111">Permission type</span></span>      | <span data-ttu-id="0fd87-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0fd87-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0fd87-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0fd87-113">Delegated (work or school account)</span></span> | <span data-ttu-id="0fd87-114">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0fd87-114">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0fd87-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0fd87-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0fd87-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0fd87-116">Not supported.</span></span>    |
|<span data-ttu-id="0fd87-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0fd87-117">Application</span></span> | <span data-ttu-id="0fd87-118">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fd87-118">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="0fd87-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0fd87-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/manager
GET /users/{id | userPrincipalName}/manager
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0fd87-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0fd87-120">Optional query parameters</span></span>
<span data-ttu-id="0fd87-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0fd87-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="0fd87-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0fd87-122">Request headers</span></span>
| <span data-ttu-id="0fd87-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0fd87-123">Header</span></span>       | <span data-ttu-id="0fd87-124">Valor</span><span class="sxs-lookup"><span data-stu-id="0fd87-124">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="0fd87-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="0fd87-125">Authorization</span></span>  | <span data-ttu-id="0fd87-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0fd87-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0fd87-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0fd87-128">Content-Type</span></span>   | <span data-ttu-id="0fd87-129">application/json</span><span class="sxs-lookup"><span data-stu-id="0fd87-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0fd87-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0fd87-130">Request body</span></span>
<span data-ttu-id="0fd87-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0fd87-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0fd87-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="0fd87-132">Response</span></span>

<span data-ttu-id="0fd87-133">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0fd87-133">If successful, this method returns a `200 OK` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0fd87-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0fd87-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0fd87-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0fd87-135">Request</span></span>
<span data-ttu-id="0fd87-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0fd87-136">Here is an example of the request.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/users/{id|userPrincipalName}/manager
```
##### <a name="response"></a><span data-ttu-id="0fd87-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="0fd87-137">Response</span></span>
<span data-ttu-id="0fd87-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0fd87-138">Here is an example of the response.</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "objectType": "User",
  "id": "111048d2-2761-4347-b978-07354283363b",
  "accountEnabled": true,
  "city": "San Diego",
  "country": "United States",
  "department": "Sales & Marketing",
  "displayName": "Sara Davis",
  "givenName": "Sara",
  "jobTitle": "Finance VP",
  "mail": "SaraD@contoso.onmicrosoft.com",
  "mailNickname": "SaraD",
  "state": "CA",
  "streetAddress": "9256 Towne Center Dr., Suite 400",
  "surname": "Davis",
  "usageLocation": "US",
  "userPrincipalName": "SaraD@contoso.onmicrosoft.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List directReports",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


