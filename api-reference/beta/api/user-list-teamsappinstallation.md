---
title: Listar aplicativos instalados para o usuário
description: Recupere a lista de aplicativos instalados no escopo pessoal do usuário especificado.
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c31e731aba27fff245ecd92fc9d93d20d2c1fe27
ms.sourcegitcommit: 82b73552fff79a4ef7a2ee57fc2d1b3286b5bd4c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/26/2019
ms.locfileid: "35908548"
---
# <a name="list-apps-installed-for-user"></a><span data-ttu-id="05c30-103">Listar aplicativos instalados para o usuário</span><span class="sxs-lookup"><span data-stu-id="05c30-103">List apps installed for user</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="05c30-104">Recupere a lista de [aplicativos](../resources/teamsappinstallation.md) instalados no escopo pessoal do [usuário](../resources/user.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="05c30-104">Retrieve the list of [apps](../resources/teamsappinstallation.md) installed in the personal scope of the specified [user](../resources/user.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="05c30-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="05c30-105">Permissions</span></span>

<span data-ttu-id="05c30-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05c30-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05c30-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="05c30-108">Permission type</span></span>      | <span data-ttu-id="05c30-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="05c30-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="05c30-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="05c30-110">Delegated (work or school account)</span></span> | <span data-ttu-id="05c30-111">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05c30-111">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="05c30-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="05c30-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="05c30-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="05c30-113">Not supported.</span></span>    |
|<span data-ttu-id="05c30-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="05c30-114">Application</span></span> | <span data-ttu-id="05c30-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05c30-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="05c30-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="05c30-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{id}/teamwork/installedApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="05c30-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="05c30-117">Optional query parameters</span></span>

<span data-ttu-id="05c30-118">Este método dá suporte aos [Parâmetros de consulta OData](/graph/query-parameters) $filter, $select e $expand para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="05c30-118">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="05c30-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="05c30-119">Request headers</span></span>

| <span data-ttu-id="05c30-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="05c30-120">Header</span></span>       | <span data-ttu-id="05c30-121">Valor</span><span class="sxs-lookup"><span data-stu-id="05c30-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="05c30-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="05c30-122">Authorization</span></span>  | <span data-ttu-id="05c30-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="05c30-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="05c30-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="05c30-125">Request body</span></span>

<span data-ttu-id="05c30-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="05c30-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="05c30-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="05c30-127">Response</span></span>

<span data-ttu-id="05c30-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [teamsAppInstallation](../resources/teamsappinstallation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="05c30-128">If successful, this method returns a `200 OK` response code and a collection of [teamsAppInstallation](../resources/teamsappinstallation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="05c30-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="05c30-129">Examples</span></span>

### <a name="example-1-list-apps-installed-for-the-specified-user"></a><span data-ttu-id="05c30-130">Exemplo 1: listar aplicativos instalados para o usuário especificado</span><span class="sxs-lookup"><span data-stu-id="05c30-130">Example 1: List apps installed for the specified user</span></span>

#### <a name="request"></a><span data-ttu-id="05c30-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="05c30-131">Request</span></span>

<span data-ttu-id="05c30-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="05c30-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_list_teamsApps"
}-->
```http
GET https://graph.microsoft.com/beta/users/{id}/teamwork/installedApps
```

#### <a name="response"></a><span data-ttu-id="05c30-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="05c30-133">Response</span></span>

<span data-ttu-id="05c30-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="05c30-134">The following is an example of the response.</span></span>
><span data-ttu-id="05c30-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="05c30-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
### <a name="example-2-get-the-names-and-other-details-of-apps-installed-for-the-user"></a><span data-ttu-id="05c30-137">Exemplo 2: obter os nomes e outros detalhes dos aplicativos instalados para o usuário</span><span class="sxs-lookup"><span data-stu-id="05c30-137">Example 2: Get the names and other details of apps installed for the user</span></span>

#### <a name="request"></a><span data-ttu-id="05c30-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="05c30-138">Request</span></span>

<span data-ttu-id="05c30-139">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="05c30-139">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "user_list_teamsApps_details"
}-->
```http
GET https://graph.microsoft.com/beta/users/{id}/teamwork/installedApps?$expand=teamsAppDefinition
```

#### <a name="response"></a><span data-ttu-id="05c30-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="05c30-140">Response</span></span>

<span data-ttu-id="05c30-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="05c30-141">The following is an example of the response.</span></span>

><span data-ttu-id="05c30-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="05c30-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
