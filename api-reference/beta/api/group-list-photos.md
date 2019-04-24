---
title: Listar fotos
description: Recuperar uma lista dos objetos profilePhoto.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 959c25bc9904a8145240f76baaf3271e29e17eef
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32502048"
---
# <a name="list-photos"></a><span data-ttu-id="e61e7-103">Listar fotos</span><span class="sxs-lookup"><span data-stu-id="e61e7-103">List photos</span></span>
<span data-ttu-id="e61e7-104">Recuperar uma lista dos objetos [profilePhoto](../resources/profilephoto.md).</span><span class="sxs-lookup"><span data-stu-id="e61e7-104">Retrieve a list of [profilePhoto](../resources/profilephoto.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="e61e7-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e61e7-105">Permissions</span></span>
<span data-ttu-id="e61e7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e61e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e61e7-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e61e7-108">Permission type</span></span>      | <span data-ttu-id="e61e7-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e61e7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e61e7-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e61e7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e61e7-111">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e61e7-111">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span> |
|<span data-ttu-id="e61e7-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e61e7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e61e7-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e61e7-113">Not supported.</span></span>    |
|<span data-ttu-id="e61e7-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e61e7-114">Application</span></span> | <span data-ttu-id="e61e7-115">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e61e7-115">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e61e7-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e61e7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/photos
GET /users/{id | userPrincipalName}/joinedGroups/{id}/photos
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e61e7-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e61e7-117">Optional query parameters</span></span>
<span data-ttu-id="e61e7-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e61e7-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e61e7-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e61e7-119">Request headers</span></span>
| <span data-ttu-id="e61e7-120">Nome</span><span class="sxs-lookup"><span data-stu-id="e61e7-120">Name</span></span>       | <span data-ttu-id="e61e7-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="e61e7-121">Type</span></span> | <span data-ttu-id="e61e7-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="e61e7-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e61e7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e61e7-123">Authorization</span></span>  | <span data-ttu-id="e61e7-124">string</span><span class="sxs-lookup"><span data-stu-id="e61e7-124">string</span></span>  | <span data-ttu-id="e61e7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e61e7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e61e7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e61e7-127">Request body</span></span>
<span data-ttu-id="e61e7-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e61e7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e61e7-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e61e7-129">Response</span></span>
<span data-ttu-id="e61e7-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [profilePhoto](../resources/profilephoto.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e61e7-130">If successful, this method returns a `200 OK` response code and collection of [profilePhoto](../resources/profilephoto.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e61e7-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e61e7-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="e61e7-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e61e7-132">Request</span></span>
<span data-ttu-id="e61e7-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e61e7-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_photos"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/photos
```

#### <a name="response"></a><span data-ttu-id="e61e7-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="e61e7-134">Response</span></span>
<span data-ttu-id="e61e7-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e61e7-135">The following is an example of the response.</span></span>
><span data-ttu-id="e61e7-136">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e61e7-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e61e7-137">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e61e7-137">All the properties will be returned from an actual call.</span></span>
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
