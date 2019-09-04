---
title: 'reportRoot: getOffice365ActivationsUserCounts'
description: Obtenha a contagem de usuários habilitados e aqueles que ativaram a assinatura do Office em desktops ou dispositivos ou computadores compartilhados.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 1f76e3e1f4baf54893d7c0073cd53f462f2917d2
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36728206"
---
# <a name="reportroot-getoffice365activationsusercounts"></a><span data-ttu-id="d6b63-103">reportRoot: getOffice365ActivationsUserCounts</span><span class="sxs-lookup"><span data-stu-id="d6b63-103">reportRoot: getOffice365ActivationsUserCounts</span></span>

<span data-ttu-id="d6b63-104">Obtenha a contagem de usuários habilitados e aqueles que ativaram a assinatura do Office em desktops ou dispositivos ou computadores compartilhados.</span><span class="sxs-lookup"><span data-stu-id="d6b63-104">Get the count of users that are enabled and those that have activated the Office subscription on desktop or devices or shared computers.</span></span>

> <span data-ttu-id="d6b63-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Ativações do Microsoft Office](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="d6b63-105">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="d6b63-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d6b63-106">Permissions</span></span>

<span data-ttu-id="d6b63-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6b63-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d6b63-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d6b63-109">Permission type</span></span>                        | <span data-ttu-id="d6b63-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d6b63-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="d6b63-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d6b63-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d6b63-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d6b63-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="d6b63-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d6b63-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d6b63-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d6b63-114">Not supported.</span></span>                           |
| <span data-ttu-id="d6b63-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d6b63-115">Application</span></span>                            | <span data-ttu-id="d6b63-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d6b63-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="d6b63-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d6b63-117">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserCounts
```

## <a name="request-headers"></a><span data-ttu-id="d6b63-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d6b63-118">Request headers</span></span>

| <span data-ttu-id="d6b63-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d6b63-119">Name</span></span>          | <span data-ttu-id="d6b63-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6b63-120">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="d6b63-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d6b63-121">Authorization</span></span> | <span data-ttu-id="d6b63-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d6b63-p102">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="d6b63-124">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="d6b63-124">If-None-Match</span></span> | <span data-ttu-id="d6b63-125">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="d6b63-125">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="d6b63-126">Opcional.</span><span class="sxs-lookup"><span data-stu-id="d6b63-126">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="d6b63-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6b63-127">Response</span></span>

<span data-ttu-id="d6b63-128">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="d6b63-128">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="d6b63-129">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="d6b63-129">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="d6b63-130">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="d6b63-130">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="d6b63-131">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="d6b63-131">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="d6b63-132">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="d6b63-132">Report Refresh Date</span></span>
- <span data-ttu-id="d6b63-133">Tipo de produto</span><span class="sxs-lookup"><span data-stu-id="d6b63-133">Product Type</span></span>
- <span data-ttu-id="d6b63-134">Atribuído</span><span class="sxs-lookup"><span data-stu-id="d6b63-134">Assigned</span></span>
- <span data-ttu-id="d6b63-135">Ativado</span><span class="sxs-lookup"><span data-stu-id="d6b63-135">Activated</span></span>
- <span data-ttu-id="d6b63-136">Ativação de computador compartilhado</span><span class="sxs-lookup"><span data-stu-id="d6b63-136">Shared Computer Activation</span></span>

## <a name="example"></a><span data-ttu-id="d6b63-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d6b63-137">Example</span></span>

#### <a name="request"></a><span data-ttu-id="d6b63-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d6b63-138">Request</span></span>

<span data-ttu-id="d6b63-139">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d6b63-139">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d6b63-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="d6b63-140">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activationsusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActivationsUserCounts
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d6b63-141">C#</span><span class="sxs-lookup"><span data-stu-id="d6b63-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activationsusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d6b63-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d6b63-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activationsusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d6b63-143">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="d6b63-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activationsusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d6b63-144">Java</span><span class="sxs-lookup"><span data-stu-id="d6b63-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getoffice365activationsusercounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d6b63-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6b63-145">Response</span></span>

<span data-ttu-id="d6b63-146">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d6b63-146">The following is an example of the response.</span></span>

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

<span data-ttu-id="d6b63-147">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="d6b63-147">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
  ]
}-->
