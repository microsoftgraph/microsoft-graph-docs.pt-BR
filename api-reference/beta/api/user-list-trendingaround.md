---
title: Listar tendênciasAround
description: Insight calculado que retorna a lista de itens que estão na tendência em torno de um usuário.
author: jpettere
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 139416e3b21166f50e2f9fed529a7efe6b4dbd3e
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720673"
---
# <a name="list-trendingaround"></a><span data-ttu-id="5136b-103">Listar tendênciasAround</span><span class="sxs-lookup"><span data-stu-id="5136b-103">List trendingAround</span></span>

<span data-ttu-id="5136b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5136b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5136b-105">Insight calculado que retorna a lista de itens que estão na tendência em torno de um usuário.</span><span class="sxs-lookup"><span data-stu-id="5136b-105">Calculated insight that returns the list of items trending around a user.</span></span>

<span data-ttu-id="5136b-106">**Observação:** Essa API será preterida e substituída pela [API de Tendência.](../resources/insights-trending.md)</span><span class="sxs-lookup"><span data-stu-id="5136b-106">**Note:** This API will be deprecated and replaced by the [Trending API](../resources/insights-trending.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5136b-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="5136b-107">Permissions</span></span>
<span data-ttu-id="5136b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5136b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5136b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5136b-110">Permission type</span></span>      | <span data-ttu-id="5136b-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5136b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5136b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5136b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5136b-113">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="5136b-113">Sites.Read.All</span></span>    |
|<span data-ttu-id="5136b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5136b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5136b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5136b-115">Not supported.</span></span>    |
|<span data-ttu-id="5136b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5136b-116">Application</span></span> | <span data-ttu-id="5136b-117">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="5136b-117">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5136b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5136b-118">HTTP request</span></span>
```http
GET /me/trendingAround
GET /users/{id | userPrincipalName}/trendingAround
GET /drive/root/createdByUser/trendingAround
GET /drive/root/lastModifiedByUser/trendingAround
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5136b-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5136b-119">Optional query parameters</span></span>
<span data-ttu-id="5136b-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5136b-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5136b-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5136b-121">Request headers</span></span>
| <span data-ttu-id="5136b-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5136b-122">Header</span></span>         | <span data-ttu-id="5136b-123">Valor</span><span class="sxs-lookup"><span data-stu-id="5136b-123">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="5136b-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="5136b-124">Authorization</span></span>  | <span data-ttu-id="5136b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5136b-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5136b-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5136b-127">Content-Type</span></span>   | <span data-ttu-id="5136b-128">application/json</span><span class="sxs-lookup"><span data-stu-id="5136b-128">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="5136b-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5136b-129">Request body</span></span>
<span data-ttu-id="5136b-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5136b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5136b-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="5136b-131">Response</span></span>

<span data-ttu-id="5136b-132">Se tiver êxito, este método retornará um código de resposta 200 OK e uma coleção de [objetos driveItem](../resources/driveitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5136b-132">If successful, this method returns a 200 OK response code and collection of [driveItem](../resources/driveitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5136b-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5136b-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5136b-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5136b-134">Request</span></span>
```http
GET https://graph.microsoft.com/beta/me/trendingAround
```
##### <a name="response"></a><span data-ttu-id="5136b-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="5136b-135">Response</span></span>
<span data-ttu-id="5136b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5136b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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