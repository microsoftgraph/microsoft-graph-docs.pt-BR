---
title: 'reportRoot: getMailboxUsageStorage'
description: Obtenha a quantidade de armazenamento usada em sua organização.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 2be6f83beda918419fa88488cc730c4f339f3f75
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42510379"
---
# <a name="reportroot-getmailboxusagestorage"></a><span data-ttu-id="5aa60-103">reportRoot: getMailboxUsageStorage</span><span class="sxs-lookup"><span data-stu-id="5aa60-103">reportRoot: getMailboxUsageStorage</span></span>

<span data-ttu-id="5aa60-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5aa60-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5aa60-105">Obtenha a quantidade de armazenamento usada em sua organização.</span><span class="sxs-lookup"><span data-stu-id="5aa60-105">Get the amount of storage used in your organization.</span></span>

> <span data-ttu-id="5aa60-106">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso da caixa de correio](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span><span class="sxs-lookup"><span data-stu-id="5aa60-106">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="5aa60-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="5aa60-107">Permissions</span></span>

<span data-ttu-id="5aa60-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5aa60-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5aa60-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5aa60-110">Permission type</span></span>                        | <span data-ttu-id="5aa60-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5aa60-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="5aa60-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5aa60-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="5aa60-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5aa60-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="5aa60-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5aa60-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5aa60-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5aa60-115">Not supported.</span></span>                           |
| <span data-ttu-id="5aa60-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5aa60-116">Application</span></span>                            | <span data-ttu-id="5aa60-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5aa60-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="5aa60-118">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="5aa60-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="5aa60-119">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="5aa60-119">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="5aa60-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5aa60-120">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageStorage(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="5aa60-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="5aa60-121">Function parameters</span></span>

<span data-ttu-id="5aa60-122">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="5aa60-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="5aa60-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="5aa60-123">Parameter</span></span> | <span data-ttu-id="5aa60-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="5aa60-124">Type</span></span>   | <span data-ttu-id="5aa60-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="5aa60-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="5aa60-126">ponto</span><span class="sxs-lookup"><span data-stu-id="5aa60-126">period</span></span>    | <span data-ttu-id="5aa60-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5aa60-127">string</span></span> | <span data-ttu-id="5aa60-128">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="5aa60-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="5aa60-129">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="5aa60-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="5aa60-130">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="5aa60-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="5aa60-131">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5aa60-131">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="5aa60-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5aa60-132">Request headers</span></span>

| <span data-ttu-id="5aa60-133">Nome</span><span class="sxs-lookup"><span data-stu-id="5aa60-133">Name</span></span>          | <span data-ttu-id="5aa60-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="5aa60-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="5aa60-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="5aa60-135">Authorization</span></span> | <span data-ttu-id="5aa60-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5aa60-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="5aa60-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="5aa60-138">If-None-Match</span></span> | <span data-ttu-id="5aa60-139">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="5aa60-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="5aa60-140">Opcional.</span><span class="sxs-lookup"><span data-stu-id="5aa60-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="5aa60-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="5aa60-141">Response</span></span>

<span data-ttu-id="5aa60-142">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="5aa60-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="5aa60-143">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="5aa60-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="5aa60-144">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="5aa60-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="5aa60-145">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="5aa60-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="5aa60-146">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="5aa60-146">Report Refresh Date</span></span>
- <span data-ttu-id="5aa60-147">Armazenamento utilizado (bytes)</span><span class="sxs-lookup"><span data-stu-id="5aa60-147">Storage Used (Byte)</span></span>
- <span data-ttu-id="5aa60-148">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="5aa60-148">Report Date</span></span>
- <span data-ttu-id="5aa60-149">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="5aa60-149">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="5aa60-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5aa60-150">Example</span></span>

#### <a name="request"></a><span data-ttu-id="5aa60-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5aa60-151">Request</span></span>

<span data-ttu-id="5aa60-152">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5aa60-152">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="5aa60-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="5aa60-153">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getmailboxusagestorage"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getMailboxUsageStorage(period='D7')
```
# <a name="c"></a>[<span data-ttu-id="5aa60-154">C#</span><span class="sxs-lookup"><span data-stu-id="5aa60-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getmailboxusagestorage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5aa60-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5aa60-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getmailboxusagestorage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5aa60-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5aa60-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getmailboxusagestorage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5aa60-157">Java</span><span class="sxs-lookup"><span data-stu-id="5aa60-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getmailboxusagestorage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5aa60-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="5aa60-158">Response</span></span>

<span data-ttu-id="5aa60-159">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5aa60-159">The following is an example of the response.</span></span>

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

<span data-ttu-id="5aa60-160">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="5aa60-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Storage Used (Byte),Report Date,Report Period
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
