---
title: Listar mailFolders
description: Obtenha todas as pastas de email na caixa de correio do usuário conectado.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: cb2d9e50776d88676cd6c2fdde39d9de89a635c0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990296"
---
# <a name="list-mailfolders"></a><span data-ttu-id="970a4-103">Listar mailFolders</span><span class="sxs-lookup"><span data-stu-id="970a4-103">List mailFolders</span></span>

> <span data-ttu-id="970a4-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="970a4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="970a4-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="970a4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="970a4-106">Obtenha todas as pastas de email na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="970a4-106">Get all the mail folders in the signed-in user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="970a4-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="970a4-107">Permissions</span></span>
<span data-ttu-id="970a4-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="970a4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="970a4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="970a4-110">Permission type</span></span>      | <span data-ttu-id="970a4-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="970a4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="970a4-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="970a4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="970a4-113">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="970a4-113">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="970a4-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="970a4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="970a4-115">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="970a4-115">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="970a4-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="970a4-116">Application</span></span> | <span data-ttu-id="970a4-117">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="970a4-117">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="970a4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="970a4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/mailFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="970a4-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="970a4-119">Optional query parameters</span></span>
<span data-ttu-id="970a4-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="970a4-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="970a4-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="970a4-121">Request headers</span></span>
| <span data-ttu-id="970a4-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="970a4-122">Header</span></span>       | <span data-ttu-id="970a4-123">Valor</span><span class="sxs-lookup"><span data-stu-id="970a4-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="970a4-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="970a4-124">Authorization</span></span>  | <span data-ttu-id="970a4-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="970a4-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="970a4-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="970a4-127">Content-Type</span></span>   | <span data-ttu-id="970a4-128">application/json</span><span class="sxs-lookup"><span data-stu-id="970a4-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="970a4-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="970a4-129">Request body</span></span>
<span data-ttu-id="970a4-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="970a4-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="970a4-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="970a4-131">Response</span></span>

<span data-ttu-id="970a4-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [MailFolder](../resources/mailfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="970a4-132">If successful, this method returns a `200 OK` response code and collection of [MailFolder](../resources/mailfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="970a4-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="970a4-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="970a4-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="970a4-134">Request</span></span>
<span data-ttu-id="970a4-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="970a4-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailFolders
```
##### <a name="response"></a><span data-ttu-id="970a4-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="970a4-136">Response</span></span>
<span data-ttu-id="970a4-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="970a4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
