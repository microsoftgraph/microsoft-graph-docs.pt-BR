---
title: Listar membros
description: Recupera uma lista dos usuários atribuídos à função de diretório.  Somente usuários podem ser atribuídos a uma função de diretório.
author: lleonard-msft
ms.openlocfilehash: 8bd0f67d6ca565dac6dfae501f5bc5c829f4db3b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359098"
---
# <a name="list-members"></a><span data-ttu-id="9912d-104">Listar membros</span><span class="sxs-lookup"><span data-stu-id="9912d-104">List members</span></span>

> <span data-ttu-id="9912d-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9912d-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9912d-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9912d-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9912d-p103">Recupera uma lista dos usuários atribuídos à função de diretório.  Somente usuários podem ser atribuídos a uma função de diretório.</span><span class="sxs-lookup"><span data-stu-id="9912d-p103">Retrieve a list of the users that are assigned to the directory role.  Only users can be assigned to a directory role.</span></span>
## <a name="permissions"></a><span data-ttu-id="9912d-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="9912d-109">Permissions</span></span>
<span data-ttu-id="9912d-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9912d-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="9912d-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9912d-112">Permission type</span></span>      | <span data-ttu-id="9912d-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9912d-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9912d-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9912d-114">Delegated (work or school account)</span></span> | <span data-ttu-id="9912d-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9912d-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9912d-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9912d-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9912d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9912d-117">Not supported.</span></span>    |
|<span data-ttu-id="9912d-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9912d-118">Application</span></span> | <span data-ttu-id="9912d-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9912d-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9912d-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9912d-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9912d-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9912d-121">Optional query parameters</span></span>
<span data-ttu-id="9912d-122">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9912d-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="9912d-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9912d-123">Request headers</span></span>
| <span data-ttu-id="9912d-124">Nome</span><span class="sxs-lookup"><span data-stu-id="9912d-124">Name</span></span>       | <span data-ttu-id="9912d-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="9912d-125">Type</span></span> | <span data-ttu-id="9912d-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="9912d-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9912d-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="9912d-127">Authorization</span></span>  | <span data-ttu-id="9912d-128">string</span><span class="sxs-lookup"><span data-stu-id="9912d-128">string</span></span>  | <span data-ttu-id="9912d-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9912d-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9912d-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9912d-131">Request body</span></span>
<span data-ttu-id="9912d-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9912d-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9912d-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="9912d-133">Response</span></span>

<span data-ttu-id="9912d-134">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9912d-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9912d-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9912d-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9912d-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9912d-136">Request</span></span>
<span data-ttu-id="9912d-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9912d-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/beta/directoryRoles/{id}/members
```
##### <a name="response"></a><span data-ttu-id="9912d-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="9912d-138">Response</span></span>
<span data-ttu-id="9912d-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9912d-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->