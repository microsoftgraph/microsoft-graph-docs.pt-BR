---
title: Obter serviços
description: Recupere uma lista de objetos de reserviço que representam os serviços disponíveis para seu locatário.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: cbe0735e884e1314dcb4ac62c0cb719ab9592e52
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895590"
---
# <a name="list-services"></a><span data-ttu-id="78ecd-103">Listar serviços</span><span class="sxs-lookup"><span data-stu-id="78ecd-103">List services</span></span>

<span data-ttu-id="78ecd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78ecd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78ecd-105">Recupere uma lista de objetos de [reserviço](../resources/printservice.md) que representam os **Serviços** disponíveis para seu locatário.</span><span class="sxs-lookup"><span data-stu-id="78ecd-105">Retrieve a list of [printService](../resources/printservice.md) objects that represent the **services** available to your tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="78ecd-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="78ecd-106">Permissions</span></span>
<span data-ttu-id="78ecd-107">Nenhuma permissão é necessária para chamar essa API, mas o locatário do usuário deve ter uma assinatura de impressão universal ativa.</span><span class="sxs-lookup"><span data-stu-id="78ecd-107">No permissions are needed to call this API, but the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="78ecd-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="78ecd-108">Permission type</span></span> | <span data-ttu-id="78ecd-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="78ecd-109">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="78ecd-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="78ecd-110">Delegated (work or school account)</span></span>|<span data-ttu-id="78ecd-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="78ecd-111">None.</span></span>|
|<span data-ttu-id="78ecd-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="78ecd-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="78ecd-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="78ecd-113">None.</span></span>|
|<span data-ttu-id="78ecd-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="78ecd-114">Application</span></span>|<span data-ttu-id="78ecd-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="78ecd-115">None.</span></span>|

## <a name="http-request"></a><span data-ttu-id="78ecd-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="78ecd-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/services
```

## <a name="optional-query-parameters"></a><span data-ttu-id="78ecd-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="78ecd-117">Optional query parameters</span></span>
<span data-ttu-id="78ecd-118">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="78ecd-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="78ecd-119">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="78ecd-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="78ecd-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="78ecd-120">Request headers</span></span>
| <span data-ttu-id="78ecd-121">Nome</span><span class="sxs-lookup"><span data-stu-id="78ecd-121">Name</span></span>      |<span data-ttu-id="78ecd-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="78ecd-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="78ecd-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="78ecd-123">Authorization</span></span> | <span data-ttu-id="78ecd-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="78ecd-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="78ecd-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="78ecd-126">Request body</span></span>
<span data-ttu-id="78ecd-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="78ecd-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="78ecd-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="78ecd-128">Response</span></span>
<span data-ttu-id="78ecd-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos de [reserviço](../resources/printservice.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="78ecd-129">If successful, this method returns a `200 OK` response code and a collection of [printService](../resources/printservice.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="78ecd-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="78ecd-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="78ecd-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="78ecd-131">Request</span></span>
<span data-ttu-id="78ecd-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="78ecd-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_services"
}-->
```http
GET https://graph.microsoft.com/beta/print/services
```
##### <a name="response"></a><span data-ttu-id="78ecd-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="78ecd-133">Response</span></span>
<span data-ttu-id="78ecd-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="78ecd-134">The following is an example of the response.</span></span>
><span data-ttu-id="78ecd-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="78ecd-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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