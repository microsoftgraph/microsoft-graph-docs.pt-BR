---
title: Membro do grupo de lista
description: Obtenha grupos e unidades administrativas que o grupo é um membro direto.
author: dkershaw10
ms.openlocfilehash: fa8977cd128fdb51296b31dac2ee959aea8c80b8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27335928"
---
# <a name="list-group-memberof"></a><span data-ttu-id="9b6bc-103">Membro do grupo de lista</span><span class="sxs-lookup"><span data-stu-id="9b6bc-103">List group memberOf</span></span>

> <span data-ttu-id="9b6bc-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9b6bc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9b6bc-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9b6bc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9b6bc-106">Obtenha grupos e unidades administrativas que o grupo é um membro direto.</span><span class="sxs-lookup"><span data-stu-id="9b6bc-106">Get groups and administrative units that the group is a direct member of.</span></span>

<span data-ttu-id="9b6bc-107">Esta operação não é transitiva.</span><span class="sxs-lookup"><span data-stu-id="9b6bc-107">This operation is not transitive.</span></span> <span data-ttu-id="9b6bc-108">Diferentemente obtendo Office 365 grupos de um usuário, isto retorna todos os tipos de grupos, não apenas a grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="9b6bc-108">Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 Groups.</span></span> 

## <a name="permissions"></a><span data-ttu-id="9b6bc-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="9b6bc-109">Permissions</span></span>

<span data-ttu-id="9b6bc-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b6bc-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b6bc-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9b6bc-112">Permission type</span></span>      | <span data-ttu-id="9b6bc-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9b6bc-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9b6bc-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9b6bc-114">Delegated (work or school account)</span></span> | <span data-ttu-id="9b6bc-115">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9b6bc-115">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9b6bc-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9b6bc-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9b6bc-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9b6bc-117">Not supported.</span></span>    |
|<span data-ttu-id="9b6bc-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9b6bc-118">Application</span></span> | <span data-ttu-id="9b6bc-119">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b6bc-119">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9b6bc-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9b6bc-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9b6bc-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9b6bc-121">Optional query parameters</span></span>
<span data-ttu-id="9b6bc-122">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9b6bc-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9b6bc-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9b6bc-123">Request headers</span></span>
| <span data-ttu-id="9b6bc-124">Nome</span><span class="sxs-lookup"><span data-stu-id="9b6bc-124">Name</span></span>       | <span data-ttu-id="9b6bc-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="9b6bc-125">Type</span></span> | <span data-ttu-id="9b6bc-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b6bc-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9b6bc-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="9b6bc-127">Authorization</span></span>  | <span data-ttu-id="9b6bc-128">string</span><span class="sxs-lookup"><span data-stu-id="9b6bc-128">string</span></span>  | <span data-ttu-id="9b6bc-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9b6bc-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9b6bc-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9b6bc-131">Request body</span></span>
<span data-ttu-id="9b6bc-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9b6bc-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9b6bc-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b6bc-133">Response</span></span>
<span data-ttu-id="9b6bc-134">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9b6bc-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b6bc-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9b6bc-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="9b6bc-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9b6bc-136">Request</span></span>

<span data-ttu-id="9b6bc-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9b6bc-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_memberof"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/memberOf
```

### <a name="response"></a><span data-ttu-id="9b6bc-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b6bc-138">Response</span></span>

<span data-ttu-id="9b6bc-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9b6bc-139">The following is an example of the response.</span></span>
><span data-ttu-id="9b6bc-140">**Observação:** no objeto response mostrado aqui pode ser reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9b6bc-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9b6bc-141">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9b6bc-141">All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->