---
title: Obtenha o canal
description: Recupere as propriedades e relacionamentos de um canal.
ms.openlocfilehash: 977484c57d7d82d13b781f658bb53eea091e2066
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037786"
---
# <a name="get-channel"></a><span data-ttu-id="4a2f4-103">Obtenha o canal</span><span class="sxs-lookup"><span data-stu-id="4a2f4-103">Get channel</span></span>

> <span data-ttu-id="4a2f4-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4a2f4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4a2f4-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4a2f4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4a2f4-106">Recupere as propriedades e relacionamentos de um [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="4a2f4-106">Retrieve the properties and relationships of a [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4a2f4-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="4a2f4-107">Permissions</span></span>
<span data-ttu-id="4a2f4-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a2f4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a2f4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4a2f4-110">Permission type</span></span>      | <span data-ttu-id="4a2f4-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4a2f4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4a2f4-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4a2f4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4a2f4-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a2f4-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4a2f4-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4a2f4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a2f4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4a2f4-115">Not supported.</span></span>    |
|<span data-ttu-id="4a2f4-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4a2f4-116">Application</span></span> | <span data-ttu-id="4a2f4-117">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a2f4-117">Group.Read.All, Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="4a2f4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4a2f4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}

```

## <a name="optional-query-parameters"></a><span data-ttu-id="4a2f4-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4a2f4-119">Optional query parameters</span></span>

<span data-ttu-id="4a2f4-120">Este método oferece suporte a $filter, $select, e $expand [OData parâmetros de consulta](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4a2f4-120">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4a2f4-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4a2f4-121">Request headers</span></span>
| <span data-ttu-id="4a2f4-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4a2f4-122">Header</span></span>       | <span data-ttu-id="4a2f4-123">Valor</span><span class="sxs-lookup"><span data-stu-id="4a2f4-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4a2f4-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="4a2f4-124">Authorization</span></span>  | <span data-ttu-id="4a2f4-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4a2f4-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4a2f4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4a2f4-127">Request body</span></span>
<span data-ttu-id="4a2f4-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4a2f4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4a2f4-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a2f4-129">Response</span></span>

<span data-ttu-id="4a2f4-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto de [canal](../resources/channel.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4a2f4-130">If successful, this method returns a `200 OK` response code and a [channel](../resources/channel.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4a2f4-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4a2f4-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4a2f4-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4a2f4-132">Request</span></span>
<span data-ttu-id="4a2f4-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4a2f4-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channel"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```
##### <a name="response"></a><span data-ttu-id="4a2f4-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a2f4-134">Response</span></span>
<span data-ttu-id="4a2f4-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4a2f4-135">Here is an example of the response.</span></span> 

><span data-ttu-id="4a2f4-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4a2f4-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
    "description": "description-value",
    "displayName": "display-name-value",
    "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
