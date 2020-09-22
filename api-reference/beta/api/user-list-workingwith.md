---
title: Listar workingWith
description: Informações calculadas para a lista de usuários com os quais um usuário está trabalhando.
author: krbain
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: ce7c0e915105ff837c1a96185610553123fc82c6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48024700"
---
# <a name="list-workingwith"></a><span data-ttu-id="291b3-103">Listar workingWith</span><span class="sxs-lookup"><span data-stu-id="291b3-103">List workingWith</span></span>

<span data-ttu-id="291b3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="291b3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="291b3-105">Informações calculadas para a lista de usuários com os quais um usuário está trabalhando.</span><span class="sxs-lookup"><span data-stu-id="291b3-105">Calculated insight for the list of users that a user has been working with.</span></span>

## <a name="permissions"></a><span data-ttu-id="291b3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="291b3-106">Permissions</span></span>
<span data-ttu-id="291b3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="291b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="291b3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="291b3-109">Permission type</span></span>      | <span data-ttu-id="291b3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="291b3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="291b3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="291b3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="291b3-112">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="291b3-112">User.Read.All</span></span>    |
|<span data-ttu-id="291b3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="291b3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="291b3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="291b3-114">Not supported.</span></span>    |
|<span data-ttu-id="291b3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="291b3-115">Application</span></span> | <span data-ttu-id="291b3-116">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="291b3-116">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="291b3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="291b3-117">HTTP request</span></span>
```http
GET /me/workingWith
GET /users/{id | userPrincipalName}/workingWith
GET /drive/root/createdByUser/workingWith
GET /drive/root/lastModifiedByUser/workingWith
```
## <a name="optional-query-parameters"></a><span data-ttu-id="291b3-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="291b3-118">Optional query parameters</span></span>
<span data-ttu-id="291b3-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="291b3-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="291b3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="291b3-120">Request headers</span></span>
| <span data-ttu-id="291b3-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="291b3-121">Header</span></span>         | <span data-ttu-id="291b3-122">Valor</span><span class="sxs-lookup"><span data-stu-id="291b3-122">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="291b3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="291b3-123">Authorization</span></span>  | <span data-ttu-id="291b3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="291b3-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="291b3-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="291b3-126">Content-Type</span></span>   | <span data-ttu-id="291b3-127">application/json</span><span class="sxs-lookup"><span data-stu-id="291b3-127">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="291b3-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="291b3-128">Request body</span></span>
<span data-ttu-id="291b3-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="291b3-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="291b3-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="291b3-130">Response</span></span>

<span data-ttu-id="291b3-131">Se bem-sucedido, este método retorna um código de resposta de OK 200 e uma coleção de objetos [User](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="291b3-131">If successful, this method returns a 200 OK response code and collection of [User](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="291b3-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="291b3-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="291b3-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="291b3-133">Request</span></span>
```http
GET https://graph.microsoft.com/beta/me/workingWith
```
##### <a name="response"></a><span data-ttu-id="291b3-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="291b3-134">Response</span></span>
<span data-ttu-id="291b3-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="291b3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


