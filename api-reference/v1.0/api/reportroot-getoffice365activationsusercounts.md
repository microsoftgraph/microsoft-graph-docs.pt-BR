---
title: 'reportRoot: getOffice365ActivationsUserCounts'
description: Obtenha a contagem de usuários habilitados e aqueles que ativaram a assinatura do Office em desktops ou dispositivos ou computadores compartilhados.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 9a17bb8c34d5658ea747c64d4ca8e61bdce61b19
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35268716"
---
# <a name="reportroot-getoffice365activationsusercounts"></a><span data-ttu-id="39013-103">reportRoot: getOffice365ActivationsUserCounts</span><span class="sxs-lookup"><span data-stu-id="39013-103">reportRoot: getOffice365ActivationsUserCounts</span></span>

<span data-ttu-id="39013-104">Obtenha a contagem de usuários habilitados e aqueles que ativaram a assinatura do Office em desktops ou dispositivos ou computadores compartilhados.</span><span class="sxs-lookup"><span data-stu-id="39013-104">Get the count of users that are enabled and those that have activated the Office subscription on desktop or devices or shared computers.</span></span>

> <span data-ttu-id="39013-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Ativações do Microsoft Office](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="39013-105">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="39013-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="39013-106">Permissions</span></span>

<span data-ttu-id="39013-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39013-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="39013-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="39013-109">Permission type</span></span>                        | <span data-ttu-id="39013-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="39013-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="39013-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="39013-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="39013-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="39013-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="39013-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="39013-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="39013-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="39013-114">Not supported.</span></span>                           |
| <span data-ttu-id="39013-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="39013-115">Application</span></span>                            | <span data-ttu-id="39013-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="39013-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="39013-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="39013-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserCounts
```

## <a name="request-headers"></a><span data-ttu-id="39013-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="39013-118">Request headers</span></span>

| <span data-ttu-id="39013-119">Nome</span><span class="sxs-lookup"><span data-stu-id="39013-119">Name</span></span>          | <span data-ttu-id="39013-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="39013-120">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="39013-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="39013-121">Authorization</span></span> | <span data-ttu-id="39013-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="39013-p102">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="39013-124">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="39013-124">If-None-Match</span></span> | <span data-ttu-id="39013-125">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="39013-125">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="39013-126">Opcional.</span><span class="sxs-lookup"><span data-stu-id="39013-126">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="39013-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="39013-127">Response</span></span>

<span data-ttu-id="39013-128">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="39013-128">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="39013-129">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="39013-129">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="39013-130">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="39013-130">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="39013-131">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="39013-131">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="39013-132">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="39013-132">Report Refresh Date</span></span>
- <span data-ttu-id="39013-133">Tipo de produto</span><span class="sxs-lookup"><span data-stu-id="39013-133">Product Type</span></span>
- <span data-ttu-id="39013-134">Atribuído</span><span class="sxs-lookup"><span data-stu-id="39013-134">Assigned</span></span>
- <span data-ttu-id="39013-135">Ativado</span><span class="sxs-lookup"><span data-stu-id="39013-135">Activated</span></span>
- <span data-ttu-id="39013-136">Ativação de computador compartilhado</span><span class="sxs-lookup"><span data-stu-id="39013-136">Shared Computer Activation</span></span>

## <a name="example"></a><span data-ttu-id="39013-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="39013-137">Example</span></span>

#### <a name="request"></a><span data-ttu-id="39013-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="39013-138">Request</span></span>

<span data-ttu-id="39013-139">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="39013-139">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activationsusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActivationsUserCounts
```

#### <a name="response"></a><span data-ttu-id="39013-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="39013-140">Response</span></span>

<span data-ttu-id="39013-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="39013-141">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.report"
} -->

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="39013-142">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="39013-142">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="39013-143">C#</span><span class="sxs-lookup"><span data-stu-id="39013-143">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365activationsusercounts-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="39013-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="39013-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365activationsusercounts-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="39013-145">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="39013-145">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365activationsusercounts-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="39013-146">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="39013-146">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Product Type,Assigned,Activated,Shared Computer Activation
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/reportroot-getoffice365activationsusercounts.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/reportroot-getoffice365activationsusercounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/reportroot-getoffice365activationsusercounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
