---
title: Obter administrativeUnit
description: Recupere as propriedades e os relacionamentos de um objeto administrativeUnit.
author: anandyadavMSFT
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1cbae5fa7516b84dd1cdfad8d59d4ff1066e5634
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/30/2020
ms.locfileid: "48312663"
---
# <a name="get-administrativeunit"></a><span data-ttu-id="e0e75-103">Obter administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="e0e75-103">Get administrativeUnit</span></span>

<span data-ttu-id="e0e75-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0e75-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0e75-105">Recupere as propriedades e os relacionamentos de um objeto [administrativeUnit](../resources/administrativeunit.md) .</span><span class="sxs-lookup"><span data-stu-id="e0e75-105">Retrieve the properties and relationships of an [administrativeUnit](../resources/administrativeunit.md) object.</span></span>

<span data-ttu-id="e0e75-106">Como o recurso **administrativeUnit** oferece suporte a [extensões](/graph/extensibility-overview), você também pode usar a `GET` operação para obter propriedades personalizadas e dados de extensão em uma instância do **administrativeUnit** .</span><span class="sxs-lookup"><span data-stu-id="e0e75-106">Since the **administrativeUnit** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in an **administrativeUnit** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="e0e75-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="e0e75-107">Permissions</span></span>
<span data-ttu-id="e0e75-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0e75-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e0e75-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e0e75-110">Permission type</span></span>      | <span data-ttu-id="e0e75-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e0e75-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e0e75-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e0e75-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e0e75-113">AdministrativeUnit. Read. All, Directory. Read. All, AdministrativeUnit. ReadWrite. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="e0e75-113">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e0e75-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e0e75-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0e75-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e0e75-115">Not supported.</span></span>    |
|<span data-ttu-id="e0e75-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e0e75-116">Application</span></span> | <span data-ttu-id="e0e75-117">AdministrativeUnit. Read. All, Directory. Read. All, AdministrativeUnit. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="e0e75-117">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e0e75-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e0e75-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /administrativeUnits/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e0e75-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e0e75-119">Optional query parameters</span></span>
<span data-ttu-id="e0e75-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e0e75-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e0e75-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e0e75-121">Request headers</span></span>
| <span data-ttu-id="e0e75-122">Nome</span><span class="sxs-lookup"><span data-stu-id="e0e75-122">Name</span></span>      |<span data-ttu-id="e0e75-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0e75-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e0e75-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="e0e75-124">Authorization</span></span>  | <span data-ttu-id="e0e75-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e0e75-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e0e75-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e0e75-127">Request body</span></span>
<span data-ttu-id="e0e75-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e0e75-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e0e75-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0e75-129">Response</span></span>

<span data-ttu-id="e0e75-130">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [administrativeUnit](../resources/administrativeunit.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e0e75-130">If successful, this method returns a `200 OK` response code and [administrativeUnit](../resources/administrativeunit.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e0e75-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e0e75-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e0e75-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e0e75-132">Request</span></span>
<span data-ttu-id="e0e75-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e0e75-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e0e75-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="e0e75-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_administrativeunit"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/administrativeUnits/{id}
```
# <a name="c"></a>[<span data-ttu-id="e0e75-135">C#</span><span class="sxs-lookup"><span data-stu-id="e0e75-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-administrativeunit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e0e75-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e0e75-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-administrativeunit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e0e75-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e0e75-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-administrativeunit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e0e75-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0e75-138">Response</span></span>
<span data-ttu-id="e0e75-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e0e75-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="e0e75-142">Confira também</span><span class="sxs-lookup"><span data-stu-id="e0e75-142">See also</span></span>

- [<span data-ttu-id="e0e75-143">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="e0e75-143">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="e0e75-144">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="e0e75-144">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
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