---
title: Listar taughtClasses
description: Obter os recursos educationClass da propriedade de navegação de classes ensinadas.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: a82e647f8c2db6859142c5de5cba619371248add
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2021
ms.locfileid: "52475420"
---
# <a name="list-taughtclasses"></a><span data-ttu-id="42cff-103">Listar taughtClasses</span><span class="sxs-lookup"><span data-stu-id="42cff-103">List taughtClasses</span></span>

<span data-ttu-id="42cff-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42cff-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="42cff-105">Obter os [recursos educationClass](../resources/educationclass.md) pertencentes a um [educationUser](../resources/educationuser.md).</span><span class="sxs-lookup"><span data-stu-id="42cff-105">Get the [educationClass](../resources/educationclass.md) resources owned by an [educationUser](../resources/educationuser.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="42cff-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="42cff-106">Permissions</span></span>

<span data-ttu-id="42cff-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42cff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="42cff-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="42cff-109">Permission type</span></span>                        | <span data-ttu-id="42cff-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="42cff-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="42cff-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="42cff-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="42cff-112">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="42cff-112">EduRoster.ReadBasic</span></span>                         |
| <span data-ttu-id="42cff-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="42cff-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42cff-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="42cff-114">Not supported</span></span>                               |
| <span data-ttu-id="42cff-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="42cff-115">Application</span></span>                            | <span data-ttu-id="42cff-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42cff-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="42cff-117">Observe que, se o token delegado for usado, os usuários só poderão ver informações sobre suas próprias classes.</span><span class="sxs-lookup"><span data-stu-id="42cff-117">Note that if the delegated token is used, users can only see information about their own classes.</span></span>

## <a name="http-request"></a><span data-ttu-id="42cff-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="42cff-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
GET /education/me/taughtClasses
GET /education/users/{educationUserId}/taughtClasses
```

## <a name="optional-query-parameters"></a><span data-ttu-id="42cff-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="42cff-119">Optional query parameters</span></span>

<span data-ttu-id="42cff-120">Use a opção de consulta OData `$orderby` para classificar grupos em uma organização pelos valores **displayName**, conforme exibido no exemplo a seguir:</span><span class="sxs-lookup"><span data-stu-id="42cff-120">You can use the OData query option `$orderby` to sort groups in an organization by the **displayName** values, as shown in the following example:</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/v1.0/groups?$orderby=displayName
```

<span data-ttu-id="42cff-121">Você também pode usar os `$filter` parâmetros , `$count` e consulta para limitar a `$search` resposta.</span><span class="sxs-lookup"><span data-stu-id="42cff-121">You can also use the `$filter`, `$count` and `$search` query parameters to limit the response.</span></span>

<span data-ttu-id="42cff-122">Quando itens são adicionados ou atualizados para este recurso, eles são indexados especialmente para uso com os `$count` e `$search` parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="42cff-122">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="42cff-123">Pode haver um pequeno atraso entre quando um item é adicionado ou atualizado e quando está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="42cff-123">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

<span data-ttu-id="42cff-124">Para obter mais informações sobre as opções de consulta OData, veja [ Parâmetros de consulta OData ](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="42cff-124">For more information on OData query options, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="42cff-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="42cff-125">Request headers</span></span>

| <span data-ttu-id="42cff-126">Nome</span><span class="sxs-lookup"><span data-stu-id="42cff-126">Name</span></span>          | <span data-ttu-id="42cff-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="42cff-127">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="42cff-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="42cff-128">Authorization</span></span> | <span data-ttu-id="42cff-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="42cff-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="42cff-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="42cff-131">Request body</span></span>

<span data-ttu-id="42cff-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="42cff-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="42cff-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="42cff-133">Response</span></span>

<span data-ttu-id="42cff-134">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [educationClass](../resources/educationclass.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="42cff-134">If successful, this method returns a `200 OK` response code and a collection of [educationClass](../resources/educationclass.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="42cff-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="42cff-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="42cff-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="42cff-136">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="42cff-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="42cff-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_educationclass"
}
-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/classes/{educationClassId}/members/{educationUserId}/taughtClasses
```
# <a name="c"></a>[<span data-ttu-id="42cff-138">C#</span><span class="sxs-lookup"><span data-stu-id="42cff-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-educationclass-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="42cff-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="42cff-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-educationclass-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="42cff-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="42cff-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-educationclass-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="42cff-141">Java</span><span class="sxs-lookup"><span data-stu-id="42cff-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-educationclass-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="42cff-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="42cff-142">Response</span></span>

> <span data-ttu-id="42cff-143">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="42cff-143">**Note:** The response object shown here might be shortened for readability.</span></span>

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
