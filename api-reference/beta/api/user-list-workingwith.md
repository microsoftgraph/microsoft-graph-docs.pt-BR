---
title: Listar workingWith
description: Informações calculadas para a lista de usuários com os quais um usuário está trabalhando.
author: krbain
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 806aa9e1f6a95d5f1d723714869546ea3943c725
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2020
ms.locfileid: "43107532"
---
# <a name="list-workingwith"></a><span data-ttu-id="dc7d5-103">Listar workingWith</span><span class="sxs-lookup"><span data-stu-id="dc7d5-103">List workingWith</span></span>

<span data-ttu-id="dc7d5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc7d5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc7d5-105">Informações calculadas para a lista de usuários com os quais um usuário está trabalhando.</span><span class="sxs-lookup"><span data-stu-id="dc7d5-105">Calculated insight for the list of users that a user has been working with.</span></span>

## <a name="permissions"></a><span data-ttu-id="dc7d5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="dc7d5-106">Permissions</span></span>
<span data-ttu-id="dc7d5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc7d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc7d5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dc7d5-109">Permission type</span></span>      | <span data-ttu-id="dc7d5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dc7d5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dc7d5-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dc7d5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="dc7d5-112">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="dc7d5-112">User.Read.All</span></span>    |
|<span data-ttu-id="dc7d5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dc7d5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dc7d5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dc7d5-114">Not supported.</span></span>    |
|<span data-ttu-id="dc7d5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dc7d5-115">Application</span></span> | <span data-ttu-id="dc7d5-116">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="dc7d5-116">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dc7d5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dc7d5-117">HTTP request</span></span>
```http
GET /me/workingWith
GET /users/{id | userPrincipalName}/workingWith
GET /drive/root/createdByUser/workingWith
GET /drive/root/lastModifiedByUser/workingWith
```
## <a name="optional-query-parameters"></a><span data-ttu-id="dc7d5-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="dc7d5-118">Optional query parameters</span></span>
<span data-ttu-id="dc7d5-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="dc7d5-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dc7d5-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dc7d5-120">Request headers</span></span>
| <span data-ttu-id="dc7d5-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dc7d5-121">Header</span></span>         | <span data-ttu-id="dc7d5-122">Valor</span><span class="sxs-lookup"><span data-stu-id="dc7d5-122">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="dc7d5-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="dc7d5-123">Authorization</span></span>  | <span data-ttu-id="dc7d5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dc7d5-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="dc7d5-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dc7d5-126">Content-Type</span></span>   | <span data-ttu-id="dc7d5-127">application/json</span><span class="sxs-lookup"><span data-stu-id="dc7d5-127">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="dc7d5-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dc7d5-128">Request body</span></span>
<span data-ttu-id="dc7d5-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dc7d5-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dc7d5-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc7d5-130">Response</span></span>

<span data-ttu-id="dc7d5-131">Se bem-sucedido, este método retorna um código de resposta de OK 200 e uma coleção de objetos [User](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dc7d5-131">If successful, this method returns a 200 OK response code and collection of [User](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc7d5-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dc7d5-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dc7d5-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dc7d5-133">Request</span></span>
```http
GET https://graph.microsoft.com/beta/me/workingWith
```
##### <a name="response"></a><span data-ttu-id="dc7d5-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc7d5-134">Response</span></span>
<span data-ttu-id="dc7d5-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dc7d5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 98

{
  "id": "id-value",
  "preferredName": "preferredName-value",
  "Email": "Email-value",
}
```
