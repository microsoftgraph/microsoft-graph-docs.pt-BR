---
title: Criar administrativeUnit
description: Use esta API para criar um novo administrativeUnit.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4815082a8a5930e426e0843d2dcf2ebe6ef190d5
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636629"
---
# <a name="create-administrativeunit"></a><span data-ttu-id="9983a-103">Criar administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="9983a-103">Create administrativeUnit</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9983a-104">Use esta API para criar um novo [administrativeUnit](../resources/administrativeunit.md).</span><span class="sxs-lookup"><span data-stu-id="9983a-104">Use this API to create a new [administrativeUnit](../resources/administrativeunit.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="9983a-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="9983a-105">Permissions</span></span>
<span data-ttu-id="9983a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9983a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="9983a-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9983a-108">Permission type</span></span>      | <span data-ttu-id="9983a-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9983a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9983a-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9983a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9983a-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9983a-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9983a-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9983a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9983a-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9983a-113">Not supported.</span></span>    |
|<span data-ttu-id="9983a-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9983a-114">Application</span></span> | <span data-ttu-id="9983a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9983a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9983a-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9983a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits

```
## <a name="request-headers"></a><span data-ttu-id="9983a-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9983a-117">Request headers</span></span>
| <span data-ttu-id="9983a-118">Nome</span><span class="sxs-lookup"><span data-stu-id="9983a-118">Name</span></span>      |<span data-ttu-id="9983a-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="9983a-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9983a-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="9983a-120">Authorization</span></span>  | <span data-ttu-id="9983a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9983a-p102">Bearer {token}. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="9983a-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9983a-123">Request body</span></span>
<span data-ttu-id="9983a-124">No corpo da solicitação, forneça uma representação JSON do objeto [administrativeUnit](../resources/administrativeunit.md) .</span><span class="sxs-lookup"><span data-stu-id="9983a-124">In the request body, supply a JSON representation of [administrativeUnit](../resources/administrativeunit.md) object.</span></span>

<span data-ttu-id="9983a-125">Como o recurso **administrativeUnit** oferece suporte a [extensões](/graph/extensibility-overview), você pode `POST` usar a operação e adicionar propriedades personalizadas com seus próprios dados à unidade administrativa ao criá-la.</span><span class="sxs-lookup"><span data-stu-id="9983a-125">Since the **administrativeUnit** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the administrative unit while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="9983a-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="9983a-126">Response</span></span>

<span data-ttu-id="9983a-127">Se bem-sucedido, este método retorna `201 Created` o código de resposta e o objeto [administrativeUnit](../resources/administrativeunit.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9983a-127">If successful, this method returns `201 Created` response code and [administrativeUnit](../resources/administrativeunit.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9983a-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9983a-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9983a-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9983a-129">Request</span></span>
<span data-ttu-id="9983a-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9983a-130">Here is an example of the request.</span></span>
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
<span data-ttu-id="9983a-131">No corpo da solicitação, forneça uma representação JSON do objeto [administrativeUnit](../resources/administrativeunit.md) .</span><span class="sxs-lookup"><span data-stu-id="9983a-131">In the request body, supply a JSON representation of [administrativeUnit](../resources/administrativeunit.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="9983a-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="9983a-132">Response</span></span>
<span data-ttu-id="9983a-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9983a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="9983a-136">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="9983a-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="9983a-137">Basic</span><span class="sxs-lookup"><span data-stu-id="9983a-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_administrativeunit_from_administrativeunits-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9983a-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9983a-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_administrativeunit_from_administrativeunits-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="9983a-139">Confira também</span><span class="sxs-lookup"><span data-stu-id="9983a-139">See also</span></span>

- [<span data-ttu-id="9983a-140">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="9983a-140">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="9983a-141">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="9983a-141">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
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
    "Error: /api-reference/beta/api/administrativeunit-post-administrativeunits.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/administrativeunit-post-administrativeunits.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
