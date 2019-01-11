---
title: Listar gerente
description: Obtenha o gerente do usuário. Retorna o usuário ou contato atribuído como gerente do usuário.
localization_priority: Normal
ms.openlocfilehash: 6f88aaf04596ade1a1cfd280af13efbc02affad6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27814970"
---
# <a name="list-manager"></a><span data-ttu-id="8ec33-104">Listar gerente</span><span class="sxs-lookup"><span data-stu-id="8ec33-104">List manager</span></span>

> <span data-ttu-id="8ec33-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8ec33-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8ec33-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8ec33-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8ec33-p103">Obtenha o gerente do usuário. Retorna o usuário ou contato atribuído como gerente do usuário.</span><span class="sxs-lookup"><span data-stu-id="8ec33-p103">Get user's manager. Returns the user or contact assigned as the user's manager.</span></span>
## <a name="permissions"></a><span data-ttu-id="8ec33-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="8ec33-109">Permissions</span></span>
<span data-ttu-id="8ec33-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ec33-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ec33-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8ec33-112">Permission type</span></span>      | <span data-ttu-id="8ec33-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8ec33-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8ec33-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8ec33-114">Delegated (work or school account)</span></span> | <span data-ttu-id="8ec33-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8ec33-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8ec33-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8ec33-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ec33-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8ec33-117">Not supported.</span></span>    |
|<span data-ttu-id="8ec33-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8ec33-118">Application</span></span> | <span data-ttu-id="8ec33-119">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ec33-119">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8ec33-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8ec33-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/manager
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8ec33-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8ec33-121">Optional query parameters</span></span>
<span data-ttu-id="8ec33-122">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8ec33-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="8ec33-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8ec33-123">Request headers</span></span>
| <span data-ttu-id="8ec33-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8ec33-124">Header</span></span>       | <span data-ttu-id="8ec33-125">Valor</span><span class="sxs-lookup"><span data-stu-id="8ec33-125">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="8ec33-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="8ec33-126">Authorization</span></span>  | <span data-ttu-id="8ec33-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8ec33-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8ec33-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8ec33-129">Content-Type</span></span>   | <span data-ttu-id="8ec33-130">application/json</span><span class="sxs-lookup"><span data-stu-id="8ec33-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8ec33-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8ec33-131">Request body</span></span>
<span data-ttu-id="8ec33-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8ec33-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8ec33-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ec33-133">Response</span></span>

<span data-ttu-id="8ec33-134">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8ec33-134">If successful, this method returns a `200 OK` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8ec33-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8ec33-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8ec33-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8ec33-136">Request</span></span>
<span data-ttu-id="8ec33-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8ec33-137">Here is an example of the request.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/users/{id|userPrincipalName}/manager
```
##### <a name="response"></a><span data-ttu-id="8ec33-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ec33-138">Response</span></span>
<span data-ttu-id="8ec33-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8ec33-139">Here is an example of the response.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List directReports",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
