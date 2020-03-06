---
title: 'reportRoot: getEmailActivityUserDetail'
description: Obtenha dados sobre as atividades de email que os usuários realizaram.
localization_priority: Priority
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 668716a35554b0891a0fa52fd879b60df7cfa352
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42510435"
---
# <a name="reportroot-getemailactivityuserdetail"></a><span data-ttu-id="ea6e0-103">reportRoot: getEmailActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="ea6e0-103">reportRoot: getEmailActivityUserDetail</span></span>

<span data-ttu-id="ea6e0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea6e0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ea6e0-105">Obtenha dados sobre as atividades de email que os usuários realizaram.</span><span class="sxs-lookup"><span data-stu-id="ea6e0-105">Get details about email activity users have performed.</span></span>

> <span data-ttu-id="ea6e0-106">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividades de email](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span><span class="sxs-lookup"><span data-stu-id="ea6e0-106">**Note:** For details about different report views and names, see [Office 365 Reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="permissions"></a><span data-ttu-id="ea6e0-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="ea6e0-107">Permissions</span></span>

<span data-ttu-id="ea6e0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea6e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ea6e0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ea6e0-110">Permission type</span></span>                        | <span data-ttu-id="ea6e0-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ea6e0-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="ea6e0-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ea6e0-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="ea6e0-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ea6e0-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="ea6e0-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ea6e0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ea6e0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ea6e0-115">Not supported.</span></span>                           |
| <span data-ttu-id="ea6e0-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ea6e0-116">Application</span></span>                            | <span data-ttu-id="ea6e0-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ea6e0-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="ea6e0-118">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="ea6e0-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="ea6e0-119">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="ea6e0-119">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="ea6e0-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ea6e0-120">HTTP request</span></span>


<!-- { "blockType": "samples" } --> 

```http
GET /reports/getEmailActivityUserDetail(period='{period_value}')
GET /reports/getEmailActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="ea6e0-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="ea6e0-121">Function parameters</span></span>

<span data-ttu-id="ea6e0-122">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="ea6e0-122">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="ea6e0-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="ea6e0-123">Parameter</span></span> | <span data-ttu-id="ea6e0-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="ea6e0-124">Type</span></span>   | <span data-ttu-id="ea6e0-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea6e0-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="ea6e0-126">ponto</span><span class="sxs-lookup"><span data-stu-id="ea6e0-126">period</span></span>    | <span data-ttu-id="ea6e0-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ea6e0-127">string</span></span> | <span data-ttu-id="ea6e0-128">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="ea6e0-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="ea6e0-129">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="ea6e0-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="ea6e0-130">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="ea6e0-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="ea6e0-131">data</span><span class="sxs-lookup"><span data-stu-id="ea6e0-131">date</span></span>      | <span data-ttu-id="ea6e0-132">Data</span><span class="sxs-lookup"><span data-stu-id="ea6e0-132">Date</span></span>   | <span data-ttu-id="ea6e0-133">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="ea6e0-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="ea6e0-134">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="ea6e0-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="ea6e0-135">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="ea6e0-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="ea6e0-136">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="ea6e0-136">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ea6e0-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ea6e0-137">Request headers</span></span>

| <span data-ttu-id="ea6e0-138">Nome</span><span class="sxs-lookup"><span data-stu-id="ea6e0-138">Name</span></span>          | <span data-ttu-id="ea6e0-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea6e0-139">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="ea6e0-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="ea6e0-140">Authorization</span></span> | <span data-ttu-id="ea6e0-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ea6e0-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="ea6e0-143">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="ea6e0-143">If-None-Match</span></span> | <span data-ttu-id="ea6e0-144">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="ea6e0-144">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="ea6e0-145">Opcional.</span><span class="sxs-lookup"><span data-stu-id="ea6e0-145">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="ea6e0-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="ea6e0-146">Response</span></span>

<span data-ttu-id="ea6e0-147">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="ea6e0-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="ea6e0-148">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="ea6e0-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="ea6e0-149">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="ea6e0-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="ea6e0-150">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="ea6e0-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="ea6e0-151">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="ea6e0-151">Report Refresh Date</span></span>
- <span data-ttu-id="ea6e0-152">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="ea6e0-152">User Principal Name</span></span>
- <span data-ttu-id="ea6e0-153">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="ea6e0-153">Display Name</span></span>
- <span data-ttu-id="ea6e0-154">Excluído</span><span class="sxs-lookup"><span data-stu-id="ea6e0-154">Is Deleted</span></span>
- <span data-ttu-id="ea6e0-155">Data de exclusão</span><span class="sxs-lookup"><span data-stu-id="ea6e0-155">Deleted Date</span></span>
- <span data-ttu-id="ea6e0-156">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="ea6e0-156">Last Activity Date</span></span>
- <span data-ttu-id="ea6e0-157">Contagem de Envios</span><span class="sxs-lookup"><span data-stu-id="ea6e0-157">Send Count</span></span>
- <span data-ttu-id="ea6e0-158">Contagem de Recebimentos</span><span class="sxs-lookup"><span data-stu-id="ea6e0-158">Receive Count</span></span>
- <span data-ttu-id="ea6e0-159">Contagem de Leituras</span><span class="sxs-lookup"><span data-stu-id="ea6e0-159">Read Count</span></span>
- <span data-ttu-id="ea6e0-160">Produtos Atribuídos</span><span class="sxs-lookup"><span data-stu-id="ea6e0-160">Assigned Products</span></span>
- <span data-ttu-id="ea6e0-161">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="ea6e0-161">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="ea6e0-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ea6e0-162">Example</span></span>

#### <a name="request"></a><span data-ttu-id="ea6e0-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ea6e0-163">Request</span></span>

<span data-ttu-id="ea6e0-164">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ea6e0-164">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ea6e0-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="ea6e0-165">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getemailactivityuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getEmailActivityUserDetail(period='D7')
```
# <a name="c"></a>[<span data-ttu-id="ea6e0-166">C#</span><span class="sxs-lookup"><span data-stu-id="ea6e0-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getemailactivityuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ea6e0-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ea6e0-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getemailactivityuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ea6e0-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ea6e0-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getemailactivityuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ea6e0-169">Java</span><span class="sxs-lookup"><span data-stu-id="ea6e0-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getemailactivityuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ea6e0-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="ea6e0-170">Response</span></span>

<span data-ttu-id="ea6e0-171">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ea6e0-171">The following is an example of the response.</span></span>

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

<span data-ttu-id="ea6e0-172">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="ea6e0-172">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Last Activity Date,Send Count,Receive Count,Read Count,Assigned Products,Report Period
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
