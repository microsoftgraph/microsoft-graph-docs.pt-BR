---
title: Listar childFolders
description: Obtém uma coleção de pastas filho sob a pasta de contatos especificada.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 78d2780b2089f5d4f90c9f7b090c43afe15c07f7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941244"
---
# <a name="list-childfolders"></a><span data-ttu-id="1a18f-103">Listar childFolders</span><span class="sxs-lookup"><span data-stu-id="1a18f-103">List childFolders</span></span>

> <span data-ttu-id="1a18f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1a18f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1a18f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1a18f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1a18f-106">Obtém uma coleção de pastas filho sob a pasta de contatos especificada.</span><span class="sxs-lookup"><span data-stu-id="1a18f-106">Get a collection of child folders under the specified contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="1a18f-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="1a18f-107">Permissions</span></span>
<span data-ttu-id="1a18f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a18f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a18f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1a18f-110">Permission type</span></span>      | <span data-ttu-id="1a18f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1a18f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1a18f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1a18f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1a18f-113">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1a18f-113">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="1a18f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1a18f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a18f-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1a18f-115">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="1a18f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1a18f-116">Application</span></span> | <span data-ttu-id="1a18f-117">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1a18f-117">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="1a18f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1a18f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1a18f-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1a18f-119">Optional query parameters</span></span>
<span data-ttu-id="1a18f-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1a18f-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="1a18f-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1a18f-121">Request headers</span></span>
| <span data-ttu-id="1a18f-122">Nome</span><span class="sxs-lookup"><span data-stu-id="1a18f-122">Name</span></span>       | <span data-ttu-id="1a18f-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="1a18f-123">Type</span></span> | <span data-ttu-id="1a18f-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a18f-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1a18f-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="1a18f-125">Authorization</span></span>  | <span data-ttu-id="1a18f-126">string</span><span class="sxs-lookup"><span data-stu-id="1a18f-126">string</span></span>  | <span data-ttu-id="1a18f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1a18f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1a18f-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1a18f-129">Request body</span></span>
<span data-ttu-id="1a18f-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1a18f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1a18f-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a18f-131">Response</span></span>

<span data-ttu-id="1a18f-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [ContactFolder](../resources/contactfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1a18f-132">If successful, this method returns a `200 OK` response code and collection of [ContactFolder](../resources/contactfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1a18f-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1a18f-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1a18f-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1a18f-134">Request</span></span>
<span data-ttu-id="1a18f-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1a18f-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_childfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/contactFolders/{id}/childFolders
```
##### <a name="response"></a><span data-ttu-id="1a18f-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a18f-136">Response</span></span>
<span data-ttu-id="1a18f-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1a18f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List childFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
