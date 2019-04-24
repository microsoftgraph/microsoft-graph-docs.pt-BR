---
title: Membros transitivos do grupo de lista
description: Obtenha uma lista dos membros do grupo. Um grupo pode ter usuários, contatos, dispositivos, entidades de serviço e outros grupos como membros. Essa operação é transitiva e também retornará uma lista simples de todos os membros aninhados.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: e1dc5c2b89305373b22b6ef87cfaee25d6669750
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32502108"
---
# <a name="list-group-transitive-members"></a><span data-ttu-id="eab6f-105">Membros transitivos do grupo de lista</span><span class="sxs-lookup"><span data-stu-id="eab6f-105">List group transitive members</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eab6f-106">Obtenha uma lista dos membros do grupo.</span><span class="sxs-lookup"><span data-stu-id="eab6f-106">Get a list of the group's members.</span></span> <span data-ttu-id="eab6f-107">Um grupo pode ter usuários, contatos, dispositivos, entidades de serviço e outros grupos como membros.</span><span class="sxs-lookup"><span data-stu-id="eab6f-107">A group can have users, contacts, devices, service principals and other groups as members.</span></span> <span data-ttu-id="eab6f-108">Essa operação é transitiva e também retornará uma lista simples de todos os membros aninhados.</span><span class="sxs-lookup"><span data-stu-id="eab6f-108">This operation is transitive and will also return a flat list of all nested members.</span></span>

## <a name="permissions"></a><span data-ttu-id="eab6f-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="eab6f-109">Permissions</span></span>

<span data-ttu-id="eab6f-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eab6f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eab6f-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eab6f-112">Permission type</span></span>      | <span data-ttu-id="eab6f-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eab6f-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eab6f-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eab6f-114">Delegated (work or school account)</span></span> | <span data-ttu-id="eab6f-115">Directory. Read. All, Directory. AccessAsUser. All, User. ReadBasic. All, User. Read. All</span><span class="sxs-lookup"><span data-stu-id="eab6f-115">Directory.Read.All, Directory.AccessAsUser.All, User.ReadBasic.All, User.Read.All</span></span>    |
|<span data-ttu-id="eab6f-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eab6f-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eab6f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eab6f-117">Not supported.</span></span>    |
|<span data-ttu-id="eab6f-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eab6f-118">Application</span></span> | <span data-ttu-id="eab6f-119">Directory. Read. All, User. Read. All</span><span class="sxs-lookup"><span data-stu-id="eab6f-119">Directory.Read.All, User.Read.All</span></span> |

> <span data-ttu-id="eab6f-120">Observação: para listar os membros de um grupo de associação oculto, a permissão member. Read. Hidden é necessária.</span><span class="sxs-lookup"><span data-stu-id="eab6f-120">Note: To list the members of a hidden membership group, the Member.Read.Hidden permission is required.</span></span>

## <a name="http-request"></a><span data-ttu-id="eab6f-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eab6f-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/{id}/transitiveMembers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="eab6f-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="eab6f-122">Optional query parameters</span></span>

<span data-ttu-id="eab6f-123">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="eab6f-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="eab6f-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eab6f-124">Request headers</span></span>

| <span data-ttu-id="eab6f-125">Nome</span><span class="sxs-lookup"><span data-stu-id="eab6f-125">Name</span></span>       | <span data-ttu-id="eab6f-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="eab6f-126">Type</span></span> | <span data-ttu-id="eab6f-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="eab6f-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="eab6f-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="eab6f-128">Authorization</span></span>  | <span data-ttu-id="eab6f-129">string</span><span class="sxs-lookup"><span data-stu-id="eab6f-129">string</span></span>  | <span data-ttu-id="eab6f-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eab6f-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eab6f-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eab6f-132">Request body</span></span>

<span data-ttu-id="eab6f-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="eab6f-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eab6f-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="eab6f-134">Response</span></span>

<span data-ttu-id="eab6f-135">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eab6f-135">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eab6f-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eab6f-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="eab6f-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eab6f-137">Request</span></span>

<span data-ttu-id="eab6f-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="eab6f-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_transitivemembers"
}-->

```http
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMembers
```

### <a name="response"></a><span data-ttu-id="eab6f-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="eab6f-139">Response</span></span>

<span data-ttu-id="eab6f-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="eab6f-140">The following is an example of the response.</span></span>
><span data-ttu-id="eab6f-141">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="eab6f-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="eab6f-142">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eab6f-142">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    "@odata.type": "#microsoft.graph.user",
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
<!--
{
  "type": "#page.annotation",
  "description": "List transitive group members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-list-transitivemembers.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
