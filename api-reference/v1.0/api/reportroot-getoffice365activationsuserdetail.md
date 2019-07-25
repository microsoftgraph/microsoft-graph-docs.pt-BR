---
title: 'reportRoot: getOffice365ActivationsUserDetail'
description: Obtenha dados sobre usuários que ativaram o Office 365.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 9df409f6dbe3943a2adda64953e9be10e43bc4e1
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35881047"
---
# <a name="reportroot-getoffice365activationsuserdetail"></a><span data-ttu-id="c8ab9-103">reportRoot: getOffice365ActivationsUserDetail</span><span class="sxs-lookup"><span data-stu-id="c8ab9-103">reportRoot: getOffice365ActivationsUserDetail</span></span>

<span data-ttu-id="c8ab9-104">Obtenha dados sobre usuários que ativaram o Office 365.</span><span class="sxs-lookup"><span data-stu-id="c8ab9-104">Get details about users who have activated Office 365.</span></span>

> <span data-ttu-id="c8ab9-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Ativações do Microsoft Office](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="c8ab9-105">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="c8ab9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c8ab9-106">Permissions</span></span>

<span data-ttu-id="c8ab9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8ab9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c8ab9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c8ab9-109">Permission type</span></span>                        | <span data-ttu-id="c8ab9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c8ab9-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="c8ab9-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c8ab9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c8ab9-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c8ab9-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="c8ab9-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c8ab9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c8ab9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c8ab9-114">Not supported.</span></span>                           |
| <span data-ttu-id="c8ab9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c8ab9-115">Application</span></span>                            | <span data-ttu-id="c8ab9-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c8ab9-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="c8ab9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c8ab9-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c8ab9-118">HTTP</span><span class="sxs-lookup"><span data-stu-id="c8ab9-118">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserDetail
```

## <a name="request-headers"></a><span data-ttu-id="c8ab9-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c8ab9-119">Request headers</span></span>

| <span data-ttu-id="c8ab9-120">Nome</span><span class="sxs-lookup"><span data-stu-id="c8ab9-120">Name</span></span>          | <span data-ttu-id="c8ab9-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="c8ab9-121">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="c8ab9-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c8ab9-122">Authorization</span></span> | <span data-ttu-id="c8ab9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c8ab9-p102">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="c8ab9-125">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="c8ab9-125">If-None-Match</span></span> | <span data-ttu-id="c8ab9-126">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="c8ab9-126">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="c8ab9-127">Opcional.</span><span class="sxs-lookup"><span data-stu-id="c8ab9-127">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="c8ab9-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="c8ab9-128">Response</span></span>

<span data-ttu-id="c8ab9-129">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="c8ab9-129">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="c8ab9-130">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="c8ab9-130">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="c8ab9-131">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="c8ab9-131">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="c8ab9-132">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="c8ab9-132">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="c8ab9-133">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="c8ab9-133">Report Refresh Date</span></span>
- <span data-ttu-id="c8ab9-134">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="c8ab9-134">User Principal Name</span></span>
- <span data-ttu-id="c8ab9-135">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="c8ab9-135">Display Name</span></span>
- <span data-ttu-id="c8ab9-136">Tipo de produto</span><span class="sxs-lookup"><span data-stu-id="c8ab9-136">Product Type</span></span>
- <span data-ttu-id="c8ab9-137">Data da última ativação</span><span class="sxs-lookup"><span data-stu-id="c8ab9-137">Last Activated Date</span></span>
- <span data-ttu-id="c8ab9-138">Windows</span><span class="sxs-lookup"><span data-stu-id="c8ab9-138">Windows</span></span>
- <span data-ttu-id="c8ab9-139">Mac</span><span class="sxs-lookup"><span data-stu-id="c8ab9-139">Mac</span></span>
- <span data-ttu-id="c8ab9-140">Windows 10 Mobile</span><span class="sxs-lookup"><span data-stu-id="c8ab9-140">Windows 10 Mobile</span></span>
- <span data-ttu-id="c8ab9-141">iOS</span><span class="sxs-lookup"><span data-stu-id="c8ab9-141">iOS</span></span>
- <span data-ttu-id="c8ab9-142">Android</span><span class="sxs-lookup"><span data-stu-id="c8ab9-142">Android</span></span>
- <span data-ttu-id="c8ab9-143">Ativado no computador compartilhado</span><span class="sxs-lookup"><span data-stu-id="c8ab9-143">Activated On Shared Computer</span></span>

## <a name="example"></a><span data-ttu-id="c8ab9-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c8ab9-144">Example</span></span>

#### <a name="request"></a><span data-ttu-id="c8ab9-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c8ab9-145">Request</span></span>

<span data-ttu-id="c8ab9-146">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c8ab9-146">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activationsuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActivationsUserDetail
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c8ab9-147">C#</span><span class="sxs-lookup"><span data-stu-id="c8ab9-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activationsuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c8ab9-148">Javascript</span><span class="sxs-lookup"><span data-stu-id="c8ab9-148">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activationsuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c8ab9-149">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c8ab9-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activationsuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c8ab9-150">Java</span><span class="sxs-lookup"><span data-stu-id="c8ab9-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getoffice365activationsuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c8ab9-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="c8ab9-151">Response</span></span>

<span data-ttu-id="c8ab9-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c8ab9-152">The following is an example of the response.</span></span>

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

<span data-ttu-id="c8ab9-153">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="c8ab9-153">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
