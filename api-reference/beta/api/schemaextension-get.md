---
title: Obter schemaExtension
description: Obtenha as propriedades da definição schemaExtension especificada.
localization_priority: Normal
ms.openlocfilehash: 090fb2131aa5cbbea845c3b9bfed2f807b4c8659
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27852777"
---
# <a name="get-schemaextension"></a><span data-ttu-id="15a76-103">Obter schemaExtension</span><span class="sxs-lookup"><span data-stu-id="15a76-103">Get schemaExtension</span></span>

> <span data-ttu-id="15a76-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="15a76-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="15a76-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="15a76-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="15a76-106">Obtenha as propriedades da definição [schemaExtension](../resources/schemaextension.md) especificada.</span><span class="sxs-lookup"><span data-stu-id="15a76-106">Get the properties of the specified [schemaExtension](../resources/schemaextension.md) definition.</span></span>

## <a name="permissions"></a><span data-ttu-id="15a76-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="15a76-107">Permissions</span></span>
<span data-ttu-id="15a76-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15a76-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="15a76-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="15a76-110">Permission type</span></span>      | <span data-ttu-id="15a76-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="15a76-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="15a76-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="15a76-112">Delegated (work or school account)</span></span> | <span data-ttu-id="15a76-113">Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="15a76-113">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="15a76-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="15a76-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15a76-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="15a76-115">Not supported.</span></span>    |
|<span data-ttu-id="15a76-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="15a76-116">Application</span></span> | <span data-ttu-id="15a76-117">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="15a76-117">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="15a76-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="15a76-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /schemaExtensions/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="15a76-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="15a76-119">Optional query parameters</span></span>
<span data-ttu-id="15a76-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="15a76-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="15a76-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="15a76-121">Request headers</span></span>
| <span data-ttu-id="15a76-122">Nome</span><span class="sxs-lookup"><span data-stu-id="15a76-122">Name</span></span>      |<span data-ttu-id="15a76-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="15a76-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="15a76-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="15a76-124">Authorization</span></span>  | <span data-ttu-id="15a76-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="15a76-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="15a76-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="15a76-127">Content-Type</span></span>   | <span data-ttu-id="15a76-128">application/json</span><span class="sxs-lookup"><span data-stu-id="15a76-128">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="15a76-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="15a76-129">Request body</span></span>
<span data-ttu-id="15a76-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="15a76-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="15a76-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="15a76-131">Response</span></span>

<span data-ttu-id="15a76-132">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [schemaExtension](../resources/schemaextension.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="15a76-132">If successful, this method returns a `200 OK` response code and [schemaExtension](../resources/schemaextension.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="15a76-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="15a76-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="15a76-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="15a76-134">Request</span></span>
<span data-ttu-id="15a76-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="15a76-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_schemaextension"
}-->
```http
GET https://graph.microsoft.com/beta/schemaExtensions/graphlearn_test
```
##### <a name="response"></a><span data-ttu-id="15a76-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="15a76-136">Response</span></span>
<span data-ttu-id="15a76-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="15a76-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
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

## <a name="see-also"></a><span data-ttu-id="15a76-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="15a76-140">See also</span></span>

- [<span data-ttu-id="15a76-141">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="15a76-141">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="15a76-142">Adicionar dados personalizados a grupos usando as extensões do esquema</span><span class="sxs-lookup"><span data-stu-id="15a76-142">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get schemaExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
