---
title: Listar classes
description: 'Recupere uma lista de objetos de classe. Se o token delegado for usado, os membros só poderão ver informações sobre suas próprias aulas. '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 1f8cc6a1dbda0f86e808d72bfc91339af58afa33
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966934"
---
# <a name="list-classes"></a><span data-ttu-id="c54bb-104">Listar classes</span><span class="sxs-lookup"><span data-stu-id="c54bb-104">List classes</span></span>

<span data-ttu-id="c54bb-105">Recupere uma lista de objetos de classe.</span><span class="sxs-lookup"><span data-stu-id="c54bb-105">Retrieve a list of class objects.</span></span> <span data-ttu-id="c54bb-106">Se o token delegado for usado, os membros só poderão ver informações sobre suas próprias aulas.</span><span class="sxs-lookup"><span data-stu-id="c54bb-106">Note that if the delegated token is used, members can only see information about their own classes.</span></span> 

<!-- Please verify the revision to the delegated token text. -->

## <a name="permissions"></a><span data-ttu-id="c54bb-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="c54bb-107">Permissions</span></span>
<span data-ttu-id="c54bb-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c54bb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c54bb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c54bb-110">Permission type</span></span>      | <span data-ttu-id="c54bb-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c54bb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c54bb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c54bb-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="c54bb-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="c54bb-113">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="c54bb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c54bb-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="c54bb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c54bb-115">Not supported.</span></span>  |
|<span data-ttu-id="c54bb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c54bb-116">Application</span></span> | <span data-ttu-id="c54bb-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c54bb-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="c54bb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c54bb-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me/classes
GET /education/users/{id}/classes
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c54bb-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c54bb-119">Optional query parameters</span></span>
<span data-ttu-id="c54bb-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c54bb-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c54bb-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c54bb-121">Request headers</span></span>
| <span data-ttu-id="c54bb-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c54bb-122">Header</span></span>       | <span data-ttu-id="c54bb-123">Valor</span><span class="sxs-lookup"><span data-stu-id="c54bb-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c54bb-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="c54bb-124">Authorization</span></span>  | <span data-ttu-id="c54bb-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c54bb-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c54bb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c54bb-127">Request body</span></span>
<span data-ttu-id="c54bb-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c54bb-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c54bb-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c54bb-129">Response</span></span>
<span data-ttu-id="c54bb-130">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [educationClass](../resources/educationclass.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c54bb-130">If successful, this method returns a `200 OK` response code and a collection of [educationClass](../resources/educationclass.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c54bb-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c54bb-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c54bb-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c54bb-132">Request</span></span>
<span data-ttu-id="c54bb-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c54bb-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_classes"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/me/classes
```
##### <a name="response"></a><span data-ttu-id="c54bb-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="c54bb-134">Response</span></span>
<span data-ttu-id="c54bb-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c54bb-135">The following is an example of the response.</span></span> 

><span data-ttu-id="c54bb-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c54bb-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 277

{
  "value": [
    {
      "id": "11019",
      "description": "Health Level 1",
      "classCode": "Health 501",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "displayName": "Health 1",
      "externalId": "11019",
      "externalName": "Health Level 1",
      "externalSource": "sis",
      "mailNickname": "fineartschool.net"
    } 
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List classes",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
