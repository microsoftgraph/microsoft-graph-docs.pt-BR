---
title: 'reportRoot: getOffice365ActivationsUserDetail'
description: Obtenha dados sobre usuários que ativaram o Office 365.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: a6b8e47017f42762dfd9e3e6f8b2792c562004b9
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35268702"
---
# <a name="reportroot-getoffice365activationsuserdetail"></a><span data-ttu-id="7f354-103">reportRoot: getOffice365ActivationsUserDetail</span><span class="sxs-lookup"><span data-stu-id="7f354-103">reportRoot: getOffice365ActivationsUserDetail</span></span>

<span data-ttu-id="7f354-104">Obtenha dados sobre usuários que ativaram o Office 365.</span><span class="sxs-lookup"><span data-stu-id="7f354-104">Get details about users who have activated Office 365.</span></span>

> <span data-ttu-id="7f354-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Ativações do Microsoft Office](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="7f354-105">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="7f354-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7f354-106">Permissions</span></span>

<span data-ttu-id="7f354-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f354-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7f354-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7f354-109">Permission type</span></span>                        | <span data-ttu-id="7f354-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7f354-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="7f354-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7f354-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7f354-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f354-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="7f354-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7f354-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f354-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7f354-114">Not supported.</span></span>                           |
| <span data-ttu-id="7f354-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7f354-115">Application</span></span>                            | <span data-ttu-id="7f354-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f354-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="7f354-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7f354-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserDetail
```

## <a name="request-headers"></a><span data-ttu-id="7f354-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7f354-118">Request headers</span></span>

| <span data-ttu-id="7f354-119">Nome</span><span class="sxs-lookup"><span data-stu-id="7f354-119">Name</span></span>          | <span data-ttu-id="7f354-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f354-120">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="7f354-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="7f354-121">Authorization</span></span> | <span data-ttu-id="7f354-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7f354-p102">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="7f354-124">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="7f354-124">If-None-Match</span></span> | <span data-ttu-id="7f354-125">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="7f354-125">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="7f354-126">Opcional.</span><span class="sxs-lookup"><span data-stu-id="7f354-126">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="7f354-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f354-127">Response</span></span>

<span data-ttu-id="7f354-128">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="7f354-128">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="7f354-129">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="7f354-129">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="7f354-130">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="7f354-130">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="7f354-131">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="7f354-131">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="7f354-132">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="7f354-132">Report Refresh Date</span></span>
- <span data-ttu-id="7f354-133">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="7f354-133">User Principal Name</span></span>
- <span data-ttu-id="7f354-134">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="7f354-134">Display Name</span></span>
- <span data-ttu-id="7f354-135">Tipo de produto</span><span class="sxs-lookup"><span data-stu-id="7f354-135">Product Type</span></span>
- <span data-ttu-id="7f354-136">Data da última ativação</span><span class="sxs-lookup"><span data-stu-id="7f354-136">Last Activated Date</span></span>
- <span data-ttu-id="7f354-137">Windows</span><span class="sxs-lookup"><span data-stu-id="7f354-137">Windows</span></span>
- <span data-ttu-id="7f354-138">Mac</span><span class="sxs-lookup"><span data-stu-id="7f354-138">Mac</span></span>
- <span data-ttu-id="7f354-139">Windows 10 Mobile</span><span class="sxs-lookup"><span data-stu-id="7f354-139">Windows 10 Mobile</span></span>
- <span data-ttu-id="7f354-140">iOS</span><span class="sxs-lookup"><span data-stu-id="7f354-140">iOS</span></span>
- <span data-ttu-id="7f354-141">Android</span><span class="sxs-lookup"><span data-stu-id="7f354-141">Android</span></span>
- <span data-ttu-id="7f354-142">Ativado no computador compartilhado</span><span class="sxs-lookup"><span data-stu-id="7f354-142">Activated On Shared Computer</span></span>

## <a name="example"></a><span data-ttu-id="7f354-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7f354-143">Example</span></span>

#### <a name="request"></a><span data-ttu-id="7f354-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7f354-144">Request</span></span>

<span data-ttu-id="7f354-145">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7f354-145">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activationsuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActivationsUserDetail
```

#### <a name="response"></a><span data-ttu-id="7f354-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f354-146">Response</span></span>

<span data-ttu-id="7f354-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7f354-147">The following is an example of the response.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="7f354-148">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="7f354-148">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="7f354-149">C#</span><span class="sxs-lookup"><span data-stu-id="7f354-149">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365activationsuserdetail-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7f354-150">Javascript</span><span class="sxs-lookup"><span data-stu-id="7f354-150">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365activationsuserdetail-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="7f354-151">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="7f354-151">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365activationsuserdetail-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="7f354-152">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="7f354-152">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Product Type,Last Activated Date,Windows,Mac,Windows 10 Mobile,iOS,Android,Activated On Shared Computer
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
    "Error: /api-reference/v1.0/api/reportroot-getoffice365activationsuserdetail.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/reportroot-getoffice365activationsuserdetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/reportroot-getoffice365activationsuserdetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
