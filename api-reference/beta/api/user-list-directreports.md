---
title: Listar directReports
description: Obtenha relatórios diretos do usuário. Retorna os usuários e contatos para quem este usuário está atribuído como gerente.
ms.openlocfilehash: 33903aa45fb5f7550feba72d0db48da389dd8c82
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035796"
---
# <a name="list-directreports"></a><span data-ttu-id="eba2f-104">Listar directReports</span><span class="sxs-lookup"><span data-stu-id="eba2f-104">List directReports</span></span>

> <span data-ttu-id="eba2f-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="eba2f-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eba2f-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="eba2f-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="eba2f-p103">Obtenha relatórios diretos do usuário. Retorna os usuários e contatos para quem este usuário está atribuído como gerente.</span><span class="sxs-lookup"><span data-stu-id="eba2f-p103">Get user's direct reports. Returns the users and contacts for whom this user is assigned as manager.</span></span>
## <a name="permissions"></a><span data-ttu-id="eba2f-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="eba2f-109">Permissions</span></span>
<span data-ttu-id="eba2f-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eba2f-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eba2f-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eba2f-112">Permission type</span></span>      | <span data-ttu-id="eba2f-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eba2f-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eba2f-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eba2f-114">Delegated (work or school account)</span></span> | <span data-ttu-id="eba2f-115">User.Read, User.ReadWrite, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="eba2f-115">User.Read, User.ReadWrite, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="eba2f-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eba2f-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eba2f-117">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eba2f-117">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="eba2f-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eba2f-118">Application</span></span> | <span data-ttu-id="eba2f-119">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eba2f-119">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="eba2f-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eba2f-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/directReports
```
## <a name="optional-query-parameters"></a><span data-ttu-id="eba2f-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="eba2f-121">Optional query parameters</span></span>
<span data-ttu-id="eba2f-122">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="eba2f-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="eba2f-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eba2f-123">Request headers</span></span>
| <span data-ttu-id="eba2f-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="eba2f-124">Header</span></span>       | <span data-ttu-id="eba2f-125">Valor</span><span class="sxs-lookup"><span data-stu-id="eba2f-125">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="eba2f-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="eba2f-126">Authorization</span></span>  | <span data-ttu-id="eba2f-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eba2f-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="eba2f-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="eba2f-129">Content-Type</span></span>   | <span data-ttu-id="eba2f-130">application/json</span><span class="sxs-lookup"><span data-stu-id="eba2f-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="eba2f-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eba2f-131">Request body</span></span>
<span data-ttu-id="eba2f-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="eba2f-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eba2f-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="eba2f-133">Response</span></span>

<span data-ttu-id="eba2f-134">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eba2f-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="eba2f-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eba2f-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eba2f-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eba2f-136">Request</span></span>
<span data-ttu-id="eba2f-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eba2f-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directreports"
}-->
```http
GET https://graph.microsoft.com/beta/me/directReports
```
##### <a name="response"></a><span data-ttu-id="eba2f-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="eba2f-138">Response</span></span>
<span data-ttu-id="eba2f-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eba2f-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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