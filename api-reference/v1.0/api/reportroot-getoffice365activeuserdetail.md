---
title: 'reportRoot: getOffice365ActiveUserDetail'
description: Obtenha dados sobre os usuários ativos do Office 365.
localization_priority: Priority
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 9e5c28010aaed4aefd6d12b60fc16abde4fc1880
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42510344"
---
# <a name="reportroot-getoffice365activeuserdetail"></a><span data-ttu-id="a73d2-103">reportRoot: getOffice365ActiveUserDetail</span><span class="sxs-lookup"><span data-stu-id="a73d2-103">reportRoot: getOffice365ActiveUserDetail</span></span>

<span data-ttu-id="a73d2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a73d2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a73d2-105">Obtenha dados sobre os usuários ativos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="a73d2-105">Get details about Office 365 active users.</span></span>

> <span data-ttu-id="a73d2-106">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Usuários ativos](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="a73d2-106">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="a73d2-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="a73d2-107">Permissions</span></span>

<span data-ttu-id="a73d2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a73d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a73d2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a73d2-110">Permission type</span></span>                        | <span data-ttu-id="a73d2-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a73d2-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="a73d2-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a73d2-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="a73d2-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a73d2-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="a73d2-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a73d2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a73d2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a73d2-115">Not supported.</span></span>                           |
| <span data-ttu-id="a73d2-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a73d2-116">Application</span></span>                            | <span data-ttu-id="a73d2-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a73d2-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="a73d2-118">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="a73d2-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="a73d2-119">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="a73d2-119">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="a73d2-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a73d2-120">HTTP request</span></span>


<!-- { "blockType": "samples" } --> 

```http
GET /reports/getOffice365ActiveUserDetail(period='{period_value}')
GET /reports/getOffice365ActiveUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="a73d2-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="a73d2-121">Function parameters</span></span>

<span data-ttu-id="a73d2-122">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="a73d2-122">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="a73d2-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="a73d2-123">Parameter</span></span> | <span data-ttu-id="a73d2-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="a73d2-124">Type</span></span>   | <span data-ttu-id="a73d2-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="a73d2-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="a73d2-126">ponto</span><span class="sxs-lookup"><span data-stu-id="a73d2-126">period</span></span>    | <span data-ttu-id="a73d2-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a73d2-127">string</span></span> | <span data-ttu-id="a73d2-128">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="a73d2-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="a73d2-129">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="a73d2-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="a73d2-130">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="a73d2-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="a73d2-131">data</span><span class="sxs-lookup"><span data-stu-id="a73d2-131">date</span></span>      | <span data-ttu-id="a73d2-132">Data</span><span class="sxs-lookup"><span data-stu-id="a73d2-132">Date</span></span>   | <span data-ttu-id="a73d2-133">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="a73d2-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="a73d2-134">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="a73d2-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="a73d2-135">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="a73d2-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="a73d2-136">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="a73d2-136">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a73d2-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a73d2-137">Request headers</span></span>

| <span data-ttu-id="a73d2-138">Nome</span><span class="sxs-lookup"><span data-stu-id="a73d2-138">Name</span></span>          | <span data-ttu-id="a73d2-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="a73d2-139">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="a73d2-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="a73d2-140">Authorization</span></span> | <span data-ttu-id="a73d2-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a73d2-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="a73d2-143">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="a73d2-143">If-None-Match</span></span> | <span data-ttu-id="a73d2-144">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="a73d2-144">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="a73d2-145">Opcional.</span><span class="sxs-lookup"><span data-stu-id="a73d2-145">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="a73d2-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="a73d2-146">Response</span></span>

<span data-ttu-id="a73d2-147">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="a73d2-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="a73d2-148">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="a73d2-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="a73d2-149">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="a73d2-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="a73d2-150">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="a73d2-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="a73d2-151">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="a73d2-151">Report Refresh Date</span></span>
- <span data-ttu-id="a73d2-152">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="a73d2-152">User Principal Name</span></span>
- <span data-ttu-id="a73d2-153">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="a73d2-153">Display Name</span></span>
- <span data-ttu-id="a73d2-154">Excluído</span><span class="sxs-lookup"><span data-stu-id="a73d2-154">Is Deleted</span></span>
- <span data-ttu-id="a73d2-155">Data de exclusão</span><span class="sxs-lookup"><span data-stu-id="a73d2-155">Deleted Date</span></span>
- <span data-ttu-id="a73d2-156">Tem a licença do Exchange</span><span class="sxs-lookup"><span data-stu-id="a73d2-156">Has Exchange License</span></span>
- <span data-ttu-id="a73d2-157">Tem a licença do OneDrive</span><span class="sxs-lookup"><span data-stu-id="a73d2-157">Has OneDrive License</span></span>
- <span data-ttu-id="a73d2-158">Tem a licença do SharePoint</span><span class="sxs-lookup"><span data-stu-id="a73d2-158">Has SharePoint License</span></span>
- <span data-ttu-id="a73d2-159">Tem a licença do Skype for Business</span><span class="sxs-lookup"><span data-stu-id="a73d2-159">Has Skype For Business License</span></span>
- <span data-ttu-id="a73d2-160">Tem a licença do Yammer</span><span class="sxs-lookup"><span data-stu-id="a73d2-160">Has Yammer License</span></span>
- <span data-ttu-id="a73d2-161">Tem a licença do Teams</span><span class="sxs-lookup"><span data-stu-id="a73d2-161">Has Teams License</span></span>
- <span data-ttu-id="a73d2-162">Data da última atividade do Exchange</span><span class="sxs-lookup"><span data-stu-id="a73d2-162">Exchange Last Activity Date</span></span>
- <span data-ttu-id="a73d2-163">Data da última atividade do OneDrive</span><span class="sxs-lookup"><span data-stu-id="a73d2-163">OneDrive Last Activity Date</span></span>
- <span data-ttu-id="a73d2-164">Data da última atividade do SharePoint</span><span class="sxs-lookup"><span data-stu-id="a73d2-164">SharePoint Last Activity Date</span></span>
- <span data-ttu-id="a73d2-165">Data da última atividade do Skype for Business</span><span class="sxs-lookup"><span data-stu-id="a73d2-165">Skype For Business Last Activity Date</span></span>
- <span data-ttu-id="a73d2-166">Data da última atividade do Yammer</span><span class="sxs-lookup"><span data-stu-id="a73d2-166">Yammer Last Activity Date</span></span>
- <span data-ttu-id="a73d2-167">Data da última atividade do Teams</span><span class="sxs-lookup"><span data-stu-id="a73d2-167">Teams Last Activity Date</span></span>
- <span data-ttu-id="a73d2-168">Data de atribuição da licença do Exchange</span><span class="sxs-lookup"><span data-stu-id="a73d2-168">Exchange License Assign Date</span></span>
- <span data-ttu-id="a73d2-169">Data de atribuição da licença do OneDrive</span><span class="sxs-lookup"><span data-stu-id="a73d2-169">OneDrive License Assign Date</span></span>
- <span data-ttu-id="a73d2-170">Data de atribuição da licença do SharePoint</span><span class="sxs-lookup"><span data-stu-id="a73d2-170">SharePoint License Assign Date</span></span>
- <span data-ttu-id="a73d2-171">Data de atribuição da licença do Skype for Business</span><span class="sxs-lookup"><span data-stu-id="a73d2-171">Skype For Business License Assign Date</span></span>
- <span data-ttu-id="a73d2-172">Data de atribuição da licença do Yammer</span><span class="sxs-lookup"><span data-stu-id="a73d2-172">Yammer License Assign Date</span></span>
- <span data-ttu-id="a73d2-173">Data de atribuição da licença do Teams</span><span class="sxs-lookup"><span data-stu-id="a73d2-173">Teams License Assign Date</span></span>
- <span data-ttu-id="a73d2-174">Produtos Atribuídos</span><span class="sxs-lookup"><span data-stu-id="a73d2-174">Assigned Products</span></span>

## <a name="example"></a><span data-ttu-id="a73d2-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a73d2-175">Example</span></span>

#### <a name="request"></a><span data-ttu-id="a73d2-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a73d2-176">Request</span></span>

<span data-ttu-id="a73d2-177">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a73d2-177">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a73d2-178">HTTP</span><span class="sxs-lookup"><span data-stu-id="a73d2-178">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activeuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActiveUserDetail(period='D7')
```
# <a name="c"></a>[<span data-ttu-id="a73d2-179">C#</span><span class="sxs-lookup"><span data-stu-id="a73d2-179">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activeuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a73d2-180">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a73d2-180">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activeuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a73d2-181">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a73d2-181">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activeuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a73d2-182">Java</span><span class="sxs-lookup"><span data-stu-id="a73d2-182">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getoffice365activeuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a73d2-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="a73d2-183">Response</span></span>

<span data-ttu-id="a73d2-184">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a73d2-184">The following is an example of the response.</span></span>

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

<span data-ttu-id="a73d2-185">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="a73d2-185">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Has Exchange License,Has OneDrive License,Has SharePoint License,Has Skype For Business License,Has Yammer License,Has Teams License,Exchange Last Activity Date,OneDrive Last Activity Date,SharePoint Last Activity Date,Skype For Business Last Activity Date,Yammer Last Activity Date,Teams Last Activity Date,Exchange License Assign Date,OneDrive License Assign Date,SharePoint License Assign Date,Skype For Business License Assign Date,Yammer License Assign Date,Teams License Assign Date,Assigned Products
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
