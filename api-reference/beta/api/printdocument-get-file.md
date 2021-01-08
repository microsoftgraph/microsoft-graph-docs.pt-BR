---
title: Baixar o arquivo binário printDocument
description: Baixe o arquivo binário associado ao documento.
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: c56d1012e4b375be318f48f91cfb7e9f863b5704
ms.sourcegitcommit: a0a5690ad9c109149e0b8c8baba164648ff5c226
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/08/2021
ms.locfileid: "49784868"
---
# <a name="download-printdocument-binary-file"></a><span data-ttu-id="b372b-103">Baixar o arquivo binário printDocument</span><span class="sxs-lookup"><span data-stu-id="b372b-103">Download printDocument binary file</span></span>

<span data-ttu-id="b372b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b372b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b372b-105">Baixe o arquivo binário associado a [um printDocument](../resources/printdocument.md).</span><span class="sxs-lookup"><span data-stu-id="b372b-105">Download the binary file associated with a [printDocument](../resources/printdocument.md).</span></span> <span data-ttu-id="b372b-106">Chamar esse método gera uma resposta de redirecionamento com uma URL pré-autenticada que pode ser usada para baixar a carga.</span><span class="sxs-lookup"><span data-stu-id="b372b-106">Calling this method yields a redirect response with a pre-authenticated URL that can be used to download the payload.</span></span>

## <a name="permissions"></a><span data-ttu-id="b372b-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="b372b-107">Permissions</span></span>
<span data-ttu-id="b372b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b372b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="b372b-110">Além das permissões a seguir, o usuário ou locatário do aplicativo deve ter uma [](printer-get.md) assinatura de Impressão Universal ativa e ter uma permissão que conceda acesso à impressora em caso de tokens de acesso do usuário e a permissão de aplicativo Printer.Read.All ou Printer.ReadWrite.All no caso de tokens de acesso somente aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b372b-110">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printer](printer-get.md) access in case of user's access tokens and either the Printer.Read.All or Printer.ReadWrite.All application permission in case of app-only access tokens.</span></span> 

| <span data-ttu-id="b372b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b372b-111">Permission type</span></span>                        | <span data-ttu-id="b372b-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b372b-112">Permissions (from least to most privileged)</span></span>                  |
| :------------------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="b372b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b372b-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="b372b-114">PrintJob.Read, PrintJob.Read.All, PrintJob.ReadWrite, PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b372b-114">PrintJob.Read, PrintJob.Read.All, PrintJob.ReadWrite, PrintJob.ReadWrite.All</span></span> |
| <span data-ttu-id="b372b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b372b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b372b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b372b-116">Not Supported.</span></span>                                               |
| <span data-ttu-id="b372b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b372b-117">Application</span></span>                            | <span data-ttu-id="b372b-118">PrintJob.Read.All, PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b372b-118">PrintJob.Read.All, PrintJob.ReadWrite.All</span></span>                    |

## <a name="http-request"></a><span data-ttu-id="b372b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b372b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}/jobs/{id}/documents/{id}/$value
```
## <a name="request-headers"></a><span data-ttu-id="b372b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b372b-120">Request headers</span></span>
| <span data-ttu-id="b372b-121">Nome</span><span class="sxs-lookup"><span data-stu-id="b372b-121">Name</span></span>          | <span data-ttu-id="b372b-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="b372b-122">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="b372b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b372b-123">Authorization</span></span> | <span data-ttu-id="b372b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b372b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b372b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b372b-126">Request body</span></span>
<span data-ttu-id="b372b-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b372b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b372b-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="b372b-128">Response</span></span>
<span data-ttu-id="b372b-129">Se bem-sucedido, este método retorna e a `302 Found` URL de download previamente autenticada no título Local.</span><span class="sxs-lookup"><span data-stu-id="b372b-129">If successful, this method returns `302 Found` and the pre-authenticated download URL in the Location header.</span></span>

## <a name="examples"></a><span data-ttu-id="b372b-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b372b-130">Examples</span></span>
<span data-ttu-id="b372b-131">O exemplo a seguir mostra como chamar essa API para adquirir uma URL de download pré-autenticada.</span><span class="sxs-lookup"><span data-stu-id="b372b-131">The following example shows how to call this API to acquire a pre-authenticated download URL.</span></span> <span data-ttu-id="b372b-132">Para iniciar o download, siga a URL de redirecionamento na resposta.</span><span class="sxs-lookup"><span data-stu-id="b372b-132">To start the download, follow the redirect URL in the response.</span></span>

### <a name="request"></a><span data-ttu-id="b372b-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b372b-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="b372b-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="b372b-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_document_value"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/fcb0bc53-a446-41d0-bfc3-5c56cdbb0f2a/jobs/46140/documents/bd260b1a-044e-4ca6-afa9-17d9a587d254/$value
```
# <a name="c"></a>[<span data-ttu-id="b372b-135">C#</span><span class="sxs-lookup"><span data-stu-id="b372b-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-document-value-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b372b-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b372b-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-document-value-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b372b-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b372b-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-document-value-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b372b-138">Java</span><span class="sxs-lookup"><span data-stu-id="b372b-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-document-value-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b372b-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="b372b-139">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 302 Accepted
Location: https://print.print.microsoft.com/downloads/bd260b1a-044e-4ca6-afa9-17d9a587d254?tempauthtoken={accesstoken}
```
