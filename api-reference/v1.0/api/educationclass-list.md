---
title: Listar educationClasses
description: Obter uma lista dos objetos educationClass e suas propriedades.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: f0841bb6a15bcb8b03819e95540c4c40d99fa57d
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474950"
---
# <a name="list-educationclasses"></a><span data-ttu-id="70682-103">Listar educationClasses</span><span class="sxs-lookup"><span data-stu-id="70682-103">List educationClasses</span></span>

<span data-ttu-id="70682-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="70682-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="70682-105">Obter uma lista dos [objetos educationClass](../resources/educationclass.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="70682-105">Get a list of the [educationClass](../resources/educationclass.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="70682-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="70682-106">Permissions</span></span>

<span data-ttu-id="70682-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70682-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="70682-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="70682-109">Permission type</span></span>                        | <span data-ttu-id="70682-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="70682-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="70682-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="70682-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="70682-112">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="70682-112">EduRoster.ReadBasic</span></span>                         |
| <span data-ttu-id="70682-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="70682-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="70682-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="70682-114">Not supported</span></span>                               |
| <span data-ttu-id="70682-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="70682-115">Application</span></span>                            | <span data-ttu-id="70682-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70682-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="70682-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="70682-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
GET /education/classes
```

## <a name="optional-query-parameters"></a><span data-ttu-id="70682-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="70682-118">Optional query parameters</span></span>

<span data-ttu-id="70682-119">Use a opção de consulta OData `$orderby` para classificar grupos em uma organização pelos valores **displayName**, conforme exibido no exemplo a seguir:</span><span class="sxs-lookup"><span data-stu-id="70682-119">You can use the OData query option `$orderby` to sort groups in an organization by the **displayName** values, as shown in the following example:</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/v1.0/groups?$orderby=displayName
```

<span data-ttu-id="70682-120">Você também pode usar os `$filter` parâmetros , `$count` e consulta para limitar a `$search` resposta.</span><span class="sxs-lookup"><span data-stu-id="70682-120">You can also use the `$filter`, `$count` and `$search` query parameters to limit the response.</span></span> 

<span data-ttu-id="70682-121">Quando itens são adicionados ou atualizados para este recurso, eles são indexados especialmente para uso com os `$count` e `$search` parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="70682-121">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="70682-122">Pode haver um pequeno atraso entre quando um item é adicionado ou atualizado e quando está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="70682-122">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

<span data-ttu-id="70682-123">Para obter mais informações sobre as opções de consulta OData, veja [ Parâmetros de consulta OData ](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="70682-123">For more information on OData query options, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="70682-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="70682-124">Request headers</span></span>

| <span data-ttu-id="70682-125">Nome</span><span class="sxs-lookup"><span data-stu-id="70682-125">Name</span></span>          | <span data-ttu-id="70682-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="70682-126">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="70682-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="70682-127">Authorization</span></span> | <span data-ttu-id="70682-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="70682-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="70682-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="70682-130">Request body</span></span>

<span data-ttu-id="70682-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="70682-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="70682-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="70682-132">Response</span></span>

<span data-ttu-id="70682-133">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [educationClass](../resources/educationclass.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="70682-133">If successful, this method returns a `200 OK` response code and a collection of [educationClass](../resources/educationclass.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="70682-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="70682-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="70682-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="70682-135">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="70682-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="70682-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_educationclass"
}
-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/classes
```
# <a name="c"></a>[<span data-ttu-id="70682-137">C#</span><span class="sxs-lookup"><span data-stu-id="70682-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-educationclass-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="70682-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="70682-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-educationclass-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="70682-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="70682-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-educationclass-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="70682-140">Java</span><span class="sxs-lookup"><span data-stu-id="70682-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-educationclass-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="70682-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="70682-141">Response</span></span>

> <span data-ttu-id="70682-142">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="70682-142">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.educationClass)"
}
-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.educationClass",
      "id": "64ef8ce5-8ce5-64ef-e58c-ef64e58cef64",
      "displayName": "String",
      "mailNickname": "String",
      "description": "String",
      "createdBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "classCode": "String",
      "externalName": "String",
      "externalId": "String",
      "externalSource": "String",
      "externalSourceDetail": "String",
      "grade": "String",
      "term": {
        "@odata.type": "microsoft.graph.educationTerm"
      }
    }
  ]
}
```
