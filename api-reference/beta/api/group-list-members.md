---
title: Membros do grupo de lista
description: Obtenha uma lista de membros de direto do grupo. Um grupo pode ter usuários, contatos, dispositivos, entidades de serviço e outros grupos como membros. Esta operação não é transitiva.
localization_priority: Normal
ms.openlocfilehash: af54ef994fb0f62af43bf9f9ce3cd5fe5d2b1503
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27854135"
---
# <a name="list-group-members"></a><span data-ttu-id="0e6a5-105">Membros do grupo de lista</span><span class="sxs-lookup"><span data-stu-id="0e6a5-105">List group members</span></span>

> <span data-ttu-id="0e6a5-106">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0e6a5-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0e6a5-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0e6a5-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0e6a5-108">Obtenha uma lista de membros de direto do grupo.</span><span class="sxs-lookup"><span data-stu-id="0e6a5-108">Get a list of the group's direct members.</span></span> <span data-ttu-id="0e6a5-109">Um grupo pode ter usuários, contatos, dispositivos, entidades de serviço e outros grupos como membros.</span><span class="sxs-lookup"><span data-stu-id="0e6a5-109">A group can have users, contacts, devices, service principals, and other groups as members.</span></span> <span data-ttu-id="0e6a5-110">Esta operação não é transitiva.</span><span class="sxs-lookup"><span data-stu-id="0e6a5-110">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="0e6a5-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="0e6a5-111">Permissions</span></span>

<span data-ttu-id="0e6a5-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e6a5-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e6a5-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0e6a5-114">Permission type</span></span>      | <span data-ttu-id="0e6a5-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0e6a5-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0e6a5-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0e6a5-116">Delegated (work or school account)</span></span> | <span data-ttu-id="0e6a5-117">Directory.Read.All, Directory.AccessAsUser.All, User.ReadBasic.All, User.Read.All</span><span class="sxs-lookup"><span data-stu-id="0e6a5-117">Directory.Read.All, Directory.AccessAsUser.All, User.ReadBasic.All, User.Read.All</span></span>    |
|<span data-ttu-id="0e6a5-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0e6a5-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e6a5-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0e6a5-119">Not supported.</span></span>    |
|<span data-ttu-id="0e6a5-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0e6a5-120">Application</span></span> | <span data-ttu-id="0e6a5-121">Directory.Read.All, User.Read.All</span><span class="sxs-lookup"><span data-stu-id="0e6a5-121">Directory.Read.All, User.Read.All</span></span> |

> <span data-ttu-id="0e6a5-122">Observação: Para listar os membros de um grupo de associação oculta, a permissão de Member.Read.Hidden é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0e6a5-122">Note: To list the members of a hidden membership group, the Member.Read.Hidden permission is required.</span></span>
 
## <a name="http-request"></a><span data-ttu-id="0e6a5-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0e6a5-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0e6a5-124">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0e6a5-124">Optional query parameters</span></span>
<span data-ttu-id="0e6a5-125">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0e6a5-125">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0e6a5-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0e6a5-126">Request headers</span></span>
| <span data-ttu-id="0e6a5-127">Nome</span><span class="sxs-lookup"><span data-stu-id="0e6a5-127">Name</span></span>       | <span data-ttu-id="0e6a5-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="0e6a5-128">Type</span></span> | <span data-ttu-id="0e6a5-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="0e6a5-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0e6a5-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="0e6a5-130">Authorization</span></span>  | <span data-ttu-id="0e6a5-131">string</span><span class="sxs-lookup"><span data-stu-id="0e6a5-131">string</span></span>  | <span data-ttu-id="0e6a5-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0e6a5-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0e6a5-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0e6a5-134">Request body</span></span>
<span data-ttu-id="0e6a5-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0e6a5-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0e6a5-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e6a5-136">Response</span></span>
<span data-ttu-id="0e6a5-137">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0e6a5-137">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e6a5-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0e6a5-138">Example</span></span>
#### <a name="request"></a><span data-ttu-id="0e6a5-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0e6a5-139">Request</span></span>
<span data-ttu-id="0e6a5-140">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0e6a5-140">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_members"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/members
```

#### <a name="response"></a><span data-ttu-id="0e6a5-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e6a5-141">Response</span></span>
<span data-ttu-id="0e6a5-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0e6a5-142">The following is an example of the response.</span></span>
><span data-ttu-id="0e6a5-143">**Observação:** no objeto response mostrado aqui pode ser reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0e6a5-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="0e6a5-144">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0e6a5-144">All the properties will be returned from an actual call.</span></span>
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
  "description": "List group members",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
