---
title: Listar fotos
description: Recuperar uma lista dos objetos profilePhoto.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 01fd069173fff1a7a6868f1596326fcb44d77fb7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932270"
---
# <a name="list-photos"></a><span data-ttu-id="4be8e-103">Listar fotos</span><span class="sxs-lookup"><span data-stu-id="4be8e-103">List photos</span></span>
<span data-ttu-id="4be8e-104">Recuperar uma lista dos objetos [profilePhoto](../resources/profilephoto.md).</span><span class="sxs-lookup"><span data-stu-id="4be8e-104">Retrieve a list of [profilePhoto](../resources/profilephoto.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="4be8e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="4be8e-105">Permissions</span></span>
<span data-ttu-id="4be8e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4be8e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4be8e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4be8e-108">Permission type</span></span>      | <span data-ttu-id="4be8e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4be8e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4be8e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4be8e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4be8e-111">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4be8e-111">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span> |
|<span data-ttu-id="4be8e-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4be8e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4be8e-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4be8e-113">Not supported.</span></span>    |
|<span data-ttu-id="4be8e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4be8e-114">Application</span></span> | <span data-ttu-id="4be8e-115">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4be8e-115">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4be8e-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4be8e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/photos
GET /users/{id | userPrincipalName}/joinedGroups/{id}/photos
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4be8e-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4be8e-117">Optional query parameters</span></span>
<span data-ttu-id="4be8e-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4be8e-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4be8e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4be8e-119">Request headers</span></span>
| <span data-ttu-id="4be8e-120">Nome</span><span class="sxs-lookup"><span data-stu-id="4be8e-120">Name</span></span>       | <span data-ttu-id="4be8e-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="4be8e-121">Type</span></span> | <span data-ttu-id="4be8e-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="4be8e-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4be8e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4be8e-123">Authorization</span></span>  | <span data-ttu-id="4be8e-124">string</span><span class="sxs-lookup"><span data-stu-id="4be8e-124">string</span></span>  | <span data-ttu-id="4be8e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4be8e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4be8e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4be8e-127">Request body</span></span>
<span data-ttu-id="4be8e-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4be8e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4be8e-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="4be8e-129">Response</span></span>
<span data-ttu-id="4be8e-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [profilePhoto](../resources/profilephoto.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4be8e-130">If successful, this method returns a `200 OK` response code and collection of [profilePhoto](../resources/profilephoto.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4be8e-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4be8e-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="4be8e-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4be8e-132">Request</span></span>
<span data-ttu-id="4be8e-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4be8e-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_photos"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/photos
```

#### <a name="response"></a><span data-ttu-id="4be8e-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="4be8e-134">Response</span></span>
<span data-ttu-id="4be8e-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4be8e-135">The following is an example of the response.</span></span>
><span data-ttu-id="4be8e-136">**Observação:** no objeto response mostrado aqui pode ser reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4be8e-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4be8e-137">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4be8e-137">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.profilePhoto",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 94

{
  "value": [
    {
      "height": 99,
      "width": 99,
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List photos",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
