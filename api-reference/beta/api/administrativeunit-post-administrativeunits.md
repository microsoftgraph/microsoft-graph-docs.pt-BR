---
title: Criar administrativeUnit
description: Use esta API para criar um novo administrativeUnit.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b46cb950fa88fa086e4417904c28d0bcb8dd41c6
ms.sourcegitcommit: fc9edd17aebed91768e31416e1c1ee0b64d5ce06
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/27/2019
ms.locfileid: "39621592"
---
# <a name="create-administrativeunit"></a><span data-ttu-id="66c93-103">Criar administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="66c93-103">Create administrativeUnit</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66c93-104">Use esta API para criar um novo [administrativeUnit](../resources/administrativeunit.md).</span><span class="sxs-lookup"><span data-stu-id="66c93-104">Use this API to create a new [administrativeUnit](../resources/administrativeunit.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="66c93-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="66c93-105">Permissions</span></span>
<span data-ttu-id="66c93-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66c93-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="66c93-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="66c93-108">Permission type</span></span>      | <span data-ttu-id="66c93-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="66c93-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="66c93-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="66c93-110">Delegated (work or school account)</span></span> | <span data-ttu-id="66c93-111">AdministrativeUnit. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="66c93-111">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="66c93-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="66c93-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66c93-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="66c93-113">Not supported.</span></span>    |
|<span data-ttu-id="66c93-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="66c93-114">Application</span></span> | <span data-ttu-id="66c93-115">AdministrativeUnit.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66c93-115">AdministrativeUnit.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="66c93-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="66c93-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits

```
## <a name="request-headers"></a><span data-ttu-id="66c93-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="66c93-117">Request headers</span></span>
| <span data-ttu-id="66c93-118">Nome</span><span class="sxs-lookup"><span data-stu-id="66c93-118">Name</span></span>      |<span data-ttu-id="66c93-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="66c93-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="66c93-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="66c93-120">Authorization</span></span>  | <span data-ttu-id="66c93-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="66c93-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="66c93-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="66c93-123">Content-type</span></span> | <span data-ttu-id="66c93-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="66c93-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="66c93-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="66c93-126">Request body</span></span>
<span data-ttu-id="66c93-127">No corpo da solicitação, forneça uma representação JSON de um objeto [administrativeUnit](../resources/administrativeunit.md) .</span><span class="sxs-lookup"><span data-stu-id="66c93-127">In the request body, supply a JSON representation of an [administrativeUnit](../resources/administrativeunit.md) object.</span></span>

<span data-ttu-id="66c93-128">Como o recurso **administrativeUnit** oferece suporte a [extensões](/graph/extensibility-overview), você pode `POST` usar a operação e adicionar propriedades personalizadas com seus próprios dados à unidade administrativa ao criá-la.</span><span class="sxs-lookup"><span data-stu-id="66c93-128">Because the **administrativeUnit** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the administrative unit while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="66c93-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="66c93-129">Response</span></span>

<span data-ttu-id="66c93-130">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [administrativeUnit](../resources/administrativeunit.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="66c93-130">If successful, this method returns a `201 Created` response code and an [administrativeUnit](../resources/administrativeunit.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66c93-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="66c93-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="66c93-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="66c93-132">Request</span></span>

<span data-ttu-id="66c93-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="66c93-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="66c93-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="66c93-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_administrativeunit_from_administrativeunits"
}-->
```http
POST https://graph.microsoft.com/beta/administrativeUnits
Content-type: application/json
Content-length: 150

{
    "displayName": "Seattle District Technical Schools",
    "description": "Seattle district technical schools administration",
    "visibility": "HiddenMembership"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="66c93-135">C#</span><span class="sxs-lookup"><span data-stu-id="66c93-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-administrativeunit-from-administrativeunits-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="66c93-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="66c93-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-administrativeunit-from-administrativeunits-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="66c93-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="66c93-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-administrativeunit-from-administrativeunits-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="66c93-138">No corpo da solicitação, forneça uma representação JSON de um objeto [administrativeUnit](../resources/administrativeunit.md) .</span><span class="sxs-lookup"><span data-stu-id="66c93-138">In the request body, supply a JSON representation of an [administrativeUnit](../resources/administrativeunit.md) object.</span></span>

### <a name="response"></a><span data-ttu-id="66c93-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="66c93-139">Response</span></span>

<span data-ttu-id="66c93-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="66c93-140">The following is an example of the response.</span></span> 
> <span data-ttu-id="66c93-141">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="66c93-141">Note: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="66c93-142">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="66c93-142">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.administrativeUnit"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 172

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#administrativeUnits/$entity",
    "id": "7a3dc8f3-b3a0-4164-9a99-ed36f3af039f",
    "deletedDateTime": null,
    "displayName": "Seattle District Technical Schools",
    "description": "Seattle district technical schools administration",
    "visibility": "HiddenMembership"
}
```

## <a name="see-also"></a><span data-ttu-id="66c93-143">Confira também</span><span class="sxs-lookup"><span data-stu-id="66c93-143">See also</span></span>

- [<span data-ttu-id="66c93-144">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="66c93-144">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="66c93-145">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="66c93-145">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create administrativeUnit",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
