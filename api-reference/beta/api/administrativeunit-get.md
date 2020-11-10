---
title: Obter administrativeUnit
description: Recupere as propriedades e os relacionamentos de um objeto administrativeUnit.
author: anandyadavMSFT
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d674513606da3e19cb870c9a01a5bd106e29f060
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48962623"
---
# <a name="get-administrativeunit"></a><span data-ttu-id="f7b4d-103">Obter administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="f7b4d-103">Get administrativeUnit</span></span>

<span data-ttu-id="f7b4d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7b4d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7b4d-105">Recupere as propriedades e os relacionamentos de um objeto [administrativeUnit](../resources/administrativeunit.md) .</span><span class="sxs-lookup"><span data-stu-id="f7b4d-105">Retrieve the properties and relationships of an [administrativeUnit](../resources/administrativeunit.md) object.</span></span>

<span data-ttu-id="f7b4d-106">Como o recurso **administrativeUnit** oferece suporte a [extensões](/graph/extensibility-overview), você também pode usar a `GET` operação para obter propriedades personalizadas e dados de extensão em uma instância do **administrativeUnit** .</span><span class="sxs-lookup"><span data-stu-id="f7b4d-106">Since the **administrativeUnit** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in an **administrativeUnit** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="f7b4d-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f7b4d-107">Permissions</span></span>
<span data-ttu-id="f7b4d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7b4d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f7b4d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f7b4d-110">Permission type</span></span>      | <span data-ttu-id="f7b4d-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f7b4d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7b4d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f7b4d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f7b4d-113">AdministrativeUnit. Read. All, Directory. Read. All, AdministrativeUnit. ReadWrite. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="f7b4d-113">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f7b4d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f7b4d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7b4d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f7b4d-115">Not supported.</span></span>    |
|<span data-ttu-id="f7b4d-116">Application</span><span class="sxs-lookup"><span data-stu-id="f7b4d-116">Application</span></span> | <span data-ttu-id="f7b4d-117">AdministrativeUnit. Read. All, Directory. Read. All, AdministrativeUnit. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f7b4d-117">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f7b4d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f7b4d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /administrativeUnits/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f7b4d-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f7b4d-119">Optional query parameters</span></span>
<span data-ttu-id="f7b4d-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f7b4d-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f7b4d-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f7b4d-121">Request headers</span></span>
| <span data-ttu-id="f7b4d-122">Nome</span><span class="sxs-lookup"><span data-stu-id="f7b4d-122">Name</span></span>      |<span data-ttu-id="f7b4d-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7b4d-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f7b4d-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="f7b4d-124">Authorization</span></span>  | <span data-ttu-id="f7b4d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f7b4d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f7b4d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f7b4d-127">Request body</span></span>
<span data-ttu-id="f7b4d-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f7b4d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f7b4d-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7b4d-129">Response</span></span>

<span data-ttu-id="f7b4d-130">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [administrativeUnit](../resources/administrativeunit.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f7b4d-130">If successful, this method returns a `200 OK` response code and [administrativeUnit](../resources/administrativeunit.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f7b4d-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f7b4d-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f7b4d-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f7b4d-132">Request</span></span>
<span data-ttu-id="f7b4d-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f7b4d-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f7b4d-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="f7b4d-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_administrativeunit"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/administrativeUnits/{id}
```
# <a name="c"></a>[<span data-ttu-id="f7b4d-135">C#</span><span class="sxs-lookup"><span data-stu-id="f7b4d-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-administrativeunit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f7b4d-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f7b4d-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-administrativeunit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f7b4d-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f7b4d-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-administrativeunit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f7b4d-138">Java</span><span class="sxs-lookup"><span data-stu-id="f7b4d-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-administrativeunit-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f7b4d-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7b4d-139">Response</span></span>
<span data-ttu-id="f7b4d-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f7b4d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="f7b4d-143">Confira também</span><span class="sxs-lookup"><span data-stu-id="f7b4d-143">See also</span></span>

- [<span data-ttu-id="f7b4d-144">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="f7b4d-144">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="f7b4d-145">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="f7b4d-145">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
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
