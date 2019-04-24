---
title: Grupo de lista memberOf
description: Obter grupos e unidades administrativas dos quais o grupo é membro direto.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: ecf127e7cc4af4aada3d75ef6415a242b0a9411b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32502107"
---
# <a name="list-group-memberof"></a><span data-ttu-id="7492c-103">Grupo de lista memberOf</span><span class="sxs-lookup"><span data-stu-id="7492c-103">List group memberOf</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7492c-104">Obter grupos e unidades administrativas dos quais o grupo é membro direto.</span><span class="sxs-lookup"><span data-stu-id="7492c-104">Get groups and administrative units that the group is a direct member of.</span></span>

<span data-ttu-id="7492c-105">Essa operação não é transitiva.</span><span class="sxs-lookup"><span data-stu-id="7492c-105">This operation is not transitive.</span></span> <span data-ttu-id="7492c-106">Ao contrário de obter os grupos do Office 365 de um usuário, isso retorna todos os tipos de grupos, não apenas grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="7492c-106">Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 Groups.</span></span> 

## <a name="permissions"></a><span data-ttu-id="7492c-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="7492c-107">Permissions</span></span>

<span data-ttu-id="7492c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7492c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7492c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7492c-110">Permission type</span></span>      | <span data-ttu-id="7492c-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7492c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7492c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7492c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7492c-113">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7492c-113">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7492c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7492c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7492c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7492c-115">Not supported.</span></span>    |
|<span data-ttu-id="7492c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7492c-116">Application</span></span> | <span data-ttu-id="7492c-117">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7492c-117">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7492c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7492c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7492c-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7492c-119">Optional query parameters</span></span>
<span data-ttu-id="7492c-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7492c-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7492c-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7492c-121">Request headers</span></span>
| <span data-ttu-id="7492c-122">Nome</span><span class="sxs-lookup"><span data-stu-id="7492c-122">Name</span></span>       | <span data-ttu-id="7492c-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="7492c-123">Type</span></span> | <span data-ttu-id="7492c-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="7492c-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7492c-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="7492c-125">Authorization</span></span>  | <span data-ttu-id="7492c-126">string</span><span class="sxs-lookup"><span data-stu-id="7492c-126">string</span></span>  | <span data-ttu-id="7492c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7492c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7492c-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7492c-129">Request body</span></span>
<span data-ttu-id="7492c-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7492c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7492c-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="7492c-131">Response</span></span>
<span data-ttu-id="7492c-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7492c-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7492c-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7492c-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="7492c-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7492c-134">Request</span></span>

<span data-ttu-id="7492c-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7492c-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_memberof"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/memberOf
```

### <a name="response"></a><span data-ttu-id="7492c-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="7492c-136">Response</span></span>

<span data-ttu-id="7492c-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7492c-137">The following is an example of the response.</span></span>
><span data-ttu-id="7492c-138">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7492c-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7492c-139">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7492c-139">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
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
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-list-memberof.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
