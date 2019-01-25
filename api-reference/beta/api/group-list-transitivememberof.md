---
title: Membro transitivo do grupo de lista
description: Obtenha grupos e unidades administrativas que o grupo é um membro de.  Essa operação é transitiva e também incluirá todos os grupos que este grupos é um membro aninhado do. Diferentemente obtendo Office 365 grupos de um usuário, isto retorna todos os tipos de grupos, não apenas a grupos do Office 365.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 95d191973a327e6b3e1b0c7e692e0d581744e0ee
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515829"
---
# <a name="list-group-transitive-memberof"></a><span data-ttu-id="7d397-105">Membro transitivo do grupo de lista</span><span class="sxs-lookup"><span data-stu-id="7d397-105">List group transitive memberOf</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d397-106">Obtenha grupos e unidades administrativas que o grupo é um membro de.</span><span class="sxs-lookup"><span data-stu-id="7d397-106">Get groups and administrative units that the group is a member of.</span></span>  <span data-ttu-id="7d397-107">Essa operação é transitiva e também incluirá todos os grupos que este grupos é um membro aninhado do.</span><span class="sxs-lookup"><span data-stu-id="7d397-107">This operation is transitive and will also include all groups that this groups is a nested member of.</span></span> <span data-ttu-id="7d397-108">Diferentemente obtendo Office 365 grupos de um usuário, isto retorna todos os tipos de grupos, não apenas a grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="7d397-108">Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 Groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="7d397-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="7d397-109">Permissions</span></span>

<span data-ttu-id="7d397-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d397-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d397-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7d397-112">Permission type</span></span>      | <span data-ttu-id="7d397-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7d397-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7d397-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7d397-114">Delegated (work or school account)</span></span> | <span data-ttu-id="7d397-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7d397-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7d397-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7d397-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7d397-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7d397-117">Not supported.</span></span>    |
|<span data-ttu-id="7d397-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7d397-118">Application</span></span> | <span data-ttu-id="7d397-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d397-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7d397-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7d397-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7d397-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7d397-121">Optional query parameters</span></span>
<span data-ttu-id="7d397-122">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7d397-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7d397-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7d397-123">Request headers</span></span>
| <span data-ttu-id="7d397-124">Nome</span><span class="sxs-lookup"><span data-stu-id="7d397-124">Name</span></span>       | <span data-ttu-id="7d397-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="7d397-125">Type</span></span> | <span data-ttu-id="7d397-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d397-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7d397-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="7d397-127">Authorization</span></span>  | <span data-ttu-id="7d397-128">string</span><span class="sxs-lookup"><span data-stu-id="7d397-128">string</span></span>  | <span data-ttu-id="7d397-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7d397-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7d397-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7d397-131">Request body</span></span>
<span data-ttu-id="7d397-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7d397-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7d397-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d397-133">Response</span></span>
<span data-ttu-id="7d397-134">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7d397-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d397-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7d397-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="7d397-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7d397-136">Request</span></span>
<span data-ttu-id="7d397-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7d397-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_transitivememberof"
}-->

```http
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMemberOf
```

### <a name="response"></a><span data-ttu-id="7d397-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d397-138">Response</span></span>

<span data-ttu-id="7d397-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7d397-139">The following is an example of the response.</span></span>
><span data-ttu-id="7d397-140">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7d397-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7d397-141">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7d397-141">All the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List group transitive memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-list-transitivememberof.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
