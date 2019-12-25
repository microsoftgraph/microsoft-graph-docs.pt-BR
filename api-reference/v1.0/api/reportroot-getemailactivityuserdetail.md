---
title: 'reportRoot: getEmailActivityUserDetail'
description: Obtenha dados sobre as atividades de email que os usuários realizaram.
localization_priority: Priority
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 89985d1349a1f10811ce8fca7dbd393bad82f68e
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40864506"
---
# <a name="reportroot-getemailactivityuserdetail"></a><span data-ttu-id="ead5e-103">reportRoot: getEmailActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="ead5e-103">reportRoot: getEmailActivityUserDetail</span></span>

<span data-ttu-id="ead5e-104">Obtenha dados sobre as atividades de email que os usuários realizaram.</span><span class="sxs-lookup"><span data-stu-id="ead5e-104">Get details about email activity users have performed.</span></span>

> <span data-ttu-id="ead5e-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividades de email](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span><span class="sxs-lookup"><span data-stu-id="ead5e-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="permissions"></a><span data-ttu-id="ead5e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ead5e-106">Permissions</span></span>

<span data-ttu-id="ead5e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ead5e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ead5e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ead5e-109">Permission type</span></span>                        | <span data-ttu-id="ead5e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ead5e-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="ead5e-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ead5e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ead5e-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ead5e-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="ead5e-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ead5e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ead5e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ead5e-114">Not supported.</span></span>                           |
| <span data-ttu-id="ead5e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ead5e-115">Application</span></span>                            | <span data-ttu-id="ead5e-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ead5e-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="ead5e-117">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="ead5e-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="ead5e-118">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="ead5e-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="ead5e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ead5e-119">HTTP request</span></span>


<!-- { "blockType": "samples" } --> 

```http
GET /reports/getEmailActivityUserDetail(period='{period_value}')
GET /reports/getEmailActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="ead5e-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="ead5e-120">Function parameters</span></span>

<span data-ttu-id="ead5e-121">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="ead5e-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="ead5e-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="ead5e-122">Parameter</span></span> | <span data-ttu-id="ead5e-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="ead5e-123">Type</span></span>   | <span data-ttu-id="ead5e-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="ead5e-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="ead5e-125">ponto</span><span class="sxs-lookup"><span data-stu-id="ead5e-125">period</span></span>    | <span data-ttu-id="ead5e-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ead5e-126">string</span></span> | <span data-ttu-id="ead5e-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="ead5e-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="ead5e-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="ead5e-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="ead5e-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="ead5e-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="ead5e-130">data</span><span class="sxs-lookup"><span data-stu-id="ead5e-130">date</span></span>      | <span data-ttu-id="ead5e-131">Data</span><span class="sxs-lookup"><span data-stu-id="ead5e-131">Date</span></span>   | <span data-ttu-id="ead5e-132">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="ead5e-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="ead5e-133">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="ead5e-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="ead5e-134">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="ead5e-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="ead5e-135">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="ead5e-135">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ead5e-136">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ead5e-136">Request headers</span></span>

| <span data-ttu-id="ead5e-137">Nome</span><span class="sxs-lookup"><span data-stu-id="ead5e-137">Name</span></span>          | <span data-ttu-id="ead5e-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="ead5e-138">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="ead5e-139">Autorização</span><span class="sxs-lookup"><span data-stu-id="ead5e-139">Authorization</span></span> | <span data-ttu-id="ead5e-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ead5e-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="ead5e-142">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="ead5e-142">If-None-Match</span></span> | <span data-ttu-id="ead5e-143">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="ead5e-143">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="ead5e-144">Opcional.</span><span class="sxs-lookup"><span data-stu-id="ead5e-144">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="ead5e-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="ead5e-145">Response</span></span>

<span data-ttu-id="ead5e-146">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="ead5e-146">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="ead5e-147">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="ead5e-147">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="ead5e-148">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="ead5e-148">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="ead5e-149">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="ead5e-149">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="ead5e-150">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="ead5e-150">Report Refresh Date</span></span>
- <span data-ttu-id="ead5e-151">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="ead5e-151">User Principal Name</span></span>
- <span data-ttu-id="ead5e-152">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="ead5e-152">Display Name</span></span>
- <span data-ttu-id="ead5e-153">Excluído</span><span class="sxs-lookup"><span data-stu-id="ead5e-153">Is Deleted</span></span>
- <span data-ttu-id="ead5e-154">Data de exclusão</span><span class="sxs-lookup"><span data-stu-id="ead5e-154">Deleted Date</span></span>
- <span data-ttu-id="ead5e-155">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="ead5e-155">Last Activity Date</span></span>
- <span data-ttu-id="ead5e-156">Contagem de Envios</span><span class="sxs-lookup"><span data-stu-id="ead5e-156">Send Count</span></span>
- <span data-ttu-id="ead5e-157">Contagem de Recebimentos</span><span class="sxs-lookup"><span data-stu-id="ead5e-157">Receive Count</span></span>
- <span data-ttu-id="ead5e-158">Contagem de Leituras</span><span class="sxs-lookup"><span data-stu-id="ead5e-158">Read Count</span></span>
- <span data-ttu-id="ead5e-159">Produtos Atribuídos</span><span class="sxs-lookup"><span data-stu-id="ead5e-159">Assigned Products</span></span>
- <span data-ttu-id="ead5e-160">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="ead5e-160">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="ead5e-161">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ead5e-161">Example</span></span>

#### <a name="request"></a><span data-ttu-id="ead5e-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ead5e-162">Request</span></span>

<span data-ttu-id="ead5e-163">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ead5e-163">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="ead5e-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="ead5e-164">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getemailactivityuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getEmailActivityUserDetail(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ead5e-165">C#</span><span class="sxs-lookup"><span data-stu-id="ead5e-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getemailactivityuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ead5e-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ead5e-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getemailactivityuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ead5e-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ead5e-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getemailactivityuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ead5e-168">Java</span><span class="sxs-lookup"><span data-stu-id="ead5e-168">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getemailactivityuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ead5e-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="ead5e-169">Response</span></span>

<span data-ttu-id="ead5e-170">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ead5e-170">The following is an example of the response.</span></span>

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

<span data-ttu-id="ead5e-171">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="ead5e-171">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
