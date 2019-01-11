---
title: Obter recurso
description: Recupere os dados binários do objeto resource de um arquivo ou imagem.
localization_priority: Normal
ms.openlocfilehash: 1f8150e0449009eef4d1afe2ce014ae848153382
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27841255"
---
# <a name="get-resource"></a><span data-ttu-id="ef1e7-103">Obter recurso</span><span class="sxs-lookup"><span data-stu-id="ef1e7-103">Get resource</span></span>

> <span data-ttu-id="ef1e7-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ef1e7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ef1e7-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ef1e7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ef1e7-106">Recupere os dados binários do objeto [resource](../resources/resource.md) de um arquivo ou imagem.</span><span class="sxs-lookup"><span data-stu-id="ef1e7-106">Retrieve the binary data of a file or image [resource](../resources/resource.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ef1e7-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="ef1e7-107">Permissions</span></span>
<span data-ttu-id="ef1e7-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef1e7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef1e7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ef1e7-110">Permission type</span></span>      | <span data-ttu-id="ef1e7-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ef1e7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ef1e7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ef1e7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ef1e7-113">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef1e7-113">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="ef1e7-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ef1e7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ef1e7-115">Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ef1e7-115">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="ef1e7-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ef1e7-116">Application</span></span> | <span data-ttu-id="ef1e7-117">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef1e7-117">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ef1e7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ef1e7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/resources/{id}/content
GET /users/{id | userPrincipalName}/onenote/resources/{id}/content
GET /groups/{id}/onenote/resources/{id}/content
GET /sites/{id}/onenote/resources/{id}/content
```

## <a name="request-headers"></a><span data-ttu-id="ef1e7-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ef1e7-119">Request headers</span></span>
| <span data-ttu-id="ef1e7-120">Nome</span><span class="sxs-lookup"><span data-stu-id="ef1e7-120">Name</span></span>       | <span data-ttu-id="ef1e7-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="ef1e7-121">Type</span></span> | <span data-ttu-id="ef1e7-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="ef1e7-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ef1e7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ef1e7-123">Authorization</span></span>  | <span data-ttu-id="ef1e7-124">string</span><span class="sxs-lookup"><span data-stu-id="ef1e7-124">string</span></span>  | <span data-ttu-id="ef1e7-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ef1e7-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ef1e7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ef1e7-127">Request body</span></span>
<span data-ttu-id="ef1e7-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ef1e7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ef1e7-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef1e7-129">Response</span></span>

<span data-ttu-id="ef1e7-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e os dados binários do arquivo ou imagem no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ef1e7-130">If successful, this method returns a `200 OK` response code and the image or file binary data in the response body.</span></span>

<span data-ttu-id="ef1e7-131">Observação: As imagens não serão renderizadas diretamente em um navegador porque elas exigem autorização para recuperá-las, como o restante do conteúdo da página.</span><span class="sxs-lookup"><span data-stu-id="ef1e7-131">Note: Images won't render directly in a browser because they require authorization to retrieve them, like the rest of the page content.</span></span>
## <a name="example"></a><span data-ttu-id="ef1e7-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ef1e7-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ef1e7-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ef1e7-133">Request</span></span>
<span data-ttu-id="ef1e7-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ef1e7-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_resource"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/resources/{id}/content
```
##### <a name="response"></a><span data-ttu-id="ef1e7-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef1e7-135">Response</span></span>
<span data-ttu-id="ef1e7-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ef1e7-136">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->
```http
HTTP/1.1 200 OK

...binary data...
```
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.onenoteResource"
} -->

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
