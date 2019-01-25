---
title: Lista workingWith
description: Percepção calculada para a lista de usuários que um usuário tiver trabalhado com.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ca5fdd4602d109d98002c0ef54fde5ad341e1903
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521618"
---
# <a name="list-workingwith"></a><span data-ttu-id="923e9-103">Lista workingWith</span><span class="sxs-lookup"><span data-stu-id="923e9-103">List workingWith</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="923e9-104">Percepção calculada para a lista de usuários que um usuário tiver trabalhado com.</span><span class="sxs-lookup"><span data-stu-id="923e9-104">Calculated insight for the list of users that a user has been working with.</span></span>

## <a name="permissions"></a><span data-ttu-id="923e9-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="923e9-105">Permissions</span></span>
<span data-ttu-id="923e9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="923e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="923e9-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="923e9-108">Permission type</span></span>      | <span data-ttu-id="923e9-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="923e9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="923e9-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="923e9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="923e9-111">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="923e9-111">User.Read.All</span></span>    |
|<span data-ttu-id="923e9-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="923e9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="923e9-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="923e9-113">Not supported.</span></span>    |
|<span data-ttu-id="923e9-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="923e9-114">Application</span></span> | <span data-ttu-id="923e9-115">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="923e9-115">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="923e9-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="923e9-116">HTTP request</span></span>
```http
GET /me/workingWith
GET /users/{id | userPrincipalName}/workingWith
GET /drive/root/createdByUser/workingWith
GET /drive/root/lastModifiedByUser/workingWith
```
## <a name="optional-query-parameters"></a><span data-ttu-id="923e9-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="923e9-117">Optional query parameters</span></span>
<span data-ttu-id="923e9-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="923e9-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="923e9-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="923e9-119">Request headers</span></span>
| <span data-ttu-id="923e9-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="923e9-120">Header</span></span>         | <span data-ttu-id="923e9-121">Valor</span><span class="sxs-lookup"><span data-stu-id="923e9-121">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="923e9-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="923e9-122">Authorization</span></span>  | <span data-ttu-id="923e9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="923e9-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="923e9-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="923e9-125">Content-Type</span></span>   | <span data-ttu-id="923e9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="923e9-126">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="923e9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="923e9-127">Request body</span></span>
<span data-ttu-id="923e9-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="923e9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="923e9-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="923e9-129">Response</span></span>

<span data-ttu-id="923e9-130">Se tiver êxito, esse método retorna um código de resposta Okey 200 e um conjunto de objetos de [usuário](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="923e9-130">If successful, this method returns a 200 OK response code and collection of [User](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="923e9-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="923e9-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="923e9-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="923e9-132">Request</span></span>
```http
GET https://graph.microsoft.com/beta/me/workingWith
```
##### <a name="response"></a><span data-ttu-id="923e9-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="923e9-133">Response</span></span>
<span data-ttu-id="923e9-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="923e9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list-workingwith.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
