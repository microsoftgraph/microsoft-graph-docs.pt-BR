---
title: Listar contactFolders
description: Obtenha a coleção de pasta de contatos na pasta de contatos padrão do usuário conectado.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: 55558b8ea0db3c35d63abdffdef55d01488fe7e4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27857369"
---
# <a name="list-contactfolders"></a><span data-ttu-id="cdbf7-103">Listar contactFolders</span><span class="sxs-lookup"><span data-stu-id="cdbf7-103">List contactFolders</span></span>

<span data-ttu-id="cdbf7-104">Obtenha a coleção de pasta de contatos na pasta de contatos padrão do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="cdbf7-104">Get the contact folder collection in the default Contacts folder of the signed-in user.</span></span>
## <a name="permissions"></a><span data-ttu-id="cdbf7-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="cdbf7-105">Permissions</span></span>
<span data-ttu-id="cdbf7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cdbf7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cdbf7-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cdbf7-108">Permission type</span></span>      | <span data-ttu-id="cdbf7-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cdbf7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cdbf7-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cdbf7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cdbf7-111">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cdbf7-111">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="cdbf7-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cdbf7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cdbf7-113">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cdbf7-113">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="cdbf7-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cdbf7-114">Application</span></span> | <span data-ttu-id="cdbf7-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cdbf7-115">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="cdbf7-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cdbf7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/contactFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="cdbf7-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="cdbf7-117">Optional query parameters</span></span>
<span data-ttu-id="cdbf7-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="cdbf7-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="cdbf7-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cdbf7-119">Request headers</span></span>
| <span data-ttu-id="cdbf7-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cdbf7-120">Header</span></span>       | <span data-ttu-id="cdbf7-121">Valor</span><span class="sxs-lookup"><span data-stu-id="cdbf7-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cdbf7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="cdbf7-122">Authorization</span></span>  | <span data-ttu-id="cdbf7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cdbf7-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="cdbf7-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cdbf7-125">Content-Type</span></span>   | <span data-ttu-id="cdbf7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cdbf7-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cdbf7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cdbf7-127">Request body</span></span>
<span data-ttu-id="cdbf7-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cdbf7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cdbf7-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="cdbf7-129">Response</span></span>

<span data-ttu-id="cdbf7-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [ContactFolder](../resources/contactfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cdbf7-130">If successful, this method returns a `200 OK` response code and collection of [ContactFolder](../resources/contactfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cdbf7-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cdbf7-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cdbf7-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cdbf7-132">Request</span></span>
<span data-ttu-id="cdbf7-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cdbf7-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contactfolders"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contactFolders
```
##### <a name="response"></a><span data-ttu-id="cdbf7-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="cdbf7-134">Response</span></span>
<span data-ttu-id="cdbf7-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cdbf7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 145

{
  "value": [
    {
      "parentFolderId": "parentFolderId-value",
      "displayName": "displayName-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List contactFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
