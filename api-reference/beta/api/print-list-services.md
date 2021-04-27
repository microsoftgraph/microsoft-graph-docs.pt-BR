---
title: Listar printServices
description: Recupere uma lista de objetos printService que representam os serviços disponíveis para seu locatário.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 3461665b6d027fdba0ecd88e97af422b4f3865ff
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051092"
---
# <a name="list-printservices"></a><span data-ttu-id="bc81d-103">Listar printServices</span><span class="sxs-lookup"><span data-stu-id="bc81d-103">List printServices</span></span>

<span data-ttu-id="bc81d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bc81d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bc81d-105">Recupere uma lista de [objetos printService](../resources/printservice.md) que representam os **serviços** disponíveis para seu locatário.</span><span class="sxs-lookup"><span data-stu-id="bc81d-105">Retrieve a list of [printService](../resources/printservice.md) objects that represent the **services** available to your tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="bc81d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="bc81d-106">Permissions</span></span>
<span data-ttu-id="bc81d-107">Nenhuma permissão é necessária para chamar essa API, mas para usar o serviço de Impressão Universal, o usuário ou locatário do aplicativo deve ter uma assinatura universal ativa.</span><span class="sxs-lookup"><span data-stu-id="bc81d-107">No permissions are needed to call this API, but to use the Universal Print service, the user or app's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="bc81d-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bc81d-108">Permission type</span></span> | <span data-ttu-id="bc81d-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bc81d-109">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="bc81d-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bc81d-110">Delegated (work or school account)</span></span>|<span data-ttu-id="bc81d-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bc81d-111">None.</span></span>|
|<span data-ttu-id="bc81d-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bc81d-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bc81d-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="bc81d-113">None.</span></span>|
|<span data-ttu-id="bc81d-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bc81d-114">Application</span></span>|<span data-ttu-id="bc81d-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bc81d-115">None.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bc81d-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bc81d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/services
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bc81d-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="bc81d-117">Optional query parameters</span></span>
<span data-ttu-id="bc81d-118">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="bc81d-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="bc81d-119">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="bc81d-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="bc81d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bc81d-120">Request headers</span></span>
| <span data-ttu-id="bc81d-121">Nome</span><span class="sxs-lookup"><span data-stu-id="bc81d-121">Name</span></span>      |<span data-ttu-id="bc81d-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc81d-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bc81d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="bc81d-123">Authorization</span></span> | <span data-ttu-id="bc81d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bc81d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bc81d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bc81d-126">Request body</span></span>
<span data-ttu-id="bc81d-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bc81d-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="bc81d-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc81d-128">Response</span></span>
<span data-ttu-id="bc81d-129">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos printService](../resources/printservice.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bc81d-129">If successful, this method returns a `200 OK` response code and a collection of [printService](../resources/printservice.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bc81d-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bc81d-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bc81d-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bc81d-131">Request</span></span>
<span data-ttu-id="bc81d-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bc81d-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bc81d-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="bc81d-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_services_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/services
```
# <a name="c"></a>[<span data-ttu-id="bc81d-134">C#</span><span class="sxs-lookup"><span data-stu-id="bc81d-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-services-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bc81d-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bc81d-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-services-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bc81d-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bc81d-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-services-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bc81d-137">Java</span><span class="sxs-lookup"><span data-stu-id="bc81d-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-services-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="bc81d-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc81d-138">Response</span></span>
<span data-ttu-id="bc81d-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bc81d-139">The following is an example of the response.</span></span>
><span data-ttu-id="bc81d-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="bc81d-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printService",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 389

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/services",
  "value": [
    {
      "id": "f4cfee8b-4117-4773-a2f0-3807beb282b9",
      "endpoints": [
        {
          "id": "mpsdiscovery",
          "displayName": "Microsoft Universal Print Discovery Service",
          "uri": "https://discovery.print.microsoft.com"
        }
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List services",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


