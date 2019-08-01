---
title: 'reportRoot: getOffice365ActivationsUserCounts'
description: Obtenha a contagem de usuários habilitados e aqueles que ativaram a assinatura do Office em desktops ou dispositivos ou computadores compartilhados.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 0f6f27dcec75cf8a761fa4f8115962e3f444b923
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36025089"
---
# <a name="reportroot-getoffice365activationsusercounts"></a><span data-ttu-id="dff41-103">reportRoot: getOffice365ActivationsUserCounts</span><span class="sxs-lookup"><span data-stu-id="dff41-103">reportRoot: getOffice365ActivationsUserCounts</span></span>

<span data-ttu-id="dff41-104">Obtenha a contagem de usuários habilitados e aqueles que ativaram a assinatura do Office em desktops ou dispositivos ou computadores compartilhados.</span><span class="sxs-lookup"><span data-stu-id="dff41-104">Get the count of users that are enabled and those that have activated the Office subscription on desktop or devices or shared computers.</span></span>

> <span data-ttu-id="dff41-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Ativações do Microsoft Office](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="dff41-105">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="dff41-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="dff41-106">Permissions</span></span>

<span data-ttu-id="dff41-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dff41-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dff41-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dff41-109">Permission type</span></span>                        | <span data-ttu-id="dff41-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dff41-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="dff41-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dff41-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="dff41-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="dff41-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="dff41-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dff41-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dff41-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dff41-114">Not supported.</span></span>                           |
| <span data-ttu-id="dff41-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dff41-115">Application</span></span>                            | <span data-ttu-id="dff41-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="dff41-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="dff41-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dff41-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="dff41-118">HTTP</span><span class="sxs-lookup"><span data-stu-id="dff41-118">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserCounts
```

## <a name="request-headers"></a><span data-ttu-id="dff41-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dff41-119">Request headers</span></span>

| <span data-ttu-id="dff41-120">Nome</span><span class="sxs-lookup"><span data-stu-id="dff41-120">Name</span></span>          | <span data-ttu-id="dff41-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="dff41-121">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="dff41-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="dff41-122">Authorization</span></span> | <span data-ttu-id="dff41-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dff41-p102">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="dff41-125">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="dff41-125">If-None-Match</span></span> | <span data-ttu-id="dff41-126">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="dff41-126">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="dff41-127">Opcional.</span><span class="sxs-lookup"><span data-stu-id="dff41-127">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="dff41-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="dff41-128">Response</span></span>

<span data-ttu-id="dff41-129">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="dff41-129">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="dff41-130">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="dff41-130">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="dff41-131">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="dff41-131">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="dff41-132">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="dff41-132">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="dff41-133">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="dff41-133">Report Refresh Date</span></span>
- <span data-ttu-id="dff41-134">Tipo de produto</span><span class="sxs-lookup"><span data-stu-id="dff41-134">Product Type</span></span>
- <span data-ttu-id="dff41-135">Atribuído</span><span class="sxs-lookup"><span data-stu-id="dff41-135">Assigned</span></span>
- <span data-ttu-id="dff41-136">Ativado</span><span class="sxs-lookup"><span data-stu-id="dff41-136">Activated</span></span>
- <span data-ttu-id="dff41-137">Ativação de computador compartilhado</span><span class="sxs-lookup"><span data-stu-id="dff41-137">Shared Computer Activation</span></span>

## <a name="example"></a><span data-ttu-id="dff41-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dff41-138">Example</span></span>

#### <a name="request"></a><span data-ttu-id="dff41-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dff41-139">Request</span></span>

<span data-ttu-id="dff41-140">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="dff41-140">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activationsusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActivationsUserCounts
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="dff41-141">C#</span><span class="sxs-lookup"><span data-stu-id="dff41-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activationsusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dff41-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="dff41-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activationsusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dff41-143">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="dff41-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activationsusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="dff41-144">Java</span><span class="sxs-lookup"><span data-stu-id="dff41-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getoffice365activationsusercounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="dff41-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="dff41-145">Response</span></span>

<span data-ttu-id="dff41-146">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="dff41-146">The following is an example of the response.</span></span>

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

<span data-ttu-id="dff41-147">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="dff41-147">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
