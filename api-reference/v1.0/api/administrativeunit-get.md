---
title: Obter administrativeUnit
description: Recupere as propriedades e os relacionamentos de um objeto administrativeUnit.
author: anandyadavMSFT
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 47cf6fced71e59681a094dc7e89f430e1efd00f2
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2020
ms.locfileid: "48405530"
---
# <a name="get-administrativeunit"></a><span data-ttu-id="889a7-103">Obter administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="889a7-103">Get administrativeUnit</span></span>

<span data-ttu-id="889a7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="889a7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="889a7-105">Recupere as propriedades e os relacionamentos de um objeto [administrativeUnit](../resources/administrativeunit.md) .</span><span class="sxs-lookup"><span data-stu-id="889a7-105">Retrieve the properties and relationships of an [administrativeUnit](../resources/administrativeunit.md) object.</span></span>


## <a name="permissions"></a><span data-ttu-id="889a7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="889a7-106">Permissions</span></span>
<span data-ttu-id="889a7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="889a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="889a7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="889a7-109">Permission type</span></span>      | <span data-ttu-id="889a7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="889a7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="889a7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="889a7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="889a7-112">AdministrativeUnit. Read. All, Directory. Read. All, AdministrativeUnit. ReadWrite. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="889a7-112">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="889a7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="889a7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="889a7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="889a7-114">Not supported.</span></span>    |
|<span data-ttu-id="889a7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="889a7-115">Application</span></span> | <span data-ttu-id="889a7-116">AdministrativeUnit. Read. All, Directory. Read. All, AdministrativeUnit. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="889a7-116">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="889a7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="889a7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directory/administrativeUnits/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="889a7-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="889a7-118">Optional query parameters</span></span>
<span data-ttu-id="889a7-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="889a7-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="889a7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="889a7-120">Request headers</span></span>
| <span data-ttu-id="889a7-121">Nome</span><span class="sxs-lookup"><span data-stu-id="889a7-121">Name</span></span>      |<span data-ttu-id="889a7-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="889a7-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="889a7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="889a7-123">Authorization</span></span>  | <span data-ttu-id="889a7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="889a7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="889a7-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="889a7-126">Request body</span></span>
<span data-ttu-id="889a7-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="889a7-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="889a7-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="889a7-128">Response</span></span>

<span data-ttu-id="889a7-129">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [administrativeUnit](../resources/administrativeunit.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="889a7-129">If successful, this method returns a `200 OK` response code and [administrativeUnit](../resources/administrativeunit.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="889a7-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="889a7-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="889a7-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="889a7-131">Request</span></span>
<span data-ttu-id="889a7-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="889a7-132">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="889a7-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="889a7-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_administrativeunit"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directory/administrativeUnits/{id}
```
# <a name="c"></a>[<span data-ttu-id="889a7-134">C#</span><span class="sxs-lookup"><span data-stu-id="889a7-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-administrativeunit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="889a7-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="889a7-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-administrativeunit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="889a7-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="889a7-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-administrativeunit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="889a7-137">Java</span><span class="sxs-lookup"><span data-stu-id="889a7-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-administrativeunit-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

##### <a name="response"></a><span data-ttu-id="889a7-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="889a7-138">Response</span></span>
<span data-ttu-id="889a7-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="889a7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="889a7-142">Confira também</span><span class="sxs-lookup"><span data-stu-id="889a7-142">See also</span></span>

- [<span data-ttu-id="889a7-143">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="889a7-143">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="889a7-144">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="889a7-144">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
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