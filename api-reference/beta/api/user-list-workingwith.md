---
title: Listar workingWith
description: Informações calculadas para a lista de usuários com os quais um usuário está trabalhando.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 587a9e34db293a738e1242b3d41406bb15990834
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35987478"
---
# <a name="list-workingwith"></a><span data-ttu-id="4bfab-103">Listar workingWith</span><span class="sxs-lookup"><span data-stu-id="4bfab-103">List workingWith</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4bfab-104">Informações calculadas para a lista de usuários com os quais um usuário está trabalhando.</span><span class="sxs-lookup"><span data-stu-id="4bfab-104">Calculated insight for the list of users that a user has been working with.</span></span>

## <a name="permissions"></a><span data-ttu-id="4bfab-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="4bfab-105">Permissions</span></span>
<span data-ttu-id="4bfab-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4bfab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4bfab-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4bfab-108">Permission type</span></span>      | <span data-ttu-id="4bfab-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4bfab-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4bfab-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4bfab-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4bfab-111">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="4bfab-111">User.Read.All</span></span>    |
|<span data-ttu-id="4bfab-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4bfab-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4bfab-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4bfab-113">Not supported.</span></span>    |
|<span data-ttu-id="4bfab-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4bfab-114">Application</span></span> | <span data-ttu-id="4bfab-115">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="4bfab-115">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4bfab-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4bfab-116">HTTP request</span></span>
```http
GET /me/workingWith
GET /users/{id | userPrincipalName}/workingWith
GET /drive/root/createdByUser/workingWith
GET /drive/root/lastModifiedByUser/workingWith
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4bfab-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4bfab-117">Optional query parameters</span></span>
<span data-ttu-id="4bfab-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4bfab-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4bfab-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4bfab-119">Request headers</span></span>
| <span data-ttu-id="4bfab-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4bfab-120">Header</span></span>         | <span data-ttu-id="4bfab-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4bfab-121">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="4bfab-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4bfab-122">Authorization</span></span>  | <span data-ttu-id="4bfab-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4bfab-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4bfab-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4bfab-125">Content-Type</span></span>   | <span data-ttu-id="4bfab-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4bfab-126">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="4bfab-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4bfab-127">Request body</span></span>
<span data-ttu-id="4bfab-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4bfab-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4bfab-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="4bfab-129">Response</span></span>

<span data-ttu-id="4bfab-130">Se bem-sucedido, este método retorna um código de resposta de OK 200 e uma coleção de objetos [User](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4bfab-130">If successful, this method returns a 200 OK response code and collection of [User](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4bfab-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4bfab-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4bfab-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4bfab-132">Request</span></span>
```http
GET https://graph.microsoft.com/beta/me/workingWith
```
##### <a name="response"></a><span data-ttu-id="4bfab-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="4bfab-133">Response</span></span>
<span data-ttu-id="4bfab-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4bfab-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
