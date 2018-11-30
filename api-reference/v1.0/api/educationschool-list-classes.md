---
title: Listar educationClasses
description: Recupera uma lista de classes de propriedade de uma escola.
ms.openlocfilehash: de98692f13c280b1e5cb4b66d17335466bfe7a57
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006672"
---
# <a name="list-educationclasses"></a><span data-ttu-id="6e78f-103">Listar educationClasses</span><span class="sxs-lookup"><span data-stu-id="6e78f-103">List educationClasses</span></span>

<span data-ttu-id="6e78f-104">Recupera uma lista de classes de propriedade de uma escola.</span><span class="sxs-lookup"><span data-stu-id="6e78f-104">Retrieve a list of classes owned by a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="6e78f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="6e78f-105">Permissions</span></span>
<span data-ttu-id="6e78f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e78f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e78f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6e78f-108">Permission type</span></span>      | <span data-ttu-id="6e78f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6e78f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6e78f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6e78f-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="6e78f-111">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="6e78f-111">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="6e78f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6e78f-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="6e78f-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6e78f-113">Not supported.</span></span>  |
|<span data-ttu-id="6e78f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6e78f-114">Application</span></span> | <span data-ttu-id="6e78f-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e78f-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="6e78f-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6e78f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/schools/{id}/classes
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6e78f-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6e78f-117">Optional query parameters</span></span>
<span data-ttu-id="6e78f-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6e78f-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6e78f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6e78f-119">Request headers</span></span>
| <span data-ttu-id="6e78f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6e78f-120">Header</span></span>       | <span data-ttu-id="6e78f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6e78f-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6e78f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6e78f-122">Authorization</span></span>  | <span data-ttu-id="6e78f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6e78f-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6e78f-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6e78f-125">Request body</span></span>
<span data-ttu-id="6e78f-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6e78f-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="6e78f-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e78f-127">Response</span></span>
<span data-ttu-id="6e78f-128">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [educationClass](../resources/educationclass.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6e78f-128">If successful, this method returns a `200 OK` response code and a collection of [educationClass](../resources/educationclass.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6e78f-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6e78f-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6e78f-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6e78f-130">Request</span></span>
<span data-ttu-id="6e78f-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6e78f-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_classes"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/schools/{school-id}/classes
```
##### <a name="response"></a><span data-ttu-id="6e78f-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e78f-132">Response</span></span>
<span data-ttu-id="6e78f-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6e78f-133">The following is an example of the response.</span></span> 

><span data-ttu-id="6e78f-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6e78f-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
