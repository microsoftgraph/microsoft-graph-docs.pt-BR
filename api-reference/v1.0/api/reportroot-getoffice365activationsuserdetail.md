---
title: 'reportRoot: getOffice365ActivationsUserDetail'
description: Obtenha dados sobre usuários que ativaram o Office 365.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: e3171ed3e6e62758828cc37a1e2f2e494a22b8a9
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36729711"
---
# <a name="reportroot-getoffice365activationsuserdetail"></a><span data-ttu-id="def11-103">reportRoot: getOffice365ActivationsUserDetail</span><span class="sxs-lookup"><span data-stu-id="def11-103">reportRoot: getOffice365ActivationsUserDetail</span></span>

<span data-ttu-id="def11-104">Obtenha dados sobre usuários que ativaram o Office 365.</span><span class="sxs-lookup"><span data-stu-id="def11-104">Get details about users who have activated Office 365.</span></span>

> <span data-ttu-id="def11-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Ativações do Microsoft Office](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="def11-105">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="def11-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="def11-106">Permissions</span></span>

<span data-ttu-id="def11-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="def11-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="def11-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="def11-109">Permission type</span></span>                        | <span data-ttu-id="def11-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="def11-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="def11-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="def11-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="def11-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="def11-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="def11-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="def11-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="def11-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="def11-114">Not supported.</span></span>                           |
| <span data-ttu-id="def11-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="def11-115">Application</span></span>                            | <span data-ttu-id="def11-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="def11-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="def11-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="def11-117">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserDetail
```

## <a name="request-headers"></a><span data-ttu-id="def11-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="def11-118">Request headers</span></span>

| <span data-ttu-id="def11-119">Nome</span><span class="sxs-lookup"><span data-stu-id="def11-119">Name</span></span>          | <span data-ttu-id="def11-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="def11-120">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="def11-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="def11-121">Authorization</span></span> | <span data-ttu-id="def11-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="def11-p102">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="def11-124">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="def11-124">If-None-Match</span></span> | <span data-ttu-id="def11-125">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="def11-125">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="def11-126">Opcional.</span><span class="sxs-lookup"><span data-stu-id="def11-126">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="def11-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="def11-127">Response</span></span>

<span data-ttu-id="def11-128">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="def11-128">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="def11-129">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="def11-129">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="def11-130">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="def11-130">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="def11-131">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="def11-131">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="def11-132">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="def11-132">Report Refresh Date</span></span>
- <span data-ttu-id="def11-133">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="def11-133">User Principal Name</span></span>
- <span data-ttu-id="def11-134">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="def11-134">Display Name</span></span>
- <span data-ttu-id="def11-135">Tipo de produto</span><span class="sxs-lookup"><span data-stu-id="def11-135">Product Type</span></span>
- <span data-ttu-id="def11-136">Data da última ativação</span><span class="sxs-lookup"><span data-stu-id="def11-136">Last Activated Date</span></span>
- <span data-ttu-id="def11-137">Windows</span><span class="sxs-lookup"><span data-stu-id="def11-137">Windows</span></span>
- <span data-ttu-id="def11-138">Mac</span><span class="sxs-lookup"><span data-stu-id="def11-138">Mac</span></span>
- <span data-ttu-id="def11-139">Windows 10 Mobile</span><span class="sxs-lookup"><span data-stu-id="def11-139">Windows 10 Mobile</span></span>
- <span data-ttu-id="def11-140">iOS</span><span class="sxs-lookup"><span data-stu-id="def11-140">iOS</span></span>
- <span data-ttu-id="def11-141">Android</span><span class="sxs-lookup"><span data-stu-id="def11-141">Android</span></span>
- <span data-ttu-id="def11-142">Ativado no computador compartilhado</span><span class="sxs-lookup"><span data-stu-id="def11-142">Activated On Shared Computer</span></span>

## <a name="example"></a><span data-ttu-id="def11-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="def11-143">Example</span></span>

#### <a name="request"></a><span data-ttu-id="def11-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="def11-144">Request</span></span>

<span data-ttu-id="def11-145">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="def11-145">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="def11-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="def11-146">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activationsuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActivationsUserDetail
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="def11-147">C#</span><span class="sxs-lookup"><span data-stu-id="def11-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activationsuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="def11-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="def11-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activationsuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="def11-149">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="def11-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activationsuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="def11-150">Java</span><span class="sxs-lookup"><span data-stu-id="def11-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getoffice365activationsuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="def11-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="def11-151">Response</span></span>

<span data-ttu-id="def11-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="def11-152">The following is an example of the response.</span></span>

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

<span data-ttu-id="def11-153">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="def11-153">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
  ]
}-->
