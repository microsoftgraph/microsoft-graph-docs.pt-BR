---
title: Listar trendingAround
description: Informações calculadas que retornam a lista de itens que se referem a um usuário.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: dc7b6176fe4fceeeeea78d63c6b7140568ff6875
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35996186"
---
# <a name="list-trendingaround"></a><span data-ttu-id="c1cf0-103">Listar trendingAround</span><span class="sxs-lookup"><span data-stu-id="c1cf0-103">List trendingAround</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1cf0-104">Informações calculadas que retornam a lista de itens que se referem a um usuário.</span><span class="sxs-lookup"><span data-stu-id="c1cf0-104">Calculated insight that returns the list of items trending around a user.</span></span>

<span data-ttu-id="c1cf0-105">**Observação:** Essa API será preterida e substituída pela [API de tendência](../resources/insights-trending.md).</span><span class="sxs-lookup"><span data-stu-id="c1cf0-105">**Note:** This API will be deprecated and replaced by the [Trending API](../resources/insights-trending.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c1cf0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c1cf0-106">Permissions</span></span>
<span data-ttu-id="c1cf0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1cf0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1cf0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c1cf0-109">Permission type</span></span>      | <span data-ttu-id="c1cf0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c1cf0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c1cf0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c1cf0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c1cf0-112">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1cf0-112">Sites.Read.All</span></span>    |
|<span data-ttu-id="c1cf0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c1cf0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c1cf0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c1cf0-114">Not supported.</span></span>    |
|<span data-ttu-id="c1cf0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c1cf0-115">Application</span></span> | <span data-ttu-id="c1cf0-116">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1cf0-116">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c1cf0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c1cf0-117">HTTP request</span></span>
```http
GET /me/trendingAround
GET /users/{id | userPrincipalName}/trendingAround
GET /drive/root/createdByUser/trendingAround
GET /drive/root/lastModifiedByUser/trendingAround
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c1cf0-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c1cf0-118">Optional query parameters</span></span>
<span data-ttu-id="c1cf0-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c1cf0-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c1cf0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c1cf0-120">Request headers</span></span>
| <span data-ttu-id="c1cf0-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c1cf0-121">Header</span></span>         | <span data-ttu-id="c1cf0-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c1cf0-122">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="c1cf0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c1cf0-123">Authorization</span></span>  | <span data-ttu-id="c1cf0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c1cf0-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c1cf0-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c1cf0-126">Content-Type</span></span>   | <span data-ttu-id="c1cf0-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c1cf0-127">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="c1cf0-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c1cf0-128">Request body</span></span>
<span data-ttu-id="c1cf0-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c1cf0-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c1cf0-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="c1cf0-130">Response</span></span>

<span data-ttu-id="c1cf0-131">Se bem-sucedido, este método retorna um código de resposta de OK 200 e uma coleção de objetos [driveItem](../resources/driveitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c1cf0-131">If successful, this method returns a 200 OK response code and collection of [driveItem](../resources/driveitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1cf0-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c1cf0-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c1cf0-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c1cf0-133">Request</span></span>
```http
GET https://graph.microsoft.com/beta/me/trendingAround
```
##### <a name="response"></a><span data-ttu-id="c1cf0-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="c1cf0-134">Response</span></span>
<span data-ttu-id="c1cf0-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c1cf0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 226

{
  "id": "id-value",
  "name": "name-value",
  "DateTimeCreated": "DateTimeCreated-value",
  "DateTimeLastModified": "DateTimeLastModified-value",
  "webUrl": "webUrl-value",
}
```
