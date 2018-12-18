---
title: Listar mailFolders
description: 'Obtenha a coleção de pastas de email sob a pasta raiz do usuário conectado. '
author: dkershaw10
ms.openlocfilehash: 6dfe86022db740dbebfc79c3da5905a8dd0a6827
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359973"
---
# <a name="list-mailfolders"></a><span data-ttu-id="32deb-103">Listar mailFolders</span><span class="sxs-lookup"><span data-stu-id="32deb-103">List mailFolders</span></span>

<span data-ttu-id="32deb-104">Obtenha a coleção de pastas de email sob a pasta raiz do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="32deb-104">Get the mail folder collection under the root folder of the signed-in user.</span></span> 
## <a name="permissions"></a><span data-ttu-id="32deb-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="32deb-105">Permissions</span></span>
<span data-ttu-id="32deb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32deb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32deb-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="32deb-108">Permission type</span></span>      | <span data-ttu-id="32deb-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="32deb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="32deb-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="32deb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="32deb-111">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="32deb-111">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="32deb-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="32deb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="32deb-113">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="32deb-113">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="32deb-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="32deb-114">Application</span></span> | <span data-ttu-id="32deb-115">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="32deb-115">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="32deb-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="32deb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/mailFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="32deb-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="32deb-117">Optional query parameters</span></span>
<span data-ttu-id="32deb-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="32deb-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="32deb-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="32deb-119">Request headers</span></span>
| <span data-ttu-id="32deb-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="32deb-120">Header</span></span>       | <span data-ttu-id="32deb-121">Valor</span><span class="sxs-lookup"><span data-stu-id="32deb-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="32deb-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="32deb-122">Authorization</span></span>  | <span data-ttu-id="32deb-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="32deb-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="32deb-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="32deb-125">Content-Type</span></span>   | <span data-ttu-id="32deb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="32deb-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="32deb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="32deb-127">Request body</span></span>
<span data-ttu-id="32deb-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="32deb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="32deb-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="32deb-129">Response</span></span>

<span data-ttu-id="32deb-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [MailFolder](../resources/mailfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="32deb-130">If successful, this method returns a `200 OK` response code and collection of [MailFolder](../resources/mailfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="32deb-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="32deb-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="32deb-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="32deb-132">Request</span></span>
<span data-ttu-id="32deb-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="32deb-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailfolders"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders
```
##### <a name="response"></a><span data-ttu-id="32deb-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="32deb-134">Response</span></span>
<span data-ttu-id="32deb-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="32deb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 232

{
  "value": [
    {
      "displayName": "displayName-value",
      "parentFolderId": "parentFolderId-value",
      "childFolderCount": 99,
      "unreadItemCount": 99,
      "totalItemCount": 99,
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List mailFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
