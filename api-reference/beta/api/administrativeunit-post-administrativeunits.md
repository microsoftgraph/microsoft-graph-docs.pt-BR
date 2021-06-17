---
title: Criar administrativeUnit
description: Use essa API para criar um novo administrativeUnit.
author: DougKirschner
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: c363c5a387cbc0824b558cebfc03732cdf8fccb3
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/17/2021
ms.locfileid: "52991915"
---
# <a name="create-administrativeunit"></a><span data-ttu-id="ceab2-103">Criar administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="ceab2-103">Create administrativeUnit</span></span>

<span data-ttu-id="ceab2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ceab2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ceab2-105">Use essa API para criar um [novo administrativeUnit](../resources/administrativeunit.md).</span><span class="sxs-lookup"><span data-stu-id="ceab2-105">Use this API to create a new [administrativeUnit](../resources/administrativeunit.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="ceab2-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="ceab2-106">Permissions</span></span>
<span data-ttu-id="ceab2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ceab2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ceab2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ceab2-109">Permission type</span></span>      | <span data-ttu-id="ceab2-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ceab2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ceab2-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ceab2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ceab2-112">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ceab2-112">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ceab2-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ceab2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ceab2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ceab2-114">Not supported.</span></span>    |
|<span data-ttu-id="ceab2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ceab2-115">Application</span></span> | <span data-ttu-id="ceab2-116">AdministrativeUnit.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ceab2-116">AdministrativeUnit.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ceab2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ceab2-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits

```
## <a name="request-headers"></a><span data-ttu-id="ceab2-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ceab2-118">Request headers</span></span>
| <span data-ttu-id="ceab2-119">Nome</span><span class="sxs-lookup"><span data-stu-id="ceab2-119">Name</span></span>      |<span data-ttu-id="ceab2-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ceab2-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ceab2-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ceab2-121">Authorization</span></span>  | <span data-ttu-id="ceab2-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ceab2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ceab2-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="ceab2-124">Content-type</span></span> | <span data-ttu-id="ceab2-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ceab2-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ceab2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ceab2-127">Request body</span></span>
<span data-ttu-id="ceab2-128">No corpo da solicitação, fornece uma representação JSON de um [objeto administrativeUnit.](../resources/administrativeunit.md)</span><span class="sxs-lookup"><span data-stu-id="ceab2-128">In the request body, supply a JSON representation of an [administrativeUnit](../resources/administrativeunit.md) object.</span></span>

<span data-ttu-id="ceab2-129">Como o **recurso administrativeUnit** dá suporte a extensões, você pode usar a operação e adicionar propriedades [personalizadas](/graph/extensibility-overview)com seus próprios dados à unidade administrativa durante `POST` a criação.</span><span class="sxs-lookup"><span data-stu-id="ceab2-129">Because the **administrativeUnit** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the administrative unit while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="ceab2-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="ceab2-130">Response</span></span>

<span data-ttu-id="ceab2-131">Se tiver êxito, este método retornará um código `201 Created` de resposta e um objeto [administrativeUnit](../resources/administrativeunit.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ceab2-131">If successful, this method returns a `201 Created` response code and an [administrativeUnit](../resources/administrativeunit.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ceab2-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ceab2-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="ceab2-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ceab2-133">Request</span></span>

<span data-ttu-id="ceab2-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ceab2-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ceab2-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="ceab2-135">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="ceab2-136">C#</span><span class="sxs-lookup"><span data-stu-id="ceab2-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-administrativeunit-from-administrativeunits-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ceab2-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ceab2-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-administrativeunit-from-administrativeunits-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ceab2-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ceab2-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-administrativeunit-from-administrativeunits-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ceab2-139">Java</span><span class="sxs-lookup"><span data-stu-id="ceab2-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-administrativeunit-from-administrativeunits-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="ceab2-140">No corpo da solicitação, fornece uma representação JSON de um [objeto administrativeUnit.](../resources/administrativeunit.md)</span><span class="sxs-lookup"><span data-stu-id="ceab2-140">In the request body, supply a JSON representation of an [administrativeUnit](../resources/administrativeunit.md) object.</span></span>

### <a name="response"></a><span data-ttu-id="ceab2-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="ceab2-141">Response</span></span>

<span data-ttu-id="ceab2-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ceab2-142">The following is an example of the response.</span></span> 
> <span data-ttu-id="ceab2-143">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ceab2-143">Note: The response object shown here might be shortened for readability.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="ceab2-144">Confira também</span><span class="sxs-lookup"><span data-stu-id="ceab2-144">See also</span></span>

- [<span data-ttu-id="ceab2-145">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="ceab2-145">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="ceab2-146">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="ceab2-146">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
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


