---
title: Membros do grupo de lista transitivos
description: Obtenha uma lista de membros do grupo. Um grupo pode ter usuários, contatos, dispositivos, entidades de serviço e outros grupos como membros. Essa operação é transitiva e também retornará uma lista simples de todos os membros aninhados.
localization_priority: Normal
ms.openlocfilehash: a89894bf17d12f7cd23350f466e9e1272fa0cb6a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27892215"
---
# <a name="list-group-transitive-members"></a><span data-ttu-id="a935a-105">Membros do grupo de lista transitivos</span><span class="sxs-lookup"><span data-stu-id="a935a-105">List group transitive members</span></span>

> <span data-ttu-id="a935a-106">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a935a-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a935a-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a935a-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a935a-108">Obtenha uma lista de membros do grupo.</span><span class="sxs-lookup"><span data-stu-id="a935a-108">Get a list of the group's members.</span></span> <span data-ttu-id="a935a-109">Um grupo pode ter usuários, contatos, dispositivos, entidades de serviço e outros grupos como membros.</span><span class="sxs-lookup"><span data-stu-id="a935a-109">A group can have users, contacts, devices, service principals and other groups as members.</span></span> <span data-ttu-id="a935a-110">Essa operação é transitiva e também retornará uma lista simples de todos os membros aninhados.</span><span class="sxs-lookup"><span data-stu-id="a935a-110">This operation is transitive and will also return a flat list of all nested members.</span></span>

## <a name="permissions"></a><span data-ttu-id="a935a-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="a935a-111">Permissions</span></span>

<span data-ttu-id="a935a-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a935a-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a935a-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a935a-114">Permission type</span></span>      | <span data-ttu-id="a935a-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a935a-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a935a-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a935a-116">Delegated (work or school account)</span></span> | <span data-ttu-id="a935a-117">Directory.Read.All, Directory.AccessAsUser.All, User.ReadBasic.All, User.Read.All</span><span class="sxs-lookup"><span data-stu-id="a935a-117">Directory.Read.All, Directory.AccessAsUser.All, User.ReadBasic.All, User.Read.All</span></span>    |
|<span data-ttu-id="a935a-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a935a-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a935a-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a935a-119">Not supported.</span></span>    |
|<span data-ttu-id="a935a-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a935a-120">Application</span></span> | <span data-ttu-id="a935a-121">Directory.Read.All, User.Read.All</span><span class="sxs-lookup"><span data-stu-id="a935a-121">Directory.Read.All, User.Read.All</span></span> |

> <span data-ttu-id="a935a-122">Observação: Para listar os membros de um grupo de associação oculta, a permissão de Member.Read.Hidden é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a935a-122">Note: To list the members of a hidden membership group, the Member.Read.Hidden permission is required.</span></span>

## <a name="http-request"></a><span data-ttu-id="a935a-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a935a-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/{id}/transitiveMembers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a935a-124">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a935a-124">Optional query parameters</span></span>

<span data-ttu-id="a935a-125">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a935a-125">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a935a-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a935a-126">Request headers</span></span>

| <span data-ttu-id="a935a-127">Nome</span><span class="sxs-lookup"><span data-stu-id="a935a-127">Name</span></span>       | <span data-ttu-id="a935a-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="a935a-128">Type</span></span> | <span data-ttu-id="a935a-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="a935a-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a935a-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="a935a-130">Authorization</span></span>  | <span data-ttu-id="a935a-131">string</span><span class="sxs-lookup"><span data-stu-id="a935a-131">string</span></span>  | <span data-ttu-id="a935a-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a935a-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a935a-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a935a-134">Request body</span></span>

<span data-ttu-id="a935a-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a935a-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a935a-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="a935a-136">Response</span></span>

<span data-ttu-id="a935a-137">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a935a-137">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a935a-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a935a-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="a935a-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a935a-139">Request</span></span>

<span data-ttu-id="a935a-140">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a935a-140">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_transitivemembers"
}-->

```http
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMembers
```

### <a name="response"></a><span data-ttu-id="a935a-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="a935a-141">Response</span></span>

<span data-ttu-id="a935a-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a935a-142">The following is an example of the response.</span></span>
><span data-ttu-id="a935a-143">**Observação:** no objeto response mostrado aqui pode ser reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a935a-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a935a-144">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a935a-144">All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List transitive group members",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
