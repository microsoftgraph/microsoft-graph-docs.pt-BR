---
title: List schemaExtensions
description: 'Obtenha uma lista de objetos schemaExtension criados por qualquer aplicativo que você possui no locatário atual (que pode ser '
localization_priority: Normal
author: dkershaw10
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 5daf20b101a0b73950df13f9e1e6c6b8a2d24d86
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453741"
---
# <a name="list-schemaextensions"></a><span data-ttu-id="6ea88-103">List schemaExtensions</span><span class="sxs-lookup"><span data-stu-id="6ea88-103">List schemaExtensions</span></span>

<span data-ttu-id="6ea88-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6ea88-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ea88-105">Obtenha uma lista de objetos [schemaExtension](../resources/schemaextension.md) criados por qualquer aplicativo que você possui no locatário atual (que pode ser **indevelopment**, **disponível**ou **preterido**) e todas as outras extensões de esquema pertencentes a outros aplicativos marcados como **disponíveis**.</span><span class="sxs-lookup"><span data-stu-id="6ea88-105">Get a list of [schemaExtension](../resources/schemaextension.md) objects created by any apps you own in the current tenant (that can be **InDevelopment**, **Available**, or **Deprecated**), and all other schema extensions owned by other apps that are marked as **Available**.</span></span> 

## <a name="permissions"></a><span data-ttu-id="6ea88-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6ea88-106">Permissions</span></span>
<span data-ttu-id="6ea88-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ea88-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="6ea88-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6ea88-109">Permission type</span></span>      | <span data-ttu-id="6ea88-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6ea88-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6ea88-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6ea88-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6ea88-112">Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6ea88-112">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6ea88-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6ea88-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6ea88-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6ea88-114">Not supported.</span></span>    |
|<span data-ttu-id="6ea88-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6ea88-115">Application</span></span> | <span data-ttu-id="6ea88-116">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="6ea88-116">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6ea88-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6ea88-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /schemaExtensions
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6ea88-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6ea88-118">Optional query parameters</span></span>
<span data-ttu-id="6ea88-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6ea88-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6ea88-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6ea88-120">Request headers</span></span>
| <span data-ttu-id="6ea88-121">Nome</span><span class="sxs-lookup"><span data-stu-id="6ea88-121">Name</span></span>      |<span data-ttu-id="6ea88-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="6ea88-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6ea88-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6ea88-123">Authorization</span></span>  | <span data-ttu-id="6ea88-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6ea88-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6ea88-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6ea88-126">Content-Type</span></span>   | <span data-ttu-id="6ea88-127">application/json</span><span class="sxs-lookup"><span data-stu-id="6ea88-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="6ea88-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6ea88-128">Request body</span></span>
<span data-ttu-id="6ea88-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6ea88-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6ea88-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="6ea88-130">Response</span></span>

<span data-ttu-id="6ea88-131">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [schemaExtension](../resources/schemaextension.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6ea88-131">If successful, this method returns a `200 OK` response code and collection of [schemaExtension](../resources/schemaextension.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6ea88-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6ea88-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6ea88-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6ea88-133">Request</span></span>
<span data-ttu-id="6ea88-134">O exemplo a seguir mostra como procurar entre todas as extensões acessíveis para uma específica filtrando sua **ID**exclusiva.</span><span class="sxs-lookup"><span data-stu-id="6ea88-134">The following example shows how to look among all the accessible extensions for a specific one by filtering on its unique **id**.</span></span> 

# <a name="http"></a>[<span data-ttu-id="6ea88-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="6ea88-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_schemaextensions"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/schemaExtensions?$filter=id%20eq%20'graphlearn_test'
```
# <a name="c"></a>[<span data-ttu-id="6ea88-136">C#</span><span class="sxs-lookup"><span data-stu-id="6ea88-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-schemaextensions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6ea88-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6ea88-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-schemaextensions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6ea88-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6ea88-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-schemaextensions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6ea88-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="6ea88-139">Response</span></span>
<span data-ttu-id="6ea88-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6ea88-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 274

{
  "value": [
    {
      "id":"graphlearn_test",
      "description": "Yet another test schema",
      "targetTypes": [
          "User", "Group"
      ],
      "status": "InDevelopment",
      "owner": "24d3b144-21ae-4080-943f-7067b395b913",
      "properties": [
          {
              "name": "testName",
              "type": "String"
          }
      ]
    }
  ]
}
```

## <a name="see-also"></a><span data-ttu-id="6ea88-143">Confira também</span><span class="sxs-lookup"><span data-stu-id="6ea88-143">See also</span></span>

- [<span data-ttu-id="6ea88-144">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="6ea88-144">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="6ea88-145">Adicionar dados personalizados a grupos usando as extensões do esquema</span><span class="sxs-lookup"><span data-stu-id="6ea88-145">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List schemaExtensions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
