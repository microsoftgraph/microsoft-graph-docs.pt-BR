---
title: Listar gerente
description: Obtenha o gerente do usuário. Retorna o usuário ou contato atribuído como gerente do usuário.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 87f57712bbef74864b6100527391d9f3c56f8455
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516095"
---
# <a name="list-manager"></a><span data-ttu-id="2df75-104">Listar gerente</span><span class="sxs-lookup"><span data-stu-id="2df75-104">List manager</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2df75-p102">Obtenha o gerente do usuário. Retorna o usuário ou contato atribuído como gerente do usuário.</span><span class="sxs-lookup"><span data-stu-id="2df75-p102">Get user's manager. Returns the user or contact assigned as the user's manager.</span></span>
## <a name="permissions"></a><span data-ttu-id="2df75-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="2df75-107">Permissions</span></span>
<span data-ttu-id="2df75-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2df75-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2df75-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2df75-110">Permission type</span></span>      | <span data-ttu-id="2df75-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2df75-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2df75-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2df75-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2df75-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2df75-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2df75-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2df75-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2df75-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2df75-115">Not supported.</span></span>    |
|<span data-ttu-id="2df75-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2df75-116">Application</span></span> | <span data-ttu-id="2df75-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2df75-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2df75-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2df75-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/manager
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2df75-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2df75-119">Optional query parameters</span></span>
<span data-ttu-id="2df75-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2df75-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="2df75-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2df75-121">Request headers</span></span>
| <span data-ttu-id="2df75-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2df75-122">Header</span></span>       | <span data-ttu-id="2df75-123">Valor</span><span class="sxs-lookup"><span data-stu-id="2df75-123">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="2df75-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="2df75-124">Authorization</span></span>  | <span data-ttu-id="2df75-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2df75-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2df75-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2df75-127">Content-Type</span></span>   | <span data-ttu-id="2df75-128">application/json</span><span class="sxs-lookup"><span data-stu-id="2df75-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2df75-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2df75-129">Request body</span></span>
<span data-ttu-id="2df75-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2df75-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2df75-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="2df75-131">Response</span></span>

<span data-ttu-id="2df75-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2df75-132">If successful, this method returns a `200 OK` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2df75-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2df75-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2df75-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2df75-134">Request</span></span>
<span data-ttu-id="2df75-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2df75-135">Here is an example of the request.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/users/{id|userPrincipalName}/manager
```
##### <a name="response"></a><span data-ttu-id="2df75-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="2df75-136">Response</span></span>
<span data-ttu-id="2df75-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2df75-137">Here is an example of the response.</span></span>
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
  "suppressions": [
    "Error: /api-reference/beta/api/user-list-manager.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
