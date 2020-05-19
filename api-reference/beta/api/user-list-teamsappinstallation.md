---
title: Lista de aplicativos instalados para o usuário
description: Recupere a lista de aplicativos instalados no escopo pessoal do usuário especificado.
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 79ba743eaa71101160fd836fac579148581b5615
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290634"
---
# <a name="list-apps-installed-for-user"></a><span data-ttu-id="9ee6c-103">Lista de aplicativos instalados para o usuário</span><span class="sxs-lookup"><span data-stu-id="9ee6c-103">List apps installed for user</span></span>

<span data-ttu-id="9ee6c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ee6c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ee6c-105">Recupere a lista de [aplicativos](../resources/teamsappinstallation.md) instalados no escopo pessoal do [usuário](../resources/user.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="9ee6c-105">Retrieve the list of [apps](../resources/teamsappinstallation.md) installed in the personal scope of the specified [user](../resources/user.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9ee6c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9ee6c-106">Permissions</span></span>

<span data-ttu-id="9ee6c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ee6c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ee6c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9ee6c-109">Permission type</span></span>      | <span data-ttu-id="9ee6c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9ee6c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9ee6c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9ee6c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9ee6c-112">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ee6c-112">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="9ee6c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9ee6c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ee6c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9ee6c-114">Not supported.</span></span>    |
|<span data-ttu-id="9ee6c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9ee6c-115">Application</span></span> | <span data-ttu-id="9ee6c-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ee6c-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9ee6c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9ee6c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{id}/teamwork/installedApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9ee6c-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9ee6c-118">Optional query parameters</span></span>

<span data-ttu-id="9ee6c-119">Este método dá suporte aos [Parâmetros de consulta OData](/graph/query-parameters) $filter, $select e $expand para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9ee6c-119">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9ee6c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9ee6c-120">Request headers</span></span>

| <span data-ttu-id="9ee6c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9ee6c-121">Header</span></span>       | <span data-ttu-id="9ee6c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9ee6c-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9ee6c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9ee6c-123">Authorization</span></span>  | <span data-ttu-id="9ee6c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9ee6c-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9ee6c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9ee6c-126">Request body</span></span>

<span data-ttu-id="9ee6c-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9ee6c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9ee6c-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ee6c-128">Response</span></span>

<span data-ttu-id="9ee6c-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [teamsAppInstallation](../resources/teamsappinstallation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9ee6c-129">If successful, this method returns a `200 OK` response code and a collection of [teamsAppInstallation](../resources/teamsappinstallation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9ee6c-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9ee6c-130">Examples</span></span>

### <a name="example-1-list-apps-installed-for-the-specified-user"></a><span data-ttu-id="9ee6c-131">Exemplo 1: listar aplicativos instalados para o usuário especificado</span><span class="sxs-lookup"><span data-stu-id="9ee6c-131">Example 1: List apps installed for the specified user</span></span>

#### <a name="request"></a><span data-ttu-id="9ee6c-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9ee6c-132">Request</span></span>

<span data-ttu-id="9ee6c-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9ee6c-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9ee6c-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="9ee6c-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_list_teamsApps"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/teamwork/installedApps
```
# <a name="c"></a>[<span data-ttu-id="9ee6c-135">C#</span><span class="sxs-lookup"><span data-stu-id="9ee6c-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-list-teamsapps-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9ee6c-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9ee6c-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-list-teamsapps-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9ee6c-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9ee6c-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-list-teamsapps-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9ee6c-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ee6c-138">Response</span></span>

<span data-ttu-id="9ee6c-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9ee6c-139">The following is an example of the response.</span></span>
><span data-ttu-id="9ee6c-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9ee6c-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "user_list_teamsApps",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```
### <a name="example-2-get-the-names-and-other-details-of-apps-installed-for-the-user"></a><span data-ttu-id="9ee6c-142">Exemplo 2: obter os nomes e outros detalhes dos aplicativos instalados para o usuário</span><span class="sxs-lookup"><span data-stu-id="9ee6c-142">Example 2: Get the names and other details of apps installed for the user</span></span>

#### <a name="request"></a><span data-ttu-id="9ee6c-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9ee6c-143">Request</span></span>

<span data-ttu-id="9ee6c-144">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9ee6c-144">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "user_list_teamsApps_details"
}-->
```http
GET https://graph.microsoft.com/beta/users/{id}/teamwork/installedApps?$expand=teamsAppDefinition
```

#### <a name="response"></a><span data-ttu-id="9ee6c-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ee6c-145">Response</span></span>

<span data-ttu-id="9ee6c-146">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9ee6c-146">The following is an example of the response.</span></span>

><span data-ttu-id="9ee6c-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9ee6c-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "user_list_teamsApps_details",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "NjRiOWM3NDYtYjE1NS00MDQyLThkNDctOTQxYmQzODE2ODFiIyMwZDgyMGVjZC1kZWYyLTQyOTctYWRhZC03ODA1NmNkZTdjNzg=",
            "teamsAppDefinition": {
                "id": "MGQ4MjBlY2QtZGVmMi00Mjk3LWFkYWQtNzgwNTZjZGU3Yzc4IyMxLjAuMA==",
                "teamsAppId": "0d820ecd-def2-4297-adad-78056cde7c78",
                "displayName": "OneNote",
                "version": "1.0.0"
            }
        },
        {
            "id": "NjRiOWM3NDYtYjE1NS00MDQyLThkNDctOTQxYmQzODE2ODFiIyMwZmQ5MjVhMC0zNTdmLTRkMjUtODQ1Ni1iMzAyMmFhYTQxYTk=",
            "teamsAppDefinition": {
                "id": "MGZkOTI1YTAtMzU3Zi00ZDI1LTg0NTYtYjMwMjJhYWE0MWE5IyMxLjc=",
                "teamsAppId": "0fd925a0-357f-4d25-8456-b3022aaa41a9",
                "displayName": "SurveyMonkey",
                "version": "1.7"
            }
        },
        {
            "id": "NjRiOWM3NDYtYjE1NS00MDQyLThkNDctOTQxYmQzODE2ODFiIyMyYTUyNzcwMy0xZjZmLTQ1NTktYTMzMi1kOGE3ZDI4OGNkODg=",
            "teamsAppDefinition": {
                "id": "MmE1Mjc3MDMtMWY2Zi00NTU5LWEzMzItZDhhN2QyODhjZDg4IyMxLjA=",
                "teamsAppId": "2a527703-1f6f-4559-a332-d8a7d288cd88",
                "displayName": "SharePoint",
                "version": "1.0"
            }
        }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "User list teamsAppInstallations",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
