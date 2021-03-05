---
title: Obter administrativeUnit
description: Recupere as propriedades e as relações de um objeto administrativeUnit.
author: anandyadavMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 83c6f6cb84800492b3736613a8d2116c0e605e7f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433016"
---
# <a name="get-administrativeunit"></a><span data-ttu-id="c902b-103">Obter administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="c902b-103">Get administrativeUnit</span></span>

<span data-ttu-id="c902b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c902b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c902b-105">Recupere as propriedades e as relações de um [objeto administrativeUnit.](../resources/administrativeunit.md)</span><span class="sxs-lookup"><span data-stu-id="c902b-105">Retrieve the properties and relationships of an [administrativeUnit](../resources/administrativeunit.md) object.</span></span>


## <a name="permissions"></a><span data-ttu-id="c902b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c902b-106">Permissions</span></span>
<span data-ttu-id="c902b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c902b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c902b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c902b-109">Permission type</span></span>      | <span data-ttu-id="c902b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c902b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c902b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c902b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c902b-112">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c902b-112">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c902b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c902b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c902b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c902b-114">Not supported.</span></span>    |
|<span data-ttu-id="c902b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c902b-115">Application</span></span> | <span data-ttu-id="c902b-116">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c902b-116">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c902b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c902b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directory/administrativeUnits/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c902b-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c902b-118">Optional query parameters</span></span>
<span data-ttu-id="c902b-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c902b-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c902b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c902b-120">Request headers</span></span>
| <span data-ttu-id="c902b-121">Nome</span><span class="sxs-lookup"><span data-stu-id="c902b-121">Name</span></span>      |<span data-ttu-id="c902b-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c902b-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c902b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c902b-123">Authorization</span></span>  | <span data-ttu-id="c902b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c902b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c902b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c902b-126">Request body</span></span>
<span data-ttu-id="c902b-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c902b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c902b-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="c902b-128">Response</span></span>

<span data-ttu-id="c902b-129">Se tiver êxito, este método retornará um código de resposta e um `200 OK` objeto [administrativeUnit](../resources/administrativeunit.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c902b-129">If successful, this method returns a `200 OK` response code and [administrativeUnit](../resources/administrativeunit.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c902b-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c902b-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c902b-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c902b-131">Request</span></span>
<span data-ttu-id="c902b-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c902b-132">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c902b-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="c902b-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_administrativeunit"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directory/administrativeUnits/{id}
```
# <a name="c"></a>[<span data-ttu-id="c902b-134">C#</span><span class="sxs-lookup"><span data-stu-id="c902b-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-administrativeunit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c902b-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c902b-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-administrativeunit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c902b-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c902b-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-administrativeunit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c902b-137">Java</span><span class="sxs-lookup"><span data-stu-id="c902b-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-administrativeunit-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

##### <a name="response"></a><span data-ttu-id="c902b-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="c902b-138">Response</span></span>
<span data-ttu-id="c902b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c902b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="c902b-142">Confira também</span><span class="sxs-lookup"><span data-stu-id="c902b-142">See also</span></span>

- [<span data-ttu-id="c902b-143">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="c902b-143">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="c902b-144">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="c902b-144">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
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
