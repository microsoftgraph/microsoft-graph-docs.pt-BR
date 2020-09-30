---
title: Baixar arquivo binário do documento
description: Baixe o arquivo binário associado ao documento.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: dca15d5a57631fc58500046388975f1b03486a18
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/30/2020
ms.locfileid: "48314056"
---
# <a name="download-printdocument-binary-file"></a><span data-ttu-id="96825-103">Baixar arquivo binário do documento</span><span class="sxs-lookup"><span data-stu-id="96825-103">Download printDocument binary file</span></span>

<span data-ttu-id="96825-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96825-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96825-105">Baixar o arquivo binário associado a um [documento](../resources/printdocument.md).</span><span class="sxs-lookup"><span data-stu-id="96825-105">Download the binary file associated with a [printDocument](../resources/printdocument.md).</span></span> <span data-ttu-id="96825-106">Chamar esse método gera uma resposta de redirecionamento com uma URL previamente autenticada que pode ser usada para baixar a carga.</span><span class="sxs-lookup"><span data-stu-id="96825-106">Calling this method yields a redirect response with a pre-authenticated URL that can be used to download the payload.</span></span>

## <a name="permissions"></a><span data-ttu-id="96825-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="96825-107">Permissions</span></span>
<span data-ttu-id="96825-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96825-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="96825-110">Além das permissões a seguir, o locatário do usuário ou do aplicativo deve ter uma assinatura universal de impressão ativa e ter uma permissão que conceda obter acesso à [impressora](printer-get.md) .</span><span class="sxs-lookup"><span data-stu-id="96825-110">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printer](printer-get.md) access.</span></span>

| <span data-ttu-id="96825-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="96825-111">Permission type</span></span>                        | <span data-ttu-id="96825-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="96825-112">Permissions (from least to most privileged)</span></span>                  |
| :------------------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="96825-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="96825-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="96825-114">PrintJob. Read, PrintJob. Read. All, PrintJob. ReadWrite, PrintJob. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="96825-114">PrintJob.Read, PrintJob.Read.All, PrintJob.ReadWrite, PrintJob.ReadWrite.All</span></span> |
| <span data-ttu-id="96825-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="96825-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96825-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="96825-116">Not Supported.</span></span>                                               |
| <span data-ttu-id="96825-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="96825-117">Application</span></span>                            | <span data-ttu-id="96825-118">PrintJob. Read. All, PrintJob. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="96825-118">PrintJob.Read.All, PrintJob.ReadWrite.All</span></span>                    |

## <a name="http-request"></a><span data-ttu-id="96825-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="96825-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}/jobs/{id}/documents/{id}/$value
```
## <a name="request-headers"></a><span data-ttu-id="96825-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="96825-120">Request headers</span></span>
| <span data-ttu-id="96825-121">Nome</span><span class="sxs-lookup"><span data-stu-id="96825-121">Name</span></span>          | <span data-ttu-id="96825-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="96825-122">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="96825-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="96825-123">Authorization</span></span> | <span data-ttu-id="96825-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="96825-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="96825-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="96825-126">Request body</span></span>
<span data-ttu-id="96825-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="96825-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="96825-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="96825-128">Response</span></span>
<span data-ttu-id="96825-129">Se tiver êxito, este método retornará `302 Found` e a URL de download previamente autenticado no cabeçalho de local.</span><span class="sxs-lookup"><span data-stu-id="96825-129">If successful, this method returns `302 Found` and the pre-authenticated download URL in the Location header.</span></span>

## <a name="examples"></a><span data-ttu-id="96825-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="96825-130">Examples</span></span>
<span data-ttu-id="96825-131">O exemplo a seguir mostra como chamar essa API para adquirir uma URL de download previamente autenticado.</span><span class="sxs-lookup"><span data-stu-id="96825-131">The following example shows how to call this API to acquire a pre-authenticated download URL.</span></span> <span data-ttu-id="96825-132">Para iniciar o download, siga a URL de redirecionamento na resposta.</span><span class="sxs-lookup"><span data-stu-id="96825-132">To start the download, follow the redirect URL in the response.</span></span>

### <a name="request"></a><span data-ttu-id="96825-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="96825-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="96825-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="96825-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_document_value"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/fcb0bc53-a446-41d0-bfc3-5c56cdbb0f2a/jobs/46140/documents/bd260b1a-044e-4ca6-afa9-17d9a587d254/$value
```
# <a name="c"></a>[<span data-ttu-id="96825-135">C#</span><span class="sxs-lookup"><span data-stu-id="96825-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-document-value-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="96825-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="96825-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-document-value-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="96825-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="96825-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-document-value-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="96825-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="96825-138">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 302 Accepted
Location: https://print.print.microsoft.com/downloads/bd260b1a-044e-4ca6-afa9-17d9a587d254?tempauthtoken={accesstoken}
```
