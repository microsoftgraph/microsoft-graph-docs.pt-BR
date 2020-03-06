---
title: Get schemaExtension
description: Obtenha as propriedades da definição schemaExtension especificada.
localization_priority: Normal
author: dkershaw10
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 163d13fd4045442188aee76c39b5f2bfa6af893a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42509959"
---
# <a name="get-schemaextension"></a><span data-ttu-id="b23d2-103">Get schemaExtension</span><span class="sxs-lookup"><span data-stu-id="b23d2-103">Get schemaExtension</span></span>

<span data-ttu-id="b23d2-104">Namespace: Microsoft. Graph Obtém as propriedades da definição [schemaExtension](../resources/schemaextension.md) especificada.</span><span class="sxs-lookup"><span data-stu-id="b23d2-104">Namespace: microsoft.graph Get the properties of the specified [schemaExtension](../resources/schemaextension.md) definition.</span></span>

## <a name="permissions"></a><span data-ttu-id="b23d2-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b23d2-105">Permissions</span></span>
<span data-ttu-id="b23d2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b23d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b23d2-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b23d2-108">Permission type</span></span>      | <span data-ttu-id="b23d2-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b23d2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b23d2-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b23d2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b23d2-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b23d2-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b23d2-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b23d2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b23d2-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b23d2-113">Not supported.</span></span>    |
|<span data-ttu-id="b23d2-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b23d2-114">Application</span></span> | <span data-ttu-id="b23d2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b23d2-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b23d2-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b23d2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /schemaExtensions/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b23d2-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b23d2-117">Optional query parameters</span></span>
<span data-ttu-id="b23d2-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b23d2-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b23d2-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b23d2-119">Request headers</span></span>
| <span data-ttu-id="b23d2-120">Nome</span><span class="sxs-lookup"><span data-stu-id="b23d2-120">Name</span></span>      |<span data-ttu-id="b23d2-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="b23d2-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b23d2-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b23d2-122">Authorization</span></span>  | <span data-ttu-id="b23d2-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b23d2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b23d2-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b23d2-125">Content-Type</span></span>   | <span data-ttu-id="b23d2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b23d2-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="b23d2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b23d2-127">Request body</span></span>
<span data-ttu-id="b23d2-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b23d2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b23d2-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b23d2-129">Response</span></span>

<span data-ttu-id="b23d2-130">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [schemaExtension](../resources/schemaextension.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b23d2-130">If successful, this method returns a `200 OK` response code and [schemaExtension](../resources/schemaextension.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b23d2-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b23d2-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b23d2-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b23d2-132">Request</span></span>
<span data-ttu-id="b23d2-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b23d2-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_schemaextension"
}-->
```http
GET https://graph.microsoft.com/v1.0/schemaExtensions/graphlearn_test
```
##### <a name="response"></a><span data-ttu-id="b23d2-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b23d2-134">Response</span></span>
<span data-ttu-id="b23d2-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b23d2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

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
```

## <a name="see-also"></a><span data-ttu-id="b23d2-138">Confira também</span><span class="sxs-lookup"><span data-stu-id="b23d2-138">See also</span></span>

- [<span data-ttu-id="b23d2-139">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="b23d2-139">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="b23d2-140">Adicionar dados personalizados a grupos usando as extensões do esquema</span><span class="sxs-lookup"><span data-stu-id="b23d2-140">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get schemaExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
