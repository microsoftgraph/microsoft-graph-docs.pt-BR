---
title: Listar classes de uma educationSchool
description: Recupera uma lista de classes de propriedade de uma escola.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: cbd644e5994f8039a29c16f0463445d92500a865
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232029"
---
# <a name="list-classes-of-an-educationschool"></a><span data-ttu-id="8d240-103">Listar classes de uma educationSchool</span><span class="sxs-lookup"><span data-stu-id="8d240-103">List classes of an educationSchool</span></span>

<span data-ttu-id="8d240-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d240-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8d240-105">Obter os [recursos educationClass](../resources/educationclass.md) pertencentes a uma [educationSchool](../resources/educationschool.md).</span><span class="sxs-lookup"><span data-stu-id="8d240-105">Get the [educationClass](../resources/educationclass.md) resources owned by an [educationSchool](../resources/educationschool.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8d240-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8d240-106">Permissions</span></span>

<span data-ttu-id="8d240-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d240-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8d240-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8d240-109">Permission type</span></span>                        | <span data-ttu-id="8d240-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8d240-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="8d240-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8d240-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8d240-112">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="8d240-112">EduRoster.ReadBasic</span></span>                         |
| <span data-ttu-id="8d240-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8d240-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d240-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8d240-114">Not supported.</span></span>                              |
| <span data-ttu-id="8d240-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8d240-115">Application</span></span>                            | <span data-ttu-id="8d240-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d240-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8d240-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8d240-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/schools/{educationSchoolId}/classes
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8d240-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8d240-118">Optional query parameters</span></span>

<span data-ttu-id="8d240-119">Use a opção de consulta OData `$orderby` para classificar grupos em uma organização pelos valores **displayName**, conforme exibido no exemplo a seguir:</span><span class="sxs-lookup"><span data-stu-id="8d240-119">You can use the OData query option `$orderby` to sort groups in an organization by the **displayName** values, as shown in the following example:</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/v1.0/groups?$orderby=displayName
```

<span data-ttu-id="8d240-120">Você também pode usar os `$filter` parâmetros , `$count` e consulta para limitar a `$search` resposta.</span><span class="sxs-lookup"><span data-stu-id="8d240-120">You can also use the `$filter`, `$count` and `$search` query parameters to limit the response.</span></span>

<span data-ttu-id="8d240-121">Quando itens são adicionados ou atualizados para este recurso, eles são indexados especialmente para uso com os `$count` e `$search` parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="8d240-121">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="8d240-122">Pode haver um pequeno atraso entre quando um item é adicionado ou atualizado e quando está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="8d240-122">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

<span data-ttu-id="8d240-123">Para obter mais informações sobre as opções de consulta OData, veja [ Parâmetros de consulta OData ](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="8d240-123">For more information on OData query options, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="8d240-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8d240-124">Request headers</span></span>
| <span data-ttu-id="8d240-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8d240-125">Header</span></span>       | <span data-ttu-id="8d240-126">Valor</span><span class="sxs-lookup"><span data-stu-id="8d240-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8d240-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="8d240-127">Authorization</span></span>  | <span data-ttu-id="8d240-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8d240-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8d240-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8d240-130">Request body</span></span>
<span data-ttu-id="8d240-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8d240-131">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="8d240-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d240-132">Response</span></span>
<span data-ttu-id="8d240-133">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [educationClass](../resources/educationclass.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8d240-133">If successful, this method returns a `200 OK` response code and a collection of [educationClass](../resources/educationclass.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8d240-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8d240-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8d240-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8d240-135">Request</span></span>
<span data-ttu-id="8d240-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8d240-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8d240-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="8d240-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_classes_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/schools/{school-id}/classes
```
# <a name="c"></a>[<span data-ttu-id="8d240-138">C#</span><span class="sxs-lookup"><span data-stu-id="8d240-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-classes-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8d240-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8d240-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-classes-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8d240-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8d240-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-classes-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8d240-141">Java</span><span class="sxs-lookup"><span data-stu-id="8d240-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-classes-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8d240-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d240-142">Response</span></span>
<span data-ttu-id="8d240-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8d240-143">The following is an example of the response.</span></span> 

><span data-ttu-id="8d240-144">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8d240-144">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "tocPath": "",
  "suppressions": [
  ]
}-->
