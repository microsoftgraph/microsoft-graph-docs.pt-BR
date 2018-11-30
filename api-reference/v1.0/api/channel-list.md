---
title: Canais de lista
description: Recupere a lista de canais nesse conjunto.
ms.openlocfilehash: 5f96d4c47a787839626a9d90733d087906407b01
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004890"
---
# <a name="list-channels"></a><span data-ttu-id="cb01b-103">Canais de lista</span><span class="sxs-lookup"><span data-stu-id="cb01b-103">List channels</span></span>



<span data-ttu-id="cb01b-104">Recupere a lista de [canais](../resources/channel.md) nesse conjunto.</span><span class="sxs-lookup"><span data-stu-id="cb01b-104">Retrieve the list of [channels](../resources/channel.md) in this team.</span></span>

## <a name="permissions"></a><span data-ttu-id="cb01b-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="cb01b-105">Permissions</span></span>
<span data-ttu-id="cb01b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb01b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="cb01b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cb01b-108">Permission type</span></span>      | <span data-ttu-id="cb01b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cb01b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cb01b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cb01b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cb01b-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb01b-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="cb01b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cb01b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cb01b-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cb01b-113">Not supported.</span></span>    |
|<span data-ttu-id="cb01b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cb01b-114">Application</span></span> | <span data-ttu-id="cb01b-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb01b-115">Group.Read.All, Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="cb01b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cb01b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cb01b-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="cb01b-117">Optional query parameters</span></span>
<span data-ttu-id="cb01b-118">Este método oferece suporte a $filter, $select, e $expand [OData parâmetros de consulta](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="cb01b-118">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cb01b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cb01b-119">Request headers</span></span>
| <span data-ttu-id="cb01b-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cb01b-120">Header</span></span>       | <span data-ttu-id="cb01b-121">Valor</span><span class="sxs-lookup"><span data-stu-id="cb01b-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cb01b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="cb01b-122">Authorization</span></span>  | <span data-ttu-id="cb01b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cb01b-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cb01b-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cb01b-125">Request body</span></span>
<span data-ttu-id="cb01b-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cb01b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cb01b-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb01b-127">Response</span></span>

<span data-ttu-id="cb01b-128">Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos de [canal](../resources/channel.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cb01b-128">If successful, this method returns a `200 OK` response code and collection of [Channel](../resources/channel.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb01b-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cb01b-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cb01b-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cb01b-130">Request</span></span>
<span data-ttu-id="cb01b-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cb01b-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channels"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels
```
##### <a name="response"></a><span data-ttu-id="cb01b-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb01b-132">Response</span></span>
<span data-ttu-id="cb01b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cb01b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 262

{
  "value": [
    {
      "description": "description-value",
      "displayName": "display-name-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List channels",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
