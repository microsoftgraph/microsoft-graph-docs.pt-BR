---
title: Listar fotos
description: Recuperar uma lista dos objetos profilePhoto.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 959c25bc9904a8145240f76baaf3271e29e17eef
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514394"
---
# <a name="list-photos"></a><span data-ttu-id="d4d86-103">Listar fotos</span><span class="sxs-lookup"><span data-stu-id="d4d86-103">List photos</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4d86-104">Recuperar uma lista dos objetos [profilePhoto](../resources/profilephoto.md).</span><span class="sxs-lookup"><span data-stu-id="d4d86-104">Retrieve a list of [profilePhoto](../resources/profilephoto.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="d4d86-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d4d86-105">Permissions</span></span>
<span data-ttu-id="d4d86-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4d86-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4d86-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d4d86-108">Permission type</span></span>      | <span data-ttu-id="d4d86-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d4d86-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d4d86-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d4d86-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d4d86-111">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4d86-111">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d4d86-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d4d86-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d4d86-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d4d86-113">Not supported.</span></span>    |
|<span data-ttu-id="d4d86-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d4d86-114">Application</span></span> | <span data-ttu-id="d4d86-115">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4d86-115">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d4d86-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d4d86-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/photos
GET /users/{id | userPrincipalName}/joinedGroups/{id}/photos
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d4d86-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d4d86-117">Optional query parameters</span></span>
<span data-ttu-id="d4d86-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d4d86-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d4d86-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d4d86-119">Request headers</span></span>
| <span data-ttu-id="d4d86-120">Nome</span><span class="sxs-lookup"><span data-stu-id="d4d86-120">Name</span></span>       | <span data-ttu-id="d4d86-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="d4d86-121">Type</span></span> | <span data-ttu-id="d4d86-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4d86-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d4d86-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d4d86-123">Authorization</span></span>  | <span data-ttu-id="d4d86-124">string</span><span class="sxs-lookup"><span data-stu-id="d4d86-124">string</span></span>  | <span data-ttu-id="d4d86-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d4d86-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d4d86-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d4d86-127">Request body</span></span>
<span data-ttu-id="d4d86-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d4d86-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d4d86-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4d86-129">Response</span></span>
<span data-ttu-id="d4d86-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [profilePhoto](../resources/profilephoto.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d4d86-130">If successful, this method returns a `200 OK` response code and collection of [profilePhoto](../resources/profilephoto.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4d86-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d4d86-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="d4d86-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d4d86-132">Request</span></span>
<span data-ttu-id="d4d86-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d4d86-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_photos"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/photos
```

#### <a name="response"></a><span data-ttu-id="d4d86-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4d86-134">Response</span></span>
<span data-ttu-id="d4d86-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d4d86-135">The following is an example of the response.</span></span>
><span data-ttu-id="d4d86-136">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d4d86-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d4d86-137">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d4d86-137">All the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List photos",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-list-photos.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
