---
title: Obter administrativeUnit
description: Recupere as propriedades e os relacionamentos de um objeto administrativeUnit.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3dbb2fede88e2232fdb14761549de03c2ec129d7
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36318996"
---
# <a name="get-administrativeunit"></a><span data-ttu-id="2a0f9-103">Obter administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="2a0f9-103">Get administrativeUnit</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a0f9-104">Recupere as propriedades e os relacionamentos de um objeto [administrativeUnit](../resources/administrativeunit.md) .</span><span class="sxs-lookup"><span data-stu-id="2a0f9-104">Retrieve the properties and relationships of an [administrativeUnit](../resources/administrativeunit.md) object.</span></span>

<span data-ttu-id="2a0f9-105">Como o recurso **administrativeUnit** oferece suporte a [extensões](/graph/extensibility-overview), você também pode `GET` usar a operação para obter propriedades personalizadas e dados de extensão em uma instância do **administrativeUnit** .</span><span class="sxs-lookup"><span data-stu-id="2a0f9-105">Since the **administrativeUnit** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in an **administrativeUnit** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="2a0f9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2a0f9-106">Permissions</span></span>
<span data-ttu-id="2a0f9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a0f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="2a0f9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2a0f9-109">Permission type</span></span>      | <span data-ttu-id="2a0f9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2a0f9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2a0f9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2a0f9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2a0f9-112">AdministrativeUnit. Read. All, Directory. Read. All, AdministrativeUnit. ReadWrite. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="2a0f9-112">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2a0f9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2a0f9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2a0f9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2a0f9-114">Not supported.</span></span>    |
|<span data-ttu-id="2a0f9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2a0f9-115">Application</span></span> | <span data-ttu-id="2a0f9-116">AdministrativeUnit. Read. All, Directory. Read. All, AdministrativeUnit. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="2a0f9-116">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2a0f9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2a0f9-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /administrativeUnits/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2a0f9-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2a0f9-118">Optional query parameters</span></span>
<span data-ttu-id="2a0f9-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2a0f9-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2a0f9-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2a0f9-120">Request headers</span></span>
| <span data-ttu-id="2a0f9-121">Nome</span><span class="sxs-lookup"><span data-stu-id="2a0f9-121">Name</span></span>      |<span data-ttu-id="2a0f9-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="2a0f9-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2a0f9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2a0f9-123">Authorization</span></span>  | <span data-ttu-id="2a0f9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2a0f9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2a0f9-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2a0f9-126">Request body</span></span>
<span data-ttu-id="2a0f9-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2a0f9-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2a0f9-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a0f9-128">Response</span></span>

<span data-ttu-id="2a0f9-129">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [administrativeUnit](../resources/administrativeunit.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2a0f9-129">If successful, this method returns a `200 OK` response code and [administrativeUnit](../resources/administrativeunit.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2a0f9-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2a0f9-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2a0f9-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2a0f9-131">Request</span></span>
<span data-ttu-id="2a0f9-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2a0f9-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2a0f9-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="2a0f9-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_administrativeunit"
}-->
```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2a0f9-134">C#</span><span class="sxs-lookup"><span data-stu-id="2a0f9-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-administrativeunit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2a0f9-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2a0f9-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-administrativeunit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2a0f9-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="2a0f9-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-administrativeunit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="2a0f9-137">Java</span><span class="sxs-lookup"><span data-stu-id="2a0f9-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-administrativeunit-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2a0f9-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a0f9-138">Response</span></span>
<span data-ttu-id="2a0f9-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2a0f9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.administrativeUnit"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 134

{
  "displayName": "displayName-value",
  "description": "description-value",
  "visibility": "visibility-value",
  "id": "id-value"
}
```

## <a name="see-also"></a><span data-ttu-id="2a0f9-142">Confira também</span><span class="sxs-lookup"><span data-stu-id="2a0f9-142">See also</span></span>

- [<span data-ttu-id="2a0f9-143">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="2a0f9-143">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="2a0f9-144">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="2a0f9-144">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get administrativeUnit",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
