---
title: List schemaExtensions
description: 'Obtenha uma lista de objetos schemaExtension criados por qualquer aplicativo que você possui no locatário atual (que pode ser '
localization_priority: Normal
author: dkershaw10
ms.openlocfilehash: eb01bb41fefc8f7eaf4c1778df6d84fe780c2e3f
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33603622"
---
# <a name="list-schemaextensions"></a><span data-ttu-id="ebfc1-103">List schemaExtensions</span><span class="sxs-lookup"><span data-stu-id="ebfc1-103">List schemaExtensions</span></span>

<span data-ttu-id="ebfc1-104">Obtenha uma lista de objetos [schemaExtension](../resources/schemaextension.md) criados por qualquer aplicativo que você possui no locatário atual (que pode ser **indevelopment**, **disponível**ou preterido) e todas as outras extensões de esquema pertencentes a outros aplicativos marcados \*\*\*\* como \*\* Disponível\*\*.</span><span class="sxs-lookup"><span data-stu-id="ebfc1-104">Get a list of [schemaExtension](../resources/schemaextension.md) objects created by any apps you own in the current tenant (that can be **InDevelopment**, **Available**, or **Deprecated**), and all other schema extensions owned by other apps that are marked as **Available**.</span></span> 

## <a name="permissions"></a><span data-ttu-id="ebfc1-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="ebfc1-105">Permissions</span></span>
<span data-ttu-id="ebfc1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ebfc1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ebfc1-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ebfc1-108">Permission type</span></span>      | <span data-ttu-id="ebfc1-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ebfc1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ebfc1-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ebfc1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ebfc1-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ebfc1-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ebfc1-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ebfc1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ebfc1-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ebfc1-113">Not supported.</span></span>    |
|<span data-ttu-id="ebfc1-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ebfc1-114">Application</span></span> | <span data-ttu-id="ebfc1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ebfc1-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ebfc1-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ebfc1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /schemaExtensions
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ebfc1-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ebfc1-117">Optional query parameters</span></span>
<span data-ttu-id="ebfc1-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ebfc1-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ebfc1-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ebfc1-119">Request headers</span></span>
| <span data-ttu-id="ebfc1-120">Nome</span><span class="sxs-lookup"><span data-stu-id="ebfc1-120">Name</span></span>      |<span data-ttu-id="ebfc1-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="ebfc1-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ebfc1-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ebfc1-122">Authorization</span></span>  | <span data-ttu-id="ebfc1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ebfc1-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ebfc1-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ebfc1-125">Content-Type</span></span>   | <span data-ttu-id="ebfc1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ebfc1-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="ebfc1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ebfc1-127">Request body</span></span>
<span data-ttu-id="ebfc1-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ebfc1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ebfc1-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ebfc1-129">Response</span></span>

<span data-ttu-id="ebfc1-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [schemaExtension](../resources/schemaextension.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ebfc1-130">If successful, this method returns a `200 OK` response code and collection of [schemaExtension](../resources/schemaextension.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ebfc1-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ebfc1-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ebfc1-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ebfc1-132">Request</span></span>
<span data-ttu-id="ebfc1-133">O exemplo a seguir mostra como procurar entre todas as extensões acessíveis para uma específica filtrando sua **ID**exclusiva.</span><span class="sxs-lookup"><span data-stu-id="ebfc1-133">The following example shows how to look among all the accessible extensions for a specific one by filtering on its unique **id**.</span></span> 
<!-- {
  "blockType": "request",
  "name": "get_schemaextensions"
}-->
```http
GET https://graph.microsoft.com/v1.0/schemaExtensions?$filter=id%20eq%20'graphlearn_test'
```
##### <a name="response"></a><span data-ttu-id="ebfc1-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="ebfc1-134">Response</span></span>
<span data-ttu-id="ebfc1-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ebfc1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="ebfc1-138">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="ebfc1-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ebfc1-139">Basic</span><span class="sxs-lookup"><span data-stu-id="ebfc1-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_schemaextensions-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ebfc1-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ebfc1-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_schemaextensions-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="ebfc1-141">Confira também</span><span class="sxs-lookup"><span data-stu-id="ebfc1-141">See also</span></span>

- [<span data-ttu-id="ebfc1-142">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="ebfc1-142">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="ebfc1-143">Adicionar dados personalizados a grupos usando as extensões do esquema</span><span class="sxs-lookup"><span data-stu-id="ebfc1-143">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List schemaExtensions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/schemaextension-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/schemaextension-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
