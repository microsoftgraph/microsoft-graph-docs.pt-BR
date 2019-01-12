---
title: Listar directReports
description: Obtenha relatórios diretos do usuário. Retorna os usuários e contatos para quem este usuário está atribuído como gerente.
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a397e45675b245325d1a086e0b87117358514e15
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984098"
---
# <a name="list-directreports"></a><span data-ttu-id="4544e-104">Listar directReports</span><span class="sxs-lookup"><span data-stu-id="4544e-104">List directReports</span></span>

<span data-ttu-id="4544e-p102">Obtenha relatórios diretos do usuário. Retorna os usuários e contatos para quem este usuário está atribuído como gerente.</span><span class="sxs-lookup"><span data-stu-id="4544e-p102">Get user's direct reports. Returns the users and contacts for whom this user is assigned as manager.</span></span>
## <a name="permissions"></a><span data-ttu-id="4544e-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="4544e-107">Permissions</span></span>
<span data-ttu-id="4544e-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4544e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4544e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4544e-110">Permission type</span></span>      | <span data-ttu-id="4544e-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4544e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4544e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4544e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4544e-113">User.Read, User.ReadWrite, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4544e-113">User.Read, User.ReadWrite, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4544e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4544e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4544e-115">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4544e-115">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="4544e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4544e-116">Application</span></span> | <span data-ttu-id="4544e-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4544e-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4544e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4544e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/directReports
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4544e-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4544e-119">Optional query parameters</span></span>
<span data-ttu-id="4544e-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4544e-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="4544e-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4544e-121">Request headers</span></span>
| <span data-ttu-id="4544e-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4544e-122">Header</span></span>       | <span data-ttu-id="4544e-123">Valor</span><span class="sxs-lookup"><span data-stu-id="4544e-123">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="4544e-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="4544e-124">Authorization</span></span>  | <span data-ttu-id="4544e-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4544e-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4544e-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4544e-127">Content-Type</span></span>   | <span data-ttu-id="4544e-128">application/json</span><span class="sxs-lookup"><span data-stu-id="4544e-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4544e-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4544e-129">Request body</span></span>
<span data-ttu-id="4544e-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4544e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4544e-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="4544e-131">Response</span></span>

<span data-ttu-id="4544e-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4544e-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4544e-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4544e-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4544e-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4544e-134">Request</span></span>
<span data-ttu-id="4544e-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4544e-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directreports"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/directReports
```
##### <a name="response"></a><span data-ttu-id="4544e-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="4544e-136">Response</span></span>
<span data-ttu-id="4544e-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4544e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List directReports",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
