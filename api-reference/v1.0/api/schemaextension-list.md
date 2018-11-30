---
title: Listar schemaExtensions
description: 'Obtenha uma lista de objetos schemaExtension criados por qualquer apps que você é proprietário no locatário atual (que pode ser '
ms.openlocfilehash: b5e11856156094cc797b9e620c8e2d3ff82da349
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007223"
---
# <a name="list-schemaextensions"></a><span data-ttu-id="76a0d-103">Listar schemaExtensions</span><span class="sxs-lookup"><span data-stu-id="76a0d-103">List schemaExtensions</span></span>

<span data-ttu-id="76a0d-104">Obtenha uma lista de objetos [schemaExtension](../resources/schemaextension.md) criados por aplicativos que você possui no locatário atual (que pode ser **InDevelopment**, **Available** ou **Deprecated**) e todas as outras extensões de esquema pertencentes a outros aplicativos que estão marcadas como **Available**.</span><span class="sxs-lookup"><span data-stu-id="76a0d-104">Get a list of [schemaExtension](../resources/schemaextension.md) objects created by any apps you own in the current tenant (that can be **InDevelopment**, **Available**, or **Deprecated**), and all other schema extensions owned by other apps that are marked as **Available**.</span></span> 

## <a name="permissions"></a><span data-ttu-id="76a0d-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="76a0d-105">Permissions</span></span>
<span data-ttu-id="76a0d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76a0d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="76a0d-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="76a0d-108">Permission type</span></span>      | <span data-ttu-id="76a0d-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="76a0d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="76a0d-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="76a0d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="76a0d-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="76a0d-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="76a0d-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="76a0d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="76a0d-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="76a0d-113">Not supported.</span></span>    |
|<span data-ttu-id="76a0d-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="76a0d-114">Application</span></span> | <span data-ttu-id="76a0d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="76a0d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="76a0d-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="76a0d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /schemaExtensions
```
## <a name="optional-query-parameters"></a><span data-ttu-id="76a0d-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="76a0d-117">Optional query parameters</span></span>
<span data-ttu-id="76a0d-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="76a0d-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="76a0d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="76a0d-119">Request headers</span></span>
| <span data-ttu-id="76a0d-120">Nome</span><span class="sxs-lookup"><span data-stu-id="76a0d-120">Name</span></span>      |<span data-ttu-id="76a0d-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="76a0d-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="76a0d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="76a0d-122">Authorization</span></span>  | <span data-ttu-id="76a0d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="76a0d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="76a0d-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="76a0d-125">Content-Type</span></span>   | <span data-ttu-id="76a0d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="76a0d-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="76a0d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="76a0d-127">Request body</span></span>
<span data-ttu-id="76a0d-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="76a0d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="76a0d-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="76a0d-129">Response</span></span>

<span data-ttu-id="76a0d-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [schemaExtension](../resources/schemaextension.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="76a0d-130">If successful, this method returns a `200 OK` response code and collection of [schemaExtension](../resources/schemaextension.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="76a0d-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="76a0d-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="76a0d-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="76a0d-132">Request</span></span>
<span data-ttu-id="76a0d-133">O exemplo a seguir mostra como procurar entre todas as extensões acessíveis uma que seja específica ao filtrar sua **id** exclusiva.</span><span class="sxs-lookup"><span data-stu-id="76a0d-133">The following example shows how to look among all the accessible extensions for a specific one by filtering on its unique **id**.</span></span> 
<!-- {
  "blockType": "request",
  "name": "get_schemaextensions"
}-->
```http
GET https://graph.microsoft.com/v1.0/schemaExtensions?$filter=id%20eq%20'graphlearn_test'
```
##### <a name="response"></a><span data-ttu-id="76a0d-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="76a0d-134">Response</span></span>
<span data-ttu-id="76a0d-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="76a0d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="76a0d-138">Confira também</span><span class="sxs-lookup"><span data-stu-id="76a0d-138">See also</span></span>

- [<span data-ttu-id="76a0d-139">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="76a0d-139">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="76a0d-140">Adicionar dados personalizados a grupos usando as extensões do esquema</span><span class="sxs-lookup"><span data-stu-id="76a0d-140">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List schemaExtensions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->