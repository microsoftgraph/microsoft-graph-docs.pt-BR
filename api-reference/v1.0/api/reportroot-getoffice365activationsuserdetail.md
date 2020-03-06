---
title: 'reportRoot: getOffice365ActivationsUserDetail'
description: Obtenha dados sobre usuários que ativaram o Office 365.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 05c8d9385a9b79e38a57dbbb179cfbdb1b95f29d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42510358"
---
# <a name="reportroot-getoffice365activationsuserdetail"></a><span data-ttu-id="74df4-103">reportRoot: getOffice365ActivationsUserDetail</span><span class="sxs-lookup"><span data-stu-id="74df4-103">reportRoot: getOffice365ActivationsUserDetail</span></span>

<span data-ttu-id="74df4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74df4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="74df4-105">Obtenha dados sobre usuários que ativaram o Office 365.</span><span class="sxs-lookup"><span data-stu-id="74df4-105">Get details about users who have activated Office 365.</span></span>

> <span data-ttu-id="74df4-106">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Ativações do Microsoft Office](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="74df4-106">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="74df4-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="74df4-107">Permissions</span></span>

<span data-ttu-id="74df4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74df4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="74df4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="74df4-110">Permission type</span></span>                        | <span data-ttu-id="74df4-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="74df4-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="74df4-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="74df4-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="74df4-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="74df4-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="74df4-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="74df4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74df4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="74df4-115">Not supported.</span></span>                           |
| <span data-ttu-id="74df4-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="74df4-116">Application</span></span>                            | <span data-ttu-id="74df4-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="74df4-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="74df4-118">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="74df4-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="74df4-119">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="74df4-119">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="74df4-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="74df4-120">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserDetail
```

## <a name="request-headers"></a><span data-ttu-id="74df4-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="74df4-121">Request headers</span></span>

| <span data-ttu-id="74df4-122">Nome</span><span class="sxs-lookup"><span data-stu-id="74df4-122">Name</span></span>          | <span data-ttu-id="74df4-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="74df4-123">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="74df4-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="74df4-124">Authorization</span></span> | <span data-ttu-id="74df4-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="74df4-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="74df4-127">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="74df4-127">If-None-Match</span></span> | <span data-ttu-id="74df4-128">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="74df4-128">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="74df4-129">Opcional.</span><span class="sxs-lookup"><span data-stu-id="74df4-129">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="74df4-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="74df4-130">Response</span></span>

<span data-ttu-id="74df4-131">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="74df4-131">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="74df4-132">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="74df4-132">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="74df4-133">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="74df4-133">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="74df4-134">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="74df4-134">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="74df4-135">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="74df4-135">Report Refresh Date</span></span>
- <span data-ttu-id="74df4-136">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="74df4-136">User Principal Name</span></span>
- <span data-ttu-id="74df4-137">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="74df4-137">Display Name</span></span>
- <span data-ttu-id="74df4-138">Tipo de produto</span><span class="sxs-lookup"><span data-stu-id="74df4-138">Product Type</span></span>
- <span data-ttu-id="74df4-139">Data da última ativação</span><span class="sxs-lookup"><span data-stu-id="74df4-139">Last Activated Date</span></span>
- <span data-ttu-id="74df4-140">Windows</span><span class="sxs-lookup"><span data-stu-id="74df4-140">Windows</span></span>
- <span data-ttu-id="74df4-141">Mac</span><span class="sxs-lookup"><span data-stu-id="74df4-141">Mac</span></span>
- <span data-ttu-id="74df4-142">Windows 10 Mobile</span><span class="sxs-lookup"><span data-stu-id="74df4-142">Windows 10 Mobile</span></span>
- <span data-ttu-id="74df4-143">iOS</span><span class="sxs-lookup"><span data-stu-id="74df4-143">iOS</span></span>
- <span data-ttu-id="74df4-144">Android</span><span class="sxs-lookup"><span data-stu-id="74df4-144">Android</span></span>
- <span data-ttu-id="74df4-145">Ativado no computador compartilhado</span><span class="sxs-lookup"><span data-stu-id="74df4-145">Activated On Shared Computer</span></span>

## <a name="example"></a><span data-ttu-id="74df4-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="74df4-146">Example</span></span>

#### <a name="request"></a><span data-ttu-id="74df4-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="74df4-147">Request</span></span>

<span data-ttu-id="74df4-148">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="74df4-148">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="74df4-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="74df4-149">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activationsuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActivationsUserDetail
```
# <a name="c"></a>[<span data-ttu-id="74df4-150">C#</span><span class="sxs-lookup"><span data-stu-id="74df4-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activationsuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="74df4-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="74df4-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activationsuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="74df4-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="74df4-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activationsuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="74df4-153">Java</span><span class="sxs-lookup"><span data-stu-id="74df4-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getoffice365activationsuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="74df4-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="74df4-154">Response</span></span>

<span data-ttu-id="74df4-155">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="74df4-155">The following is an example of the response.</span></span>

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

<span data-ttu-id="74df4-156">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="74df4-156">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
