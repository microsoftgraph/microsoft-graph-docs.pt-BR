---
title: Criar administrativeUnit
description: Use esta API para criar um novo administrativeUnit.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 891e281554015ac453a678f78e4f299babf46f4b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35945771"
---
# <a name="create-administrativeunit"></a><span data-ttu-id="6a03b-103">Criar administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="6a03b-103">Create administrativeUnit</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a03b-104">Use esta API para criar um novo [administrativeUnit](../resources/administrativeunit.md).</span><span class="sxs-lookup"><span data-stu-id="6a03b-104">Use this API to create a new [administrativeUnit](../resources/administrativeunit.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="6a03b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="6a03b-105">Permissions</span></span>
<span data-ttu-id="6a03b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a03b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="6a03b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6a03b-108">Permission type</span></span>      | <span data-ttu-id="6a03b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6a03b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6a03b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6a03b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6a03b-111">AdministrativeUnit. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="6a03b-111">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6a03b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6a03b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a03b-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6a03b-113">Not supported.</span></span>    |
|<span data-ttu-id="6a03b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6a03b-114">Application</span></span> | <span data-ttu-id="6a03b-115">AdministrativeUnit. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="6a03b-115">AdministrativeUnit.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6a03b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6a03b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits

```
## <a name="request-headers"></a><span data-ttu-id="6a03b-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6a03b-117">Request headers</span></span>
| <span data-ttu-id="6a03b-118">Nome</span><span class="sxs-lookup"><span data-stu-id="6a03b-118">Name</span></span>      |<span data-ttu-id="6a03b-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a03b-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6a03b-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="6a03b-120">Authorization</span></span>  | <span data-ttu-id="6a03b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6a03b-p102">Bearer {token}. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="6a03b-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6a03b-123">Request body</span></span>
<span data-ttu-id="6a03b-124">No corpo da solicitação, forneça uma representação JSON do objeto [administrativeUnit](../resources/administrativeunit.md) .</span><span class="sxs-lookup"><span data-stu-id="6a03b-124">In the request body, supply a JSON representation of [administrativeUnit](../resources/administrativeunit.md) object.</span></span>

<span data-ttu-id="6a03b-125">Como o recurso **administrativeUnit** oferece suporte a [extensões](/graph/extensibility-overview), você pode `POST` usar a operação e adicionar propriedades personalizadas com seus próprios dados à unidade administrativa ao criá-la.</span><span class="sxs-lookup"><span data-stu-id="6a03b-125">Since the **administrativeUnit** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the administrative unit while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="6a03b-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a03b-126">Response</span></span>

<span data-ttu-id="6a03b-127">Se bem-sucedido, este método retorna `201 Created` o código de resposta e o objeto [administrativeUnit](../resources/administrativeunit.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6a03b-127">If successful, this method returns `201 Created` response code and [administrativeUnit](../resources/administrativeunit.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a03b-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6a03b-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6a03b-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6a03b-129">Request</span></span>
<span data-ttu-id="6a03b-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6a03b-130">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6a03b-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="6a03b-131">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="6a03b-132">C#</span><span class="sxs-lookup"><span data-stu-id="6a03b-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-administrativeunit-from-administrativeunits-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6a03b-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="6a03b-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-administrativeunit-from-administrativeunits-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6a03b-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="6a03b-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-administrativeunit-from-administrativeunits-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="6a03b-135">Java</span><span class="sxs-lookup"><span data-stu-id="6a03b-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-administrativeunit-from-administrativeunits-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="6a03b-136">No corpo da solicitação, forneça uma representação JSON do objeto [administrativeUnit](../resources/administrativeunit.md) .</span><span class="sxs-lookup"><span data-stu-id="6a03b-136">In the request body, supply a JSON representation of [administrativeUnit](../resources/administrativeunit.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="6a03b-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a03b-137">Response</span></span>
<span data-ttu-id="6a03b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6a03b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="6a03b-141">Confira também</span><span class="sxs-lookup"><span data-stu-id="6a03b-141">See also</span></span>

- [<span data-ttu-id="6a03b-142">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="6a03b-142">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="6a03b-143">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="6a03b-143">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
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
