---
title: Listar fotos
description: Recuperar uma lista dos objetos profilePhoto.
author: dkershaw10
ms.openlocfilehash: 2597d532d28614bb595ffe44aa6705187619aa44
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27315817"
---
# <a name="list-photos"></a><span data-ttu-id="dfef7-103">Listar fotos</span><span class="sxs-lookup"><span data-stu-id="dfef7-103">List photos</span></span>

> <span data-ttu-id="dfef7-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="dfef7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dfef7-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="dfef7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dfef7-106">Recuperar uma lista dos objetos [profilePhoto](../resources/profilephoto.md).</span><span class="sxs-lookup"><span data-stu-id="dfef7-106">Retrieve a list of [profilePhoto](../resources/profilephoto.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="dfef7-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="dfef7-107">Permissions</span></span>
<span data-ttu-id="dfef7-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dfef7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dfef7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dfef7-110">Permission type</span></span>      | <span data-ttu-id="dfef7-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dfef7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dfef7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dfef7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="dfef7-113">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dfef7-113">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="dfef7-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dfef7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dfef7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dfef7-115">Not supported.</span></span>    |
|<span data-ttu-id="dfef7-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dfef7-116">Application</span></span> | <span data-ttu-id="dfef7-117">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dfef7-117">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dfef7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dfef7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/photos
GET /users/{id | userPrincipalName}/joinedGroups/{id}/photos
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dfef7-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="dfef7-119">Optional query parameters</span></span>
<span data-ttu-id="dfef7-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="dfef7-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dfef7-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dfef7-121">Request headers</span></span>
| <span data-ttu-id="dfef7-122">Nome</span><span class="sxs-lookup"><span data-stu-id="dfef7-122">Name</span></span>       | <span data-ttu-id="dfef7-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="dfef7-123">Type</span></span> | <span data-ttu-id="dfef7-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="dfef7-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="dfef7-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="dfef7-125">Authorization</span></span>  | <span data-ttu-id="dfef7-126">string</span><span class="sxs-lookup"><span data-stu-id="dfef7-126">string</span></span>  | <span data-ttu-id="dfef7-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dfef7-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dfef7-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dfef7-129">Request body</span></span>
<span data-ttu-id="dfef7-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dfef7-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dfef7-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="dfef7-131">Response</span></span>
<span data-ttu-id="dfef7-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [profilePhoto](../resources/profilephoto.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dfef7-132">If successful, this method returns a `200 OK` response code and collection of [profilePhoto](../resources/profilephoto.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dfef7-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dfef7-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="dfef7-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dfef7-134">Request</span></span>
<span data-ttu-id="dfef7-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="dfef7-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_photos"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/photos
```

#### <a name="response"></a><span data-ttu-id="dfef7-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="dfef7-136">Response</span></span>
<span data-ttu-id="dfef7-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="dfef7-137">The following is an example of the response.</span></span>
><span data-ttu-id="dfef7-138">**Observação:** no objeto response mostrado aqui pode ser reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="dfef7-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="dfef7-139">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dfef7-139">All the properties will be returned from an actual call.</span></span>
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