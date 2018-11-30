---
title: Listar schemaExtensions
description: 'Obtenha uma lista de objetos schemaExtension criados por qualquer apps que você é proprietário no locatário atual (que pode ser '
ms.openlocfilehash: 9e366ae62276198ad08f322646c920816d25ec64
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037903"
---
# <a name="list-schemaextensions"></a><span data-ttu-id="cbd79-103">Listar schemaExtensions</span><span class="sxs-lookup"><span data-stu-id="cbd79-103">List schemaExtensions</span></span>

> <span data-ttu-id="cbd79-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="cbd79-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cbd79-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="cbd79-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cbd79-106">Obtenha uma lista de objetos [schemaExtension](../resources/schemaextension.md) criados por aplicativos que você possui no locatário atual (que pode ser **InDevelopment**, **Available** ou **Deprecated**) e todas as outras extensões de esquema pertencentes a outros aplicativos que estão marcadas como **Available**.</span><span class="sxs-lookup"><span data-stu-id="cbd79-106">Get a list of [schemaExtension](../resources/schemaextension.md) objects created by any apps you own in the current tenant (that can be **InDevelopment**, **Available**, or **Deprecated**), and all other schema extensions owned by other apps that are marked as **Available**.</span></span> 

## <a name="permissions"></a><span data-ttu-id="cbd79-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="cbd79-107">Permissions</span></span>
<span data-ttu-id="cbd79-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cbd79-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="cbd79-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cbd79-110">Permission type</span></span>      | <span data-ttu-id="cbd79-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cbd79-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cbd79-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cbd79-112">Delegated (work or school account)</span></span> | <span data-ttu-id="cbd79-113">Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cbd79-113">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cbd79-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cbd79-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cbd79-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cbd79-115">Not supported.</span></span>    |
|<span data-ttu-id="cbd79-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cbd79-116">Application</span></span> | <span data-ttu-id="cbd79-117">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="cbd79-117">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cbd79-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cbd79-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /schemaExtensions
```
## <a name="optional-query-parameters"></a><span data-ttu-id="cbd79-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="cbd79-119">Optional query parameters</span></span>
<span data-ttu-id="cbd79-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="cbd79-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cbd79-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cbd79-121">Request headers</span></span>
| <span data-ttu-id="cbd79-122">Nome</span><span class="sxs-lookup"><span data-stu-id="cbd79-122">Name</span></span>      |<span data-ttu-id="cbd79-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="cbd79-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="cbd79-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="cbd79-124">Authorization</span></span>  | <span data-ttu-id="cbd79-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cbd79-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cbd79-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cbd79-127">Content-Type</span></span>   | <span data-ttu-id="cbd79-128">application/json</span><span class="sxs-lookup"><span data-stu-id="cbd79-128">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="cbd79-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cbd79-129">Request body</span></span>
<span data-ttu-id="cbd79-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cbd79-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cbd79-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="cbd79-131">Response</span></span>

<span data-ttu-id="cbd79-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [schemaExtension](../resources/schemaextension.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cbd79-132">If successful, this method returns a `200 OK` response code and collection of [schemaExtension](../resources/schemaextension.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cbd79-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cbd79-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cbd79-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cbd79-134">Request</span></span>
<span data-ttu-id="cbd79-135">O exemplo a seguir mostra como procurar entre todas as extensões acessíveis uma que seja específica ao filtrar sua **id** exclusiva.</span><span class="sxs-lookup"><span data-stu-id="cbd79-135">The following example shows how to look among all the accessible extensions for a specific one by filtering on its unique **id**.</span></span> 
<!-- {
  "blockType": "request",
  "name": "get_schemaextensions"
}-->
```http
GET https://graph.microsoft.com/beta/schemaExtensions?$filter=id%20eq%20'graphlearn_test'
```
##### <a name="response"></a><span data-ttu-id="cbd79-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="cbd79-136">Response</span></span>
<span data-ttu-id="cbd79-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cbd79-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="cbd79-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="cbd79-140">See also</span></span>

- [<span data-ttu-id="cbd79-141">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="cbd79-141">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="cbd79-142">Adicionar dados personalizados a grupos usando as extensões do esquema</span><span class="sxs-lookup"><span data-stu-id="cbd79-142">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List schemaExtensions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->