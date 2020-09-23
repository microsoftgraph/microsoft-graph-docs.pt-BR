---
title: Criar administrativeUnit
description: Use esta API para criar um novo administrativeUnit.
author: anandyadavMSFT
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 72d00bf19e25b29d4ce54c88afb7c54373a196ee
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/23/2020
ms.locfileid: "48223605"
---
# <a name="create-administrativeunit"></a><span data-ttu-id="40ebf-103">Criar administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="40ebf-103">Create administrativeUnit</span></span>

<span data-ttu-id="40ebf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40ebf-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="40ebf-105">Use esta API para criar um novo [administrativeUnit](../resources/administrativeunit.md).</span><span class="sxs-lookup"><span data-stu-id="40ebf-105">Use this API to create a new [administrativeUnit](../resources/administrativeunit.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="40ebf-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="40ebf-106">Permissions</span></span>
<span data-ttu-id="40ebf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40ebf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="40ebf-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="40ebf-109">Permission type</span></span>      | <span data-ttu-id="40ebf-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="40ebf-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="40ebf-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="40ebf-111">Delegated (work or school account)</span></span> | <span data-ttu-id="40ebf-112">AdministrativeUnit. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="40ebf-112">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="40ebf-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="40ebf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40ebf-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="40ebf-114">Not supported.</span></span>    |
|<span data-ttu-id="40ebf-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="40ebf-115">Application</span></span> | <span data-ttu-id="40ebf-116">AdministrativeUnit.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40ebf-116">AdministrativeUnit.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="40ebf-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="40ebf-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directory/administrativeUnits

```
## <a name="request-headers"></a><span data-ttu-id="40ebf-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="40ebf-118">Request headers</span></span>
| <span data-ttu-id="40ebf-119">Nome</span><span class="sxs-lookup"><span data-stu-id="40ebf-119">Name</span></span>      |<span data-ttu-id="40ebf-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="40ebf-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="40ebf-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="40ebf-121">Authorization</span></span>  | <span data-ttu-id="40ebf-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="40ebf-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="40ebf-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="40ebf-124">Content-type</span></span> | <span data-ttu-id="40ebf-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="40ebf-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="40ebf-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="40ebf-127">Request body</span></span>
<span data-ttu-id="40ebf-128">No corpo da solicitação, forneça uma representação JSON de um objeto [administrativeUnit](../resources/administrativeunit.md) .</span><span class="sxs-lookup"><span data-stu-id="40ebf-128">In the request body, supply a JSON representation of an [administrativeUnit](../resources/administrativeunit.md) object.</span></span>

<span data-ttu-id="40ebf-129">Como o recurso **administrativeUnit** oferece suporte a [extensões](/graph/extensibility-overview), você pode usar a `POST` operação e adicionar propriedades personalizadas com seus próprios dados à unidade administrativa ao criá-la.</span><span class="sxs-lookup"><span data-stu-id="40ebf-129">Because the **administrativeUnit** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the administrative unit while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="40ebf-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="40ebf-130">Response</span></span>

<span data-ttu-id="40ebf-131">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [administrativeUnit](../resources/administrativeunit.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="40ebf-131">If successful, this method returns a `201 Created` response code and an [administrativeUnit](../resources/administrativeunit.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40ebf-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="40ebf-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="40ebf-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="40ebf-133">Request</span></span>

<span data-ttu-id="40ebf-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="40ebf-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="40ebf-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="40ebf-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_administrativeunit_from_administrativeunits"
}-->
```http
POST https://graph.microsoft.com/v1.0/directory/administrativeUnits
Content-type: application/json
Content-length: 150

{
    "displayName": "Seattle District Technical Schools",
    "description": "Seattle district technical schools administration",
    "visibility": "HiddenMembership"
}
```
# <a name="c"></a>[<span data-ttu-id="40ebf-136">C#</span><span class="sxs-lookup"><span data-stu-id="40ebf-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-administrativeunit-from-administrativeunits-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="40ebf-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="40ebf-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-administrativeunit-from-administrativeunits-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="40ebf-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="40ebf-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-administrativeunit-from-administrativeunits-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="40ebf-139">Java</span><span class="sxs-lookup"><span data-stu-id="40ebf-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-administrativeunit-from-administrativeunits-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

<span data-ttu-id="40ebf-140">No corpo da solicitação, forneça uma representação JSON de um objeto [administrativeUnit](../resources/administrativeunit.md) .</span><span class="sxs-lookup"><span data-stu-id="40ebf-140">In the request body, supply a JSON representation of an [administrativeUnit](../resources/administrativeunit.md) object.</span></span>

### <a name="response"></a><span data-ttu-id="40ebf-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="40ebf-141">Response</span></span>

<span data-ttu-id="40ebf-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="40ebf-142">The following is an example of the response.</span></span> 
> <span data-ttu-id="40ebf-143">Observação: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="40ebf-143">Note: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="40ebf-144">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="40ebf-144">All the properties will be returned from an actual call.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#administrativeUnits/$entity",
    "id": "7a3dc8f3-b3a0-4164-9a99-ed36f3af039f",
    "deletedDateTime": null,
    "displayName": "Seattle District Technical Schools",
    "description": "Seattle district technical schools administration",
    "visibility": "HiddenMembership"
}
```

## <a name="see-also"></a><span data-ttu-id="40ebf-145">Confira também</span><span class="sxs-lookup"><span data-stu-id="40ebf-145">See also</span></span>

- [<span data-ttu-id="40ebf-146">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="40ebf-146">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="40ebf-147">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="40ebf-147">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
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
