---
title: Listar childFolders
description: 'Obtenha a coleção de pastas sob a pasta especificada. Você pode usar o `.../me/MailFolders` atalho para acessar o nível superior '
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 3fec593d1d1b29e84f43e46d4bee7ef8f4aa61d7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32565510"
---
# <a name="list-childfolders"></a><span data-ttu-id="29b92-104">Listar childFolders</span><span class="sxs-lookup"><span data-stu-id="29b92-104">List childFolders</span></span>

<span data-ttu-id="29b92-p102">Obtenha a coleção de pastas sob a pasta especificada. Você pode usar o atalho `.../me/MailFolders` para obter a coleção de pastas de nível superior e navegar até outra pasta.</span><span class="sxs-lookup"><span data-stu-id="29b92-p102">Get the folder collection under the specified folder. You can use the `.../me/MailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="29b92-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="29b92-107">Permissions</span></span>
<span data-ttu-id="29b92-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29b92-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29b92-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="29b92-110">Permission type</span></span>      | <span data-ttu-id="29b92-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="29b92-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="29b92-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="29b92-112">Delegated (work or school account)</span></span> | <span data-ttu-id="29b92-113">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="29b92-113">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="29b92-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="29b92-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29b92-115">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="29b92-115">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="29b92-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="29b92-116">Application</span></span> | <span data-ttu-id="29b92-117">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="29b92-117">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="29b92-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="29b92-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="29b92-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="29b92-119">Optional query parameters</span></span>
<span data-ttu-id="29b92-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="29b92-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="29b92-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="29b92-121">Request headers</span></span>
| <span data-ttu-id="29b92-122">Nome</span><span class="sxs-lookup"><span data-stu-id="29b92-122">Name</span></span>       | <span data-ttu-id="29b92-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="29b92-123">Type</span></span> | <span data-ttu-id="29b92-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="29b92-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="29b92-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="29b92-125">Authorization</span></span>  | <span data-ttu-id="29b92-126">string</span><span class="sxs-lookup"><span data-stu-id="29b92-126">string</span></span>  | <span data-ttu-id="29b92-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="29b92-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="29b92-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="29b92-129">Request body</span></span>
<span data-ttu-id="29b92-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="29b92-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="29b92-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="29b92-131">Response</span></span>

<span data-ttu-id="29b92-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [MailFolder](../resources/mailfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="29b92-132">If successful, this method returns a `200 OK` response code and collection of [MailFolder](../resources/mailfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="29b92-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="29b92-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="29b92-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="29b92-134">Request</span></span>
<span data-ttu-id="29b92-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="29b92-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_childfolders"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}/childFolders
```
##### <a name="response"></a><span data-ttu-id="29b92-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="29b92-136">Response</span></span>
<span data-ttu-id="29b92-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="29b92-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List childFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
