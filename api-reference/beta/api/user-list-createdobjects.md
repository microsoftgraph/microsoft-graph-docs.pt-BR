---
title: Listar createdObjects
description: Obtenha uma lista de objetos de diretório criados pelo usuário.
author: dkershaw10
ms.openlocfilehash: a7067926e5104c08d65a1753fc716787bed52fd5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27342102"
---
# <a name="list-createdobjects"></a><span data-ttu-id="d0c02-103">Listar createdObjects</span><span class="sxs-lookup"><span data-stu-id="d0c02-103">List createdObjects</span></span>

> <span data-ttu-id="d0c02-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d0c02-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d0c02-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d0c02-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d0c02-106">Obtenha uma lista de objetos de diretório criados pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="d0c02-106">Get a list of directory objects that were created by the user.</span></span>
## <a name="permissions"></a><span data-ttu-id="d0c02-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="d0c02-107">Permissions</span></span>
<span data-ttu-id="d0c02-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0c02-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0c02-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d0c02-110">Permission type</span></span>      | <span data-ttu-id="d0c02-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d0c02-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d0c02-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d0c02-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d0c02-113">User.Read, User.ReadWrite, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d0c02-113">User.Read, User.ReadWrite, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d0c02-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d0c02-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d0c02-115">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d0c02-115">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="d0c02-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d0c02-116">Application</span></span> | <span data-ttu-id="d0c02-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0c02-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d0c02-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d0c02-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/createdObjects
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d0c02-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d0c02-119">Optional query parameters</span></span>
<span data-ttu-id="d0c02-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d0c02-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d0c02-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d0c02-121">Request headers</span></span>
| <span data-ttu-id="d0c02-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d0c02-122">Header</span></span>       | <span data-ttu-id="d0c02-123">Valor</span><span class="sxs-lookup"><span data-stu-id="d0c02-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d0c02-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="d0c02-124">Authorization</span></span>  | <span data-ttu-id="d0c02-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d0c02-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d0c02-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d0c02-127">Content-Type</span></span>  | <span data-ttu-id="d0c02-128">application/json</span><span class="sxs-lookup"><span data-stu-id="d0c02-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d0c02-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d0c02-129">Request body</span></span>
<span data-ttu-id="d0c02-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d0c02-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d0c02-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0c02-131">Response</span></span>

<span data-ttu-id="d0c02-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d0c02-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d0c02-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d0c02-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d0c02-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d0c02-134">Request</span></span>
<span data-ttu-id="d0c02-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d0c02-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_createdobjects"
}-->
```http
GET https://graph.microsoft.com/beta/me/createdObjects
```
##### <a name="response"></a><span data-ttu-id="d0c02-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0c02-136">Response</span></span>
<span data-ttu-id="d0c02-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d0c02-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List createdObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->