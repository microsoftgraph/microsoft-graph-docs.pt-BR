---
title: Lista trendingAround
description: Percepção calculada que retorna a lista de itens de tendências em torno de um usuário.
author: dkershaw10
ms.openlocfilehash: 2f2595cbaacc74053b23d6b26b64fb9a17e2924a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27333828"
---
# <a name="list-trendingaround"></a><span data-ttu-id="f586d-103">Lista trendingAround</span><span class="sxs-lookup"><span data-stu-id="f586d-103">List trendingAround</span></span>

> <span data-ttu-id="f586d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f586d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f586d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f586d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f586d-106">Percepção calculada que retorna a lista de itens de tendências em torno de um usuário.</span><span class="sxs-lookup"><span data-stu-id="f586d-106">Calculated insight that returns the list of items trending around a user.</span></span>

<span data-ttu-id="f586d-107">**Observação:** Essa API será preterida e substituída pela [API de tendências](../resources/insights-trending.md).</span><span class="sxs-lookup"><span data-stu-id="f586d-107">**Note:** This API will be deprecated and replaced by the [Trending API](../resources/insights-trending.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f586d-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="f586d-108">Permissions</span></span>
<span data-ttu-id="f586d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f586d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f586d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f586d-111">Permission type</span></span>      | <span data-ttu-id="f586d-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f586d-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f586d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f586d-113">Delegated (work or school account)</span></span> | <span data-ttu-id="f586d-114">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="f586d-114">Sites.Read.All</span></span>    |
|<span data-ttu-id="f586d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f586d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f586d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f586d-116">Not supported.</span></span>    |
|<span data-ttu-id="f586d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f586d-117">Application</span></span> | <span data-ttu-id="f586d-118">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="f586d-118">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f586d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f586d-119">HTTP request</span></span>
```http
GET /me/trendingAround
GET /users/{id | userPrincipalName}/trendingAround
GET /drive/root/createdByUser/trendingAround
GET /drive/root/lastModifiedByUser/trendingAround
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f586d-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f586d-120">Optional query parameters</span></span>
<span data-ttu-id="f586d-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f586d-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f586d-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f586d-122">Request headers</span></span>
| <span data-ttu-id="f586d-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f586d-123">Header</span></span>         | <span data-ttu-id="f586d-124">Valor</span><span class="sxs-lookup"><span data-stu-id="f586d-124">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="f586d-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="f586d-125">Authorization</span></span>  | <span data-ttu-id="f586d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f586d-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f586d-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f586d-128">Content-Type</span></span>   | <span data-ttu-id="f586d-129">application/json</span><span class="sxs-lookup"><span data-stu-id="f586d-129">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="f586d-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f586d-130">Request body</span></span>
<span data-ttu-id="f586d-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f586d-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f586d-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="f586d-132">Response</span></span>

<span data-ttu-id="f586d-133">Se tiver êxito, esse método retorna um código de resposta Okey 200 e a coleção de objetos [driveItem](../resources/driveitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f586d-133">If successful, this method returns a 200 OK response code and collection of [driveItem](../resources/driveitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f586d-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f586d-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f586d-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f586d-135">Request</span></span>
```http
GET https://graph.microsoft.com/beta/me/trendingAround
```
##### <a name="response"></a><span data-ttu-id="f586d-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="f586d-136">Response</span></span>
<span data-ttu-id="f586d-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f586d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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