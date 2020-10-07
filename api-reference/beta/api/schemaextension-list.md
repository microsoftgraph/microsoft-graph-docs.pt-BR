---
title: List schemaExtensions
description: 'Obtenha uma lista de objetos schemaExtension criados por qualquer aplicativo que você possui no locatário atual (que pode ser '
localization_priority: Normal
author: dkershaw10
doc_type: apiPageType
ms.prod: extensions
ms.openlocfilehash: ca8986dec23e03763aca1491ed4627fa0b87792b
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/07/2020
ms.locfileid: "48373539"
---
# <a name="list-schemaextensions"></a><span data-ttu-id="7bca4-103">List schemaExtensions</span><span class="sxs-lookup"><span data-stu-id="7bca4-103">List schemaExtensions</span></span>

<span data-ttu-id="7bca4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7bca4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7bca4-105">Obtenha uma lista de objetos [schemaExtension](../resources/schemaextension.md) criados por qualquer aplicativo que você possui no locatário atual (que pode ser **indevelopment**, **disponível**ou **preterido**) e todas as outras extensões de esquema pertencentes a outros aplicativos marcados como **disponíveis**.</span><span class="sxs-lookup"><span data-stu-id="7bca4-105">Get a list of [schemaExtension](../resources/schemaextension.md) objects created by any apps you own in the current tenant (that can be **InDevelopment**, **Available**, or **Deprecated**), and all other schema extensions owned by other apps that are marked as **Available**.</span></span> 

> <span data-ttu-id="7bca4-106">**Observação:** A lista também conterá definições de extensão de esquema (marcadas como `Available` ) criadas por outros desenvolvedores de outros locatários.</span><span class="sxs-lookup"><span data-stu-id="7bca4-106">**Note:** The list will also contain schema extension definitions (marked as `Available`) created by other developers from other tenants.</span></span> <span data-ttu-id="7bca4-107">Isto é diferente de outras APIs que retornam apenas os dados específicos do locatário.</span><span class="sxs-lookup"><span data-stu-id="7bca4-107">This is different from other APIs that only return tenant-specific data.</span></span> <span data-ttu-id="7bca4-108">Os dados de extensão criados com base nas definições de extensão de esquema são específicos do locatário e só podem ser acessados por aplicativos explicitamente concedidos à permissão.</span><span class="sxs-lookup"><span data-stu-id="7bca4-108">Extension data created based on schema extension definitions is tenant-specific and can only be accessed by apps explicitly granted permission.</span></span> 

## <a name="permissions"></a><span data-ttu-id="7bca4-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="7bca4-109">Permissions</span></span>
<span data-ttu-id="7bca4-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7bca4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="7bca4-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7bca4-112">Permission type</span></span>      | <span data-ttu-id="7bca4-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7bca4-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7bca4-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7bca4-114">Delegated (work or school account)</span></span> | <span data-ttu-id="7bca4-115">User. Read, Application. Read. All</span><span class="sxs-lookup"><span data-stu-id="7bca4-115">User.Read, Application.Read.All</span></span>   |
|<span data-ttu-id="7bca4-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7bca4-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7bca4-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7bca4-117">Not supported.</span></span>    |
|<span data-ttu-id="7bca4-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7bca4-118">Application</span></span> | <span data-ttu-id="7bca4-119">Application.Read.All</span><span class="sxs-lookup"><span data-stu-id="7bca4-119">Application.Read.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="7bca4-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7bca4-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /schemaExtensions
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7bca4-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7bca4-121">Optional query parameters</span></span>
<span data-ttu-id="7bca4-122">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7bca4-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7bca4-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7bca4-123">Request headers</span></span>
| <span data-ttu-id="7bca4-124">Nome</span><span class="sxs-lookup"><span data-stu-id="7bca4-124">Name</span></span>      |<span data-ttu-id="7bca4-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="7bca4-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7bca4-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="7bca4-126">Authorization</span></span>  | <span data-ttu-id="7bca4-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7bca4-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7bca4-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7bca4-129">Content-Type</span></span>   | <span data-ttu-id="7bca4-130">application/json</span><span class="sxs-lookup"><span data-stu-id="7bca4-130">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="7bca4-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7bca4-131">Request body</span></span>
<span data-ttu-id="7bca4-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7bca4-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7bca4-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="7bca4-133">Response</span></span>

<span data-ttu-id="7bca4-134">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [schemaExtension](../resources/schemaextension.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7bca4-134">If successful, this method returns a `200 OK` response code and collection of [schemaExtension](../resources/schemaextension.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7bca4-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7bca4-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7bca4-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7bca4-136">Request</span></span>
<span data-ttu-id="7bca4-137">O exemplo a seguir mostra como procurar entre todas as extensões acessíveis para uma específica filtrando sua **ID**exclusiva.</span><span class="sxs-lookup"><span data-stu-id="7bca4-137">The following example shows how to look among all the accessible extensions for a specific one by filtering on its unique **id**.</span></span> 

# <a name="http"></a>[<span data-ttu-id="7bca4-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="7bca4-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_schemaextensions"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/schemaExtensions?$filter=id%20eq%20'graphlearn_test'
```
# <a name="c"></a>[<span data-ttu-id="7bca4-139">C#</span><span class="sxs-lookup"><span data-stu-id="7bca4-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-schemaextensions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7bca4-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7bca4-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-schemaextensions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7bca4-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7bca4-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-schemaextensions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7bca4-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="7bca4-142">Response</span></span>
<span data-ttu-id="7bca4-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7bca4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="7bca4-146">Confira também</span><span class="sxs-lookup"><span data-stu-id="7bca4-146">See also</span></span>

- [<span data-ttu-id="7bca4-147">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="7bca4-147">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="7bca4-148">Adicionar dados personalizados a grupos usando as extensões do esquema</span><span class="sxs-lookup"><span data-stu-id="7bca4-148">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


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
