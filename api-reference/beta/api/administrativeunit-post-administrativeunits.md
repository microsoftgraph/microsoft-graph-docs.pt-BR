---
title: Criar administrativeUnit
description: Use esta API para criar um novo administrativeUnit.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c8c9c5199a9c0e78aabf237a71f802e2f9fb4d73
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36408644"
---
# <a name="create-administrativeunit"></a><span data-ttu-id="05c37-103">Criar administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="05c37-103">Create administrativeUnit</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="05c37-104">Use esta API para criar um novo [administrativeUnit](../resources/administrativeunit.md).</span><span class="sxs-lookup"><span data-stu-id="05c37-104">Use this API to create a new [administrativeUnit](../resources/administrativeunit.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="05c37-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="05c37-105">Permissions</span></span>
<span data-ttu-id="05c37-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05c37-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="05c37-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="05c37-108">Permission type</span></span>      | <span data-ttu-id="05c37-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="05c37-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="05c37-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="05c37-110">Delegated (work or school account)</span></span> | <span data-ttu-id="05c37-111">AdministrativeUnit. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="05c37-111">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="05c37-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="05c37-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="05c37-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="05c37-113">Not supported.</span></span>    |
|<span data-ttu-id="05c37-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="05c37-114">Application</span></span> | <span data-ttu-id="05c37-115">AdministrativeUnit. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="05c37-115">AdministrativeUnit.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="05c37-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="05c37-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits

```
## <a name="request-headers"></a><span data-ttu-id="05c37-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="05c37-117">Request headers</span></span>
| <span data-ttu-id="05c37-118">Nome</span><span class="sxs-lookup"><span data-stu-id="05c37-118">Name</span></span>      |<span data-ttu-id="05c37-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="05c37-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="05c37-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="05c37-120">Authorization</span></span>  | <span data-ttu-id="05c37-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="05c37-p102">Bearer {token}. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="05c37-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="05c37-123">Request body</span></span>
<span data-ttu-id="05c37-124">No corpo da solicitação, forneça uma representação JSON do objeto [administrativeUnit](../resources/administrativeunit.md) .</span><span class="sxs-lookup"><span data-stu-id="05c37-124">In the request body, supply a JSON representation of [administrativeUnit](../resources/administrativeunit.md) object.</span></span>

<span data-ttu-id="05c37-125">Como o recurso **administrativeUnit** oferece suporte a [extensões](/graph/extensibility-overview), você pode `POST` usar a operação e adicionar propriedades personalizadas com seus próprios dados à unidade administrativa ao criá-la.</span><span class="sxs-lookup"><span data-stu-id="05c37-125">Since the **administrativeUnit** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the administrative unit while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="05c37-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="05c37-126">Response</span></span>

<span data-ttu-id="05c37-127">Se bem-sucedido, este método retorna `201 Created` o código de resposta e o objeto [administrativeUnit](../resources/administrativeunit.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="05c37-127">If successful, this method returns `201 Created` response code and [administrativeUnit](../resources/administrativeunit.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05c37-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="05c37-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="05c37-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="05c37-129">Request</span></span>
<span data-ttu-id="05c37-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="05c37-130">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="05c37-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="05c37-131">HTTP</span></span>](#tab/http)
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
    "visibility": "true"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="05c37-132">C#</span><span class="sxs-lookup"><span data-stu-id="05c37-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-administrativeunit-from-administrativeunits-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="05c37-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="05c37-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-administrativeunit-from-administrativeunits-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="05c37-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="05c37-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-administrativeunit-from-administrativeunits-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="05c37-135">No corpo da solicitação, forneça uma representação JSON do objeto [administrativeUnit](../resources/administrativeunit.md) .</span><span class="sxs-lookup"><span data-stu-id="05c37-135">In the request body, supply a JSON representation of [administrativeUnit](../resources/administrativeunit.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="05c37-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="05c37-136">Response</span></span>
<span data-ttu-id="05c37-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="05c37-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "administrativeUnit": {
    "displayName": "Seattle District Technical Schools",
    "description": "Seattle district technical schools administration",
    "visibility": "true",
    "id": "7a3dc8f3-b3a0-4164-9a99-ed36f3af039f"
  }
}
```

## <a name="see-also"></a><span data-ttu-id="05c37-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="05c37-140">See also</span></span>

- [<span data-ttu-id="05c37-141">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="05c37-141">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="05c37-142">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="05c37-142">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
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
