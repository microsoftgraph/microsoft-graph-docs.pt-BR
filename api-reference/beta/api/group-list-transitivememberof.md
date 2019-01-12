---
title: Membro transitivo do grupo de lista
description: Obtenha grupos e unidades administrativas que o grupo é um membro de.  Essa operação é transitiva e também incluirá todos os grupos que este grupos é um membro aninhado do. Diferentemente obtendo Office 365 grupos de um usuário, isto retorna todos os tipos de grupos, não apenas a grupos do Office 365.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: ec03ca6fce354f2a0b81cf0f81bf3061db504365
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921665"
---
# <a name="list-group-transitive-memberof"></a><span data-ttu-id="d58c6-105">Membro transitivo do grupo de lista</span><span class="sxs-lookup"><span data-stu-id="d58c6-105">List group transitive memberOf</span></span>

> <span data-ttu-id="d58c6-106">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d58c6-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d58c6-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d58c6-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d58c6-108">Obtenha grupos e unidades administrativas que o grupo é um membro de.</span><span class="sxs-lookup"><span data-stu-id="d58c6-108">Get groups and administrative units that the group is a member of.</span></span>  <span data-ttu-id="d58c6-109">Essa operação é transitiva e também incluirá todos os grupos que este grupos é um membro aninhado do.</span><span class="sxs-lookup"><span data-stu-id="d58c6-109">This operation is transitive and will also include all groups that this groups is a nested member of.</span></span> <span data-ttu-id="d58c6-110">Diferentemente obtendo Office 365 grupos de um usuário, isto retorna todos os tipos de grupos, não apenas a grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="d58c6-110">Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 Groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="d58c6-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="d58c6-111">Permissions</span></span>

<span data-ttu-id="d58c6-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d58c6-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d58c6-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d58c6-114">Permission type</span></span>      | <span data-ttu-id="d58c6-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d58c6-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d58c6-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d58c6-116">Delegated (work or school account)</span></span> | <span data-ttu-id="d58c6-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d58c6-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d58c6-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d58c6-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d58c6-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d58c6-119">Not supported.</span></span>    |
|<span data-ttu-id="d58c6-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d58c6-120">Application</span></span> | <span data-ttu-id="d58c6-121">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d58c6-121">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d58c6-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d58c6-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d58c6-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d58c6-123">Optional query parameters</span></span>
<span data-ttu-id="d58c6-124">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d58c6-124">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d58c6-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d58c6-125">Request headers</span></span>
| <span data-ttu-id="d58c6-126">Nome</span><span class="sxs-lookup"><span data-stu-id="d58c6-126">Name</span></span>       | <span data-ttu-id="d58c6-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="d58c6-127">Type</span></span> | <span data-ttu-id="d58c6-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="d58c6-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d58c6-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="d58c6-129">Authorization</span></span>  | <span data-ttu-id="d58c6-130">string</span><span class="sxs-lookup"><span data-stu-id="d58c6-130">string</span></span>  | <span data-ttu-id="d58c6-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d58c6-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d58c6-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d58c6-133">Request body</span></span>
<span data-ttu-id="d58c6-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d58c6-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d58c6-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="d58c6-135">Response</span></span>
<span data-ttu-id="d58c6-136">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d58c6-136">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d58c6-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d58c6-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="d58c6-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d58c6-138">Request</span></span>
<span data-ttu-id="d58c6-139">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d58c6-139">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_transitivememberof"
}-->

```http
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMemberOf
```

### <a name="response"></a><span data-ttu-id="d58c6-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="d58c6-140">Response</span></span>

<span data-ttu-id="d58c6-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d58c6-141">The following is an example of the response.</span></span>
><span data-ttu-id="d58c6-142">**Observação:** no objeto response mostrado aqui pode ser reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d58c6-142">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d58c6-143">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d58c6-143">All the properties will be returned from an actual call.</span></span>
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
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All users at the company",
      "displayName": "All Users",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true,
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List group transitive memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
