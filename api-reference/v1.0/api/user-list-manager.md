---
title: Listar gerente
description: Obtenha o gerente do usuário. Retorna o usuário ou contato atribuído como gerente do usuário.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ae243f0fa4c8212cecebedc39ebfc2d5713d5689
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32571314"
---
# <a name="list-manager"></a><span data-ttu-id="497c4-104">Listar gerente</span><span class="sxs-lookup"><span data-stu-id="497c4-104">List manager</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="497c4-105">Obtenha o gerente do usuário.</span><span class="sxs-lookup"><span data-stu-id="497c4-105">Get user's manager.</span></span> <span data-ttu-id="497c4-106">Retorna o usuário ou contato atribuído como gerente do usuário.</span><span class="sxs-lookup"><span data-stu-id="497c4-106">Returns the user or contact assigned as the user's manager.</span></span>
## <a name="permissions"></a><span data-ttu-id="497c4-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="497c4-107">Permissions</span></span>
<span data-ttu-id="497c4-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="497c4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="497c4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="497c4-110">Permission type</span></span>      | <span data-ttu-id="497c4-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="497c4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="497c4-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="497c4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="497c4-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="497c4-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="497c4-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="497c4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="497c4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="497c4-115">Not supported.</span></span>    |
|<span data-ttu-id="497c4-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="497c4-116">Application</span></span> | <span data-ttu-id="497c4-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="497c4-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="497c4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="497c4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/manager
```
## <a name="optional-query-parameters"></a><span data-ttu-id="497c4-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="497c4-119">Optional query parameters</span></span>
<span data-ttu-id="497c4-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="497c4-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="497c4-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="497c4-121">Request headers</span></span>
| <span data-ttu-id="497c4-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="497c4-122">Header</span></span>       | <span data-ttu-id="497c4-123">Valor</span><span class="sxs-lookup"><span data-stu-id="497c4-123">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="497c4-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="497c4-124">Authorization</span></span>  | <span data-ttu-id="497c4-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="497c4-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="497c4-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="497c4-127">Content-Type</span></span>   | <span data-ttu-id="497c4-128">application/json</span><span class="sxs-lookup"><span data-stu-id="497c4-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="497c4-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="497c4-129">Request body</span></span>
<span data-ttu-id="497c4-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="497c4-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="497c4-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="497c4-131">Response</span></span>

<span data-ttu-id="497c4-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="497c4-132">If successful, this method returns a `200 OK` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="497c4-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="497c4-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="497c4-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="497c4-134">Request</span></span>
<span data-ttu-id="497c4-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="497c4-135">Here is an example of the request.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/users/{id|userPrincipalName}/manager
```
##### <a name="response"></a><span data-ttu-id="497c4-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="497c4-136">Response</span></span>
<span data-ttu-id="497c4-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="497c4-137">Here is an example of the response.</span></span>
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
