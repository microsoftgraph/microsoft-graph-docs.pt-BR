---
title: Listar proprietários
description: Recupere uma lista de proprietários (objetos directoryObject) para um aplicativo.
author: sureshja
localization_priority: Normal
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 29b90fba024d97ceecfd4fe72f37a72de6f7fb8a
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129198"
---
# <a name="list-owners"></a><span data-ttu-id="ed18b-103">Listar proprietários</span><span class="sxs-lookup"><span data-stu-id="ed18b-103">List owners</span></span>

<span data-ttu-id="ed18b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed18b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed18b-105">Recupere uma lista de proprietários de um aplicativo que são [objetos directoryObject.](../resources/directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="ed18b-105">Retrieve a list of owners for an application that are [directoryObject](../resources/directoryobject.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="ed18b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ed18b-106">Permissions</span></span>
<span data-ttu-id="ed18b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed18b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed18b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ed18b-109">Permission type</span></span>      | <span data-ttu-id="ed18b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ed18b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ed18b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ed18b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ed18b-112">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ed18b-112">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ed18b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ed18b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ed18b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ed18b-114">Not supported.</span></span>    |
|<span data-ttu-id="ed18b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ed18b-115">Application</span></span> | <span data-ttu-id="ed18b-116">Application.Read.All, Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed18b-116">Application.Read.All, Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="ed18b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ed18b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications/{id}/owners
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ed18b-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ed18b-118">Optional query parameters</span></span>
<span data-ttu-id="ed18b-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ed18b-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ed18b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ed18b-120">Request headers</span></span>
| <span data-ttu-id="ed18b-121">Nome</span><span class="sxs-lookup"><span data-stu-id="ed18b-121">Name</span></span>           | <span data-ttu-id="ed18b-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed18b-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="ed18b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ed18b-123">Authorization</span></span>  | <span data-ttu-id="ed18b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ed18b-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ed18b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ed18b-126">Request body</span></span>
<span data-ttu-id="ed18b-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ed18b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ed18b-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed18b-128">Response</span></span>

<span data-ttu-id="ed18b-129">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ed18b-129">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ed18b-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ed18b-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ed18b-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ed18b-131">Request</span></span>
<span data-ttu-id="ed18b-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ed18b-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ed18b-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="ed18b-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_get_owners"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/applications/{id}/owners
```
# <a name="c"></a>[<span data-ttu-id="ed18b-134">C#</span><span class="sxs-lookup"><span data-stu-id="ed18b-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/application-get-owners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ed18b-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ed18b-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-get-owners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ed18b-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ed18b-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-get-owners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ed18b-137">Java</span><span class="sxs-lookup"><span data-stu-id="ed18b-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/application-get-owners-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ed18b-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed18b-138">Response</span></span>
<span data-ttu-id="ed18b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ed18b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

