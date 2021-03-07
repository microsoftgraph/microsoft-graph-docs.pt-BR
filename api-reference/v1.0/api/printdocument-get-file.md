---
title: Baixar arquivo binário printDocument
description: Baixe o arquivo binário associado ao documento.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 7bde42e03af509f101515dc847283fc1e354c478
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517025"
---
# <a name="download-printdocument-binary-file"></a><span data-ttu-id="d2701-103">Baixar arquivo binário printDocument</span><span class="sxs-lookup"><span data-stu-id="d2701-103">Download printDocument binary file</span></span>

<span data-ttu-id="d2701-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2701-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="d2701-105">Baixe o arquivo binário associado a [um printDocument](../resources/printdocument.md).</span><span class="sxs-lookup"><span data-stu-id="d2701-105">Download the binary file associated with a [printDocument](../resources/printdocument.md).</span></span> <span data-ttu-id="d2701-106">Chamar esse método gera uma resposta de redirecionamento com uma URL pré-autenticada que pode ser usada para baixar a carga.</span><span class="sxs-lookup"><span data-stu-id="d2701-106">Calling this method yields a redirect response with a pre-authenticated URL that can be used to download the payload.</span></span>

## <a name="permissions"></a><span data-ttu-id="d2701-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="d2701-107">Permissions</span></span>
<span data-ttu-id="d2701-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2701-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="d2701-110">Além das permissões a seguir, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa e ter uma permissão que conceda concessões obter acesso [à](printer-get.md) impressora.</span><span class="sxs-lookup"><span data-stu-id="d2701-110">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants grants [Get printer](printer-get.md) access.</span></span>

| <span data-ttu-id="d2701-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d2701-111">Permission type</span></span>                        | <span data-ttu-id="d2701-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d2701-112">Permissions (from least to most privileged)</span></span>                  |
| :------------------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="d2701-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d2701-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="d2701-114">PrintJob.Read, PrintJob.Read.All, PrintJob.ReadWrite, PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2701-114">PrintJob.Read, PrintJob.Read.All, PrintJob.ReadWrite, PrintJob.ReadWrite.All</span></span> |
| <span data-ttu-id="d2701-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d2701-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2701-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d2701-116">Not Supported.</span></span>                                               |
| <span data-ttu-id="d2701-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d2701-117">Application</span></span>                            | <span data-ttu-id="d2701-118">PrintJob.Read.All, PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2701-118">PrintJob.Read.All, PrintJob.ReadWrite.All</span></span>                    |

## <a name="http-request"></a><span data-ttu-id="d2701-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d2701-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{printerId}/jobs/{printJobId}/documents/{printDocumentId}/$value
```
## <a name="request-headers"></a><span data-ttu-id="d2701-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d2701-120">Request headers</span></span>
| <span data-ttu-id="d2701-121">Nome</span><span class="sxs-lookup"><span data-stu-id="d2701-121">Name</span></span>          | <span data-ttu-id="d2701-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2701-122">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="d2701-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d2701-123">Authorization</span></span> | <span data-ttu-id="d2701-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d2701-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d2701-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d2701-126">Request body</span></span>
<span data-ttu-id="d2701-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d2701-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d2701-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2701-128">Response</span></span>
<span data-ttu-id="d2701-129">Se tiver êxito, este método retornará e a `302 Found` URL de download pré-autenticada no header Location.</span><span class="sxs-lookup"><span data-stu-id="d2701-129">If successful, this method returns `302 Found` and the pre-authenticated download URL in the Location header.</span></span>

## <a name="examples"></a><span data-ttu-id="d2701-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d2701-130">Examples</span></span>
<span data-ttu-id="d2701-131">O exemplo a seguir mostra como chamar essa API para adquirir uma URL de download pré-autenticada.</span><span class="sxs-lookup"><span data-stu-id="d2701-131">The following example shows how to call this API to acquire a pre-authenticated download URL.</span></span> <span data-ttu-id="d2701-132">Para iniciar o download, siga a URL de redirecionamento na resposta.</span><span class="sxs-lookup"><span data-stu-id="d2701-132">To start the download, follow the redirect URL in the response.</span></span>

### <a name="request"></a><span data-ttu-id="d2701-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d2701-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_document_value"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/print/printers/{printerId}/jobs/{printJobId}/documents/{printDocumentId}/$value
```

### <a name="response"></a><span data-ttu-id="d2701-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2701-134">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 302 Found
Location: https://print.print.microsoft.com/downloads/bd260b1a-044e-4ca6-afa9-17d9a587d254?tempauthtoken={accesstoken}
```
