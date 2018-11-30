---
title: Lista workingWith
description: Percepção calculada para a lista de usuários que um usuário tiver trabalhado com.
ms.openlocfilehash: ce464667c66a430f20c60485712c649120dac4a5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034795"
---
# <a name="list-workingwith"></a><span data-ttu-id="59270-103">Lista workingWith</span><span class="sxs-lookup"><span data-stu-id="59270-103">List workingWith</span></span>

> <span data-ttu-id="59270-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="59270-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="59270-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="59270-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="59270-106">Percepção calculada para a lista de usuários que um usuário tiver trabalhado com.</span><span class="sxs-lookup"><span data-stu-id="59270-106">Calculated insight for the list of users that a user has been working with.</span></span>

## <a name="permissions"></a><span data-ttu-id="59270-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="59270-107">Permissions</span></span>
<span data-ttu-id="59270-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59270-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59270-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="59270-110">Permission type</span></span>      | <span data-ttu-id="59270-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="59270-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="59270-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="59270-112">Delegated (work or school account)</span></span> | <span data-ttu-id="59270-113">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="59270-113">User.Read.All</span></span>    |
|<span data-ttu-id="59270-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="59270-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59270-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="59270-115">Not supported.</span></span>    |
|<span data-ttu-id="59270-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="59270-116">Application</span></span> | <span data-ttu-id="59270-117">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="59270-117">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="59270-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="59270-118">HTTP request</span></span>
```http
GET /me/workingWith
GET /users/{id | userPrincipalName}/workingWith
GET /drive/root/createdByUser/workingWith
GET /drive/root/lastModifiedByUser/workingWith
```
## <a name="optional-query-parameters"></a><span data-ttu-id="59270-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="59270-119">Optional query parameters</span></span>
<span data-ttu-id="59270-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="59270-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="59270-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="59270-121">Request headers</span></span>
| <span data-ttu-id="59270-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="59270-122">Header</span></span>         | <span data-ttu-id="59270-123">Valor</span><span class="sxs-lookup"><span data-stu-id="59270-123">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="59270-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="59270-124">Authorization</span></span>  | <span data-ttu-id="59270-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59270-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="59270-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="59270-127">Content-Type</span></span>   | <span data-ttu-id="59270-128">application/json</span><span class="sxs-lookup"><span data-stu-id="59270-128">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="59270-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="59270-129">Request body</span></span>
<span data-ttu-id="59270-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="59270-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="59270-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="59270-131">Response</span></span>

<span data-ttu-id="59270-132">Se tiver êxito, esse método retorna um código de resposta Okey 200 e um conjunto de objetos de [usuário](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="59270-132">If successful, this method returns a 200 OK response code and collection of [User](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59270-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="59270-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="59270-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="59270-134">Request</span></span>
```http
GET https://graph.microsoft.com/beta/me/workingWith
```
##### <a name="response"></a><span data-ttu-id="59270-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="59270-135">Response</span></span>
<span data-ttu-id="59270-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="59270-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
