---
title: Baixar arquivo binário do documento
description: Baixe o arquivo binário associado ao documento.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: a7e7de914d8549472e08c23f65af25ca99542a58
ms.sourcegitcommit: 3c0fa2d13ede0fdfa66d966d4ec32cb468c3befa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/25/2020
ms.locfileid: "48273652"
---
# <a name="download-printdocument-binary-file"></a><span data-ttu-id="d4145-103">Baixar arquivo binário do documento</span><span class="sxs-lookup"><span data-stu-id="d4145-103">Download printDocument binary file</span></span>

<span data-ttu-id="d4145-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4145-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4145-105">Baixar o arquivo binário associado a um [documento](../resources/printdocument.md).</span><span class="sxs-lookup"><span data-stu-id="d4145-105">Download the binary file associated with a [printDocument](../resources/printdocument.md).</span></span> <span data-ttu-id="d4145-106">Chamar esse método gera uma resposta de redirecionamento com uma URL previamente autenticada que pode ser usada para baixar a carga.</span><span class="sxs-lookup"><span data-stu-id="d4145-106">Calling this method yields a redirect response with a pre-authenticated URL that can be used to download the payload.</span></span>

## <a name="permissions"></a><span data-ttu-id="d4145-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="d4145-107">Permissions</span></span>
<span data-ttu-id="d4145-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4145-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="d4145-110">Além das permissões a seguir, o locatário do usuário ou do aplicativo deve ter uma assinatura universal de impressão ativa e ter uma permissão que conceda obter acesso à [impressora](printer-get.md) .</span><span class="sxs-lookup"><span data-stu-id="d4145-110">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printer](printer-get.md) access.</span></span>

| <span data-ttu-id="d4145-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d4145-111">Permission type</span></span>                        | <span data-ttu-id="d4145-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d4145-112">Permissions (from least to most privileged)</span></span>                  |
| :------------------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="d4145-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d4145-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="d4145-114">PrintJob. Read, PrintJob. Read. All, PrintJob. ReadWrite, PrintJob. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="d4145-114">PrintJob.Read, PrintJob.Read.All, PrintJob.ReadWrite, PrintJob.ReadWrite.All</span></span> |
| <span data-ttu-id="d4145-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d4145-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d4145-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d4145-116">Not Supported.</span></span>                                               |
| <span data-ttu-id="d4145-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d4145-117">Application</span></span>                            | <span data-ttu-id="d4145-118">PrintJob. Read. All, PrintJob. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="d4145-118">PrintJob.Read.All, PrintJob.ReadWrite.All</span></span>                    |

## <a name="http-request"></a><span data-ttu-id="d4145-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d4145-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}/jobs/{id}/documents/{id}/$value
```
## <a name="request-headers"></a><span data-ttu-id="d4145-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d4145-120">Request headers</span></span>
| <span data-ttu-id="d4145-121">Nome</span><span class="sxs-lookup"><span data-stu-id="d4145-121">Name</span></span>          | <span data-ttu-id="d4145-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4145-122">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="d4145-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d4145-123">Authorization</span></span> | <span data-ttu-id="d4145-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d4145-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d4145-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d4145-126">Request body</span></span>
<span data-ttu-id="d4145-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d4145-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d4145-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4145-128">Response</span></span>
<span data-ttu-id="d4145-129">Se tiver êxito, este método retornará `302 Found` e a URL de download previamente autenticado no cabeçalho de local.</span><span class="sxs-lookup"><span data-stu-id="d4145-129">If successful, this method returns `302 Found` and the pre-authenticated download URL in the Location header.</span></span>

## <a name="examples"></a><span data-ttu-id="d4145-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d4145-130">Examples</span></span>
<span data-ttu-id="d4145-131">O exemplo a seguir mostra como chamar essa API para adquirir uma URL de download previamente autenticado.</span><span class="sxs-lookup"><span data-stu-id="d4145-131">The following example shows how to call this API to acquire a pre-authenticated download URL.</span></span> <span data-ttu-id="d4145-132">Para iniciar o download, siga a URL de redirecionamento na resposta.</span><span class="sxs-lookup"><span data-stu-id="d4145-132">To start the download, follow the redirect URL in the response.</span></span>

### <a name="request"></a><span data-ttu-id="d4145-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d4145-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_document_value"
}-->
```http
GET https://graph.microsoft.com/beta/print/printers/fcb0bc53-a446-41d0-bfc3-5c56cdbb0f2a/jobs/46140/documents/bd260b1a-044e-4ca6-afa9-17d9a587d254/$value
```

### <a name="response"></a><span data-ttu-id="d4145-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4145-134">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 302 Accepted
Location: https://print.print.microsoft.com/downloads/bd260b1a-044e-4ca6-afa9-17d9a587d254?tempauthtoken={accesstoken}
```
