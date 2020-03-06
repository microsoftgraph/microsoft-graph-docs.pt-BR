---
title: 'reportRoot: getOneDriveUsageAccountDetail'
description: Obtenha dados sobre o uso do OneDrive por conta.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: d0cbf19fb5cc1b1f648138fc11ee62ec37fc4a03
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42510274"
---
# <a name="reportroot-getonedriveusageaccountdetail"></a><span data-ttu-id="ee4bc-103">reportRoot: getOneDriveUsageAccountDetail</span><span class="sxs-lookup"><span data-stu-id="ee4bc-103">reportRoot: getOneDriveUsageAccountDetail</span></span>

<span data-ttu-id="ee4bc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee4bc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ee4bc-105">Obtenha dados sobre o uso do OneDrive por conta.</span><span class="sxs-lookup"><span data-stu-id="ee4bc-105">Get details about OneDrive usage by account.</span></span>

> <span data-ttu-id="ee4bc-106">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso do OneDrive for Business](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span><span class="sxs-lookup"><span data-stu-id="ee4bc-106">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="ee4bc-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="ee4bc-107">Permissions</span></span>

<span data-ttu-id="ee4bc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee4bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ee4bc-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ee4bc-110">Permission type</span></span>                        | <span data-ttu-id="ee4bc-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ee4bc-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="ee4bc-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ee4bc-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="ee4bc-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ee4bc-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="ee4bc-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ee4bc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee4bc-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ee4bc-115">Not supported.</span></span>                           |
| <span data-ttu-id="ee4bc-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ee4bc-116">Application</span></span>                            | <span data-ttu-id="ee4bc-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ee4bc-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="ee4bc-118">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="ee4bc-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="ee4bc-119">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="ee4bc-119">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="ee4bc-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ee4bc-120">HTTP request</span></span>


<!-- { "blockType": "samples" } --> 

```http
GET /reports/getOneDriveUsageAccountDetail(period='{period_value}')
GET /reports/getOneDriveUsageAccountDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="ee4bc-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="ee4bc-121">Function parameters</span></span>

<span data-ttu-id="ee4bc-122">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="ee4bc-122">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="ee4bc-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="ee4bc-123">Parameter</span></span> | <span data-ttu-id="ee4bc-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="ee4bc-124">Type</span></span>   | <span data-ttu-id="ee4bc-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee4bc-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="ee4bc-126">ponto</span><span class="sxs-lookup"><span data-stu-id="ee4bc-126">period</span></span>    | <span data-ttu-id="ee4bc-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ee4bc-127">string</span></span> | <span data-ttu-id="ee4bc-128">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="ee4bc-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="ee4bc-129">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="ee4bc-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="ee4bc-130">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="ee4bc-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="ee4bc-131">data</span><span class="sxs-lookup"><span data-stu-id="ee4bc-131">date</span></span>      | <span data-ttu-id="ee4bc-132">Data</span><span class="sxs-lookup"><span data-stu-id="ee4bc-132">Date</span></span>   | <span data-ttu-id="ee4bc-133">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="ee4bc-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="ee4bc-134">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="ee4bc-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="ee4bc-135">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="ee4bc-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="ee4bc-136">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="ee4bc-136">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ee4bc-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ee4bc-137">Request headers</span></span>

| <span data-ttu-id="ee4bc-138">Nome</span><span class="sxs-lookup"><span data-stu-id="ee4bc-138">Name</span></span>          | <span data-ttu-id="ee4bc-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee4bc-139">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="ee4bc-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="ee4bc-140">Authorization</span></span> | <span data-ttu-id="ee4bc-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ee4bc-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="ee4bc-143">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="ee4bc-143">If-None-Match</span></span> | <span data-ttu-id="ee4bc-144">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="ee4bc-144">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="ee4bc-145">Opcional.</span><span class="sxs-lookup"><span data-stu-id="ee4bc-145">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="ee4bc-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee4bc-146">Response</span></span>

<span data-ttu-id="ee4bc-147">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="ee4bc-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="ee4bc-148">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="ee4bc-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="ee4bc-149">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="ee4bc-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="ee4bc-150">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="ee4bc-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="ee4bc-151">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="ee4bc-151">Report Refresh Date</span></span>
- <span data-ttu-id="ee4bc-152">URL do site</span><span class="sxs-lookup"><span data-stu-id="ee4bc-152">Site URL</span></span>
- <span data-ttu-id="ee4bc-153">Nome de exibição do proprietário</span><span class="sxs-lookup"><span data-stu-id="ee4bc-153">Owner Display Name</span></span>
- <span data-ttu-id="ee4bc-154">Excluído</span><span class="sxs-lookup"><span data-stu-id="ee4bc-154">Is Deleted</span></span>
- <span data-ttu-id="ee4bc-155">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="ee4bc-155">Last Activity Date</span></span>
- <span data-ttu-id="ee4bc-156">Contagem de arquivos</span><span class="sxs-lookup"><span data-stu-id="ee4bc-156">File Count</span></span>
- <span data-ttu-id="ee4bc-157">Contagem de arquivos ativos</span><span class="sxs-lookup"><span data-stu-id="ee4bc-157">Active File Count</span></span>
- <span data-ttu-id="ee4bc-158">Armazenamento utilizado (bytes)</span><span class="sxs-lookup"><span data-stu-id="ee4bc-158">Storage Used (Byte)</span></span>
- <span data-ttu-id="ee4bc-159">Armazenamento alocado (bytes)</span><span class="sxs-lookup"><span data-stu-id="ee4bc-159">Storage Allocated (Byte)</span></span>
- <span data-ttu-id="ee4bc-160">Nome principal do proprietário</span><span class="sxs-lookup"><span data-stu-id="ee4bc-160">Owner Principal Name</span></span>
- <span data-ttu-id="ee4bc-161">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="ee4bc-161">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="ee4bc-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ee4bc-162">Example</span></span>

#### <a name="request"></a><span data-ttu-id="ee4bc-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ee4bc-163">Request</span></span>

<span data-ttu-id="ee4bc-164">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ee4bc-164">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ee4bc-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="ee4bc-165">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getonedriveusageuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getOneDriveUsageAccountDetail(period='D7')
```
# <a name="c"></a>[<span data-ttu-id="ee4bc-166">C#</span><span class="sxs-lookup"><span data-stu-id="ee4bc-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getonedriveusageuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ee4bc-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ee4bc-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getonedriveusageuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ee4bc-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ee4bc-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getonedriveusageuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ee4bc-169">Java</span><span class="sxs-lookup"><span data-stu-id="ee4bc-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getonedriveusageuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ee4bc-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee4bc-170">Response</span></span>

<span data-ttu-id="ee4bc-171">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ee4bc-171">The following is an example of the response.</span></span>

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

<span data-ttu-id="ee4bc-172">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="ee4bc-172">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site URL,Owner Display Name,Is Deleted,Last Activity Date,File Count,Active File Count,Storage Used (Byte),Storage Allocated (Byte),Owner Principal Name,Report Period
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
