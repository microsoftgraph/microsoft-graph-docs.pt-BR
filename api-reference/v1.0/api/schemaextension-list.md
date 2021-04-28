---
title: List schemaExtensions
description: 'Obter uma lista de objetos schemaExtension criados por todos os aplicativos que você possui no locatário atual (que pode ser '
localization_priority: Normal
author: dkershaw10
ms.prod: extensions
doc_type: apiPageType
ms.openlocfilehash: 32ce5aea57fe4becee644d500cba043460ab825d
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52038954"
---
# <a name="list-schemaextensions"></a><span data-ttu-id="3efc8-103">List schemaExtensions</span><span class="sxs-lookup"><span data-stu-id="3efc8-103">List schemaExtensions</span></span>

<span data-ttu-id="3efc8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3efc8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3efc8-105">Obter uma lista de objetos [schemaExtension](../resources/schemaextension.md) criados por qualquer aplicativo que você possui no locatário atual (que pode ser **InDevelopment**, **Disponível** ou **Preterido**) e todas as outras extensões de esquema pertencentes a outros aplicativos marcados como **Disponíveis**.</span><span class="sxs-lookup"><span data-stu-id="3efc8-105">Get a list of [schemaExtension](../resources/schemaextension.md) objects created by any apps you own in the current tenant (that can be **InDevelopment**, **Available**, or **Deprecated**), and all other schema extensions owned by other apps that are marked as **Available**.</span></span> 

> <span data-ttu-id="3efc8-106">**Observação:** A lista também conterá definições de extensão de esquema (marcadas como `Available` ) criadas por outros desenvolvedores de outros locatários.</span><span class="sxs-lookup"><span data-stu-id="3efc8-106">**Note:** The list will also contain schema extension definitions (marked as `Available`) created by other developers from other tenants.</span></span> <span data-ttu-id="3efc8-107">Isto é diferente de outras APIs que retornam apenas os dados específicos do locatário.</span><span class="sxs-lookup"><span data-stu-id="3efc8-107">This is different from other APIs that only return tenant-specific data.</span></span> <span data-ttu-id="3efc8-108">Os dados de extensão criados com base em definições de extensão de esquema são específicos do locatário e só podem ser acessados por aplicativos explicitamente concedidos permissão.</span><span class="sxs-lookup"><span data-stu-id="3efc8-108">Extension data created based on schema extension definitions is tenant-specific and can only be accessed by apps explicitly granted permission.</span></span> 

## <a name="permissions"></a><span data-ttu-id="3efc8-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="3efc8-109">Permissions</span></span>
<span data-ttu-id="3efc8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3efc8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="3efc8-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3efc8-112">Permission type</span></span>      | <span data-ttu-id="3efc8-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3efc8-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3efc8-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3efc8-114">Delegated (work or school account)</span></span> | <span data-ttu-id="3efc8-115">User.Read, Application.Read.All</span><span class="sxs-lookup"><span data-stu-id="3efc8-115">User.Read, Application.Read.All</span></span>  |
|<span data-ttu-id="3efc8-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3efc8-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3efc8-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3efc8-117">Not supported.</span></span>    |
|<span data-ttu-id="3efc8-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3efc8-118">Application</span></span> | <span data-ttu-id="3efc8-119">Application.Read.All</span><span class="sxs-lookup"><span data-stu-id="3efc8-119">Application.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3efc8-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3efc8-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /schemaExtensions
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3efc8-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3efc8-121">Optional query parameters</span></span>
<span data-ttu-id="3efc8-122">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3efc8-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3efc8-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3efc8-123">Request headers</span></span>
| <span data-ttu-id="3efc8-124">Nome</span><span class="sxs-lookup"><span data-stu-id="3efc8-124">Name</span></span>      |<span data-ttu-id="3efc8-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="3efc8-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3efc8-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="3efc8-126">Authorization</span></span>  | <span data-ttu-id="3efc8-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3efc8-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3efc8-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3efc8-129">Content-Type</span></span>   | <span data-ttu-id="3efc8-130">application/json</span><span class="sxs-lookup"><span data-stu-id="3efc8-130">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="3efc8-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3efc8-131">Request body</span></span>
<span data-ttu-id="3efc8-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3efc8-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3efc8-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="3efc8-133">Response</span></span>

<span data-ttu-id="3efc8-134">Se tiver êxito, este método retornará um código `200 OK` de resposta e uma coleção de objetos [schemaExtension](../resources/schemaextension.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3efc8-134">If successful, this method returns a `200 OK` response code and collection of [schemaExtension](../resources/schemaextension.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3efc8-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3efc8-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3efc8-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3efc8-136">Request</span></span>
<span data-ttu-id="3efc8-137">O exemplo a seguir mostra como procurar entre todas as extensões acessíveis para uma específica, filtrando sua **id exclusiva.**</span><span class="sxs-lookup"><span data-stu-id="3efc8-137">The following example shows how to look among all the accessible extensions for a specific one by filtering on its unique **id**.</span></span> 

# <a name="http"></a>[<span data-ttu-id="3efc8-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="3efc8-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_schemaextensions"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/schemaExtensions?$filter=id%20eq%20'graphlearn_test'
```
# <a name="c"></a>[<span data-ttu-id="3efc8-139">C#</span><span class="sxs-lookup"><span data-stu-id="3efc8-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-schemaextensions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3efc8-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3efc8-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-schemaextensions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3efc8-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3efc8-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-schemaextensions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3efc8-142">Java</span><span class="sxs-lookup"><span data-stu-id="3efc8-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-schemaextensions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3efc8-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="3efc8-143">Response</span></span>
<span data-ttu-id="3efc8-144">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3efc8-144">Here is an example of the response.</span></span> <span data-ttu-id="3efc8-145">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="3efc8-145">Note: The response object shown here might be shortened for readability.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="3efc8-146">Confira também</span><span class="sxs-lookup"><span data-stu-id="3efc8-146">See also</span></span>

- [<span data-ttu-id="3efc8-147">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="3efc8-147">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="3efc8-148">Adicionar dados personalizados a grupos usando as extensões do esquema</span><span class="sxs-lookup"><span data-stu-id="3efc8-148">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List schemaExtensions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
