---
title: Listar createdObjects
description: Obtenha uma lista de objetos de diretório criados pelo usuário.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: 8ad374df970c7e17c88781e248aef4dd0ed432b5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876010"
---
# <a name="list-createdobjects"></a><span data-ttu-id="9ed6b-103">Listar createdObjects</span><span class="sxs-lookup"><span data-stu-id="9ed6b-103">List createdObjects</span></span>

> <span data-ttu-id="9ed6b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9ed6b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9ed6b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9ed6b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9ed6b-106">Obtenha uma lista de objetos de diretório criados pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="9ed6b-106">Get a list of directory objects that were created by the user.</span></span>
## <a name="permissions"></a><span data-ttu-id="9ed6b-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="9ed6b-107">Permissions</span></span>
<span data-ttu-id="9ed6b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ed6b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ed6b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9ed6b-110">Permission type</span></span>      | <span data-ttu-id="9ed6b-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9ed6b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9ed6b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9ed6b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9ed6b-113">User.Read, User.ReadWrite, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9ed6b-113">User.Read, User.ReadWrite, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9ed6b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9ed6b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ed6b-115">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9ed6b-115">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="9ed6b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9ed6b-116">Application</span></span> | <span data-ttu-id="9ed6b-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ed6b-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9ed6b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9ed6b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/createdObjects
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9ed6b-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9ed6b-119">Optional query parameters</span></span>
<span data-ttu-id="9ed6b-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9ed6b-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="9ed6b-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9ed6b-121">Request headers</span></span>
| <span data-ttu-id="9ed6b-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9ed6b-122">Header</span></span>       | <span data-ttu-id="9ed6b-123">Valor</span><span class="sxs-lookup"><span data-stu-id="9ed6b-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9ed6b-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="9ed6b-124">Authorization</span></span>  | <span data-ttu-id="9ed6b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9ed6b-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9ed6b-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9ed6b-127">Content-Type</span></span>  | <span data-ttu-id="9ed6b-128">application/json</span><span class="sxs-lookup"><span data-stu-id="9ed6b-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9ed6b-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9ed6b-129">Request body</span></span>
<span data-ttu-id="9ed6b-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9ed6b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9ed6b-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ed6b-131">Response</span></span>

<span data-ttu-id="9ed6b-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9ed6b-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9ed6b-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9ed6b-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9ed6b-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9ed6b-134">Request</span></span>
<span data-ttu-id="9ed6b-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9ed6b-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_createdobjects"
}-->
```http
GET https://graph.microsoft.com/beta/me/createdObjects
```
##### <a name="response"></a><span data-ttu-id="9ed6b-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ed6b-136">Response</span></span>
<span data-ttu-id="9ed6b-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9ed6b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
