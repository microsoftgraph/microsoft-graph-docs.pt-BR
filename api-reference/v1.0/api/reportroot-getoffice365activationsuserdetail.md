---
title: 'reportRoot: getOffice365ActivationsUserDetail'
description: Obtenha dados sobre usuários que ativaram o Office 365.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: e403643b01315741cc28c19b32c1aed0b2409e6c
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865416"
---
# <a name="reportroot-getoffice365activationsuserdetail"></a><span data-ttu-id="92804-103">reportRoot: getOffice365ActivationsUserDetail</span><span class="sxs-lookup"><span data-stu-id="92804-103">reportRoot: getOffice365ActivationsUserDetail</span></span>

<span data-ttu-id="92804-104">Obtenha dados sobre usuários que ativaram o Office 365.</span><span class="sxs-lookup"><span data-stu-id="92804-104">Get details about users who have activated Office 365.</span></span>

> <span data-ttu-id="92804-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Ativações do Microsoft Office](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="92804-105">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="92804-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="92804-106">Permissions</span></span>

<span data-ttu-id="92804-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92804-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="92804-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="92804-109">Permission type</span></span>                        | <span data-ttu-id="92804-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="92804-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="92804-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="92804-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="92804-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="92804-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="92804-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="92804-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="92804-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="92804-114">Not supported.</span></span>                           |
| <span data-ttu-id="92804-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="92804-115">Application</span></span>                            | <span data-ttu-id="92804-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="92804-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="92804-117">**Observação**: para permissões delegadas para permitir que os aplicativos leiam relatórios de uso do serviço em nome de um usuário, o administrador do locatário deve ter atribuído ao usuário a função de administrador limitada do Azure ad apropriada.</span><span class="sxs-lookup"><span data-stu-id="92804-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="92804-118">Para obter mais detalhes, consulte [Authorization for APIs to read Office 365 Usage Reports](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="92804-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="92804-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="92804-119">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserDetail
```

## <a name="request-headers"></a><span data-ttu-id="92804-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="92804-120">Request headers</span></span>

| <span data-ttu-id="92804-121">Nome</span><span class="sxs-lookup"><span data-stu-id="92804-121">Name</span></span>          | <span data-ttu-id="92804-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="92804-122">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="92804-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="92804-123">Authorization</span></span> | <span data-ttu-id="92804-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="92804-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="92804-126">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="92804-126">If-None-Match</span></span> | <span data-ttu-id="92804-127">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="92804-127">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="92804-128">Opcional.</span><span class="sxs-lookup"><span data-stu-id="92804-128">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="92804-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="92804-129">Response</span></span>

<span data-ttu-id="92804-130">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="92804-130">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="92804-131">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="92804-131">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="92804-132">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="92804-132">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="92804-133">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="92804-133">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="92804-134">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="92804-134">Report Refresh Date</span></span>
- <span data-ttu-id="92804-135">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="92804-135">User Principal Name</span></span>
- <span data-ttu-id="92804-136">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="92804-136">Display Name</span></span>
- <span data-ttu-id="92804-137">Tipo de produto</span><span class="sxs-lookup"><span data-stu-id="92804-137">Product Type</span></span>
- <span data-ttu-id="92804-138">Data da última ativação</span><span class="sxs-lookup"><span data-stu-id="92804-138">Last Activated Date</span></span>
- <span data-ttu-id="92804-139">Windows</span><span class="sxs-lookup"><span data-stu-id="92804-139">Windows</span></span>
- <span data-ttu-id="92804-140">Mac</span><span class="sxs-lookup"><span data-stu-id="92804-140">Mac</span></span>
- <span data-ttu-id="92804-141">Windows 10 Mobile</span><span class="sxs-lookup"><span data-stu-id="92804-141">Windows 10 Mobile</span></span>
- <span data-ttu-id="92804-142">iOS</span><span class="sxs-lookup"><span data-stu-id="92804-142">iOS</span></span>
- <span data-ttu-id="92804-143">Android</span><span class="sxs-lookup"><span data-stu-id="92804-143">Android</span></span>
- <span data-ttu-id="92804-144">Ativado no computador compartilhado</span><span class="sxs-lookup"><span data-stu-id="92804-144">Activated On Shared Computer</span></span>

## <a name="example"></a><span data-ttu-id="92804-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="92804-145">Example</span></span>

#### <a name="request"></a><span data-ttu-id="92804-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="92804-146">Request</span></span>

<span data-ttu-id="92804-147">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="92804-147">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="92804-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="92804-148">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activationsuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActivationsUserDetail
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="92804-149">C#</span><span class="sxs-lookup"><span data-stu-id="92804-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activationsuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="92804-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="92804-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activationsuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="92804-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="92804-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activationsuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="92804-152">Java</span><span class="sxs-lookup"><span data-stu-id="92804-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getoffice365activationsuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="92804-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="92804-153">Response</span></span>

<span data-ttu-id="92804-154">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="92804-154">The following is an example of the response.</span></span>

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

<span data-ttu-id="92804-155">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="92804-155">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
