---
title: 'reportRoot: getTeamsUserActivityUserDetail'
description: Obter detalhes sobre a atividade de usuário do Microsoft Teams por usuário.
localization_priority: Priority
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: e432abf6e1b6d8cc0906709319543a1c7905771d
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33603548"
---
# <a name="reportroot-getteamsuseractivityuserdetail"></a><span data-ttu-id="bb56e-103">reportRoot: getTeamsUserActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="bb56e-103">reportRoot: getTeamsUserActivityUserDetail</span></span>

<span data-ttu-id="bb56e-104">Obtém detalhes sobre a atividade de usuários do Microsoft Teams por usuário.</span><span class="sxs-lookup"><span data-stu-id="bb56e-104">Get details about Microsoft Teams user activity by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="bb56e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="bb56e-105">Permissions</span></span>

<span data-ttu-id="bb56e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb56e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bb56e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bb56e-108">Permission type</span></span>                        | <span data-ttu-id="bb56e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bb56e-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="bb56e-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bb56e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="bb56e-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="bb56e-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="bb56e-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bb56e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bb56e-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bb56e-113">Not supported.</span></span>                           |
| <span data-ttu-id="bb56e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bb56e-114">Application</span></span>                            | <span data-ttu-id="bb56e-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="bb56e-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="bb56e-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bb56e-116">HTTP request</span></span>

<!-- { "blockType": "samples" } -->

```http
GET /reports/getTeamsUserActivityUserDetail(period='{period_value}')
GET /reports/getTeamsUserActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="bb56e-117">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="bb56e-117">Function parameters</span></span>

<span data-ttu-id="bb56e-118">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="bb56e-118">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="bb56e-119">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="bb56e-119">Parameter</span></span> | <span data-ttu-id="bb56e-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="bb56e-120">Type</span></span>   | <span data-ttu-id="bb56e-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb56e-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="bb56e-122">ponto</span><span class="sxs-lookup"><span data-stu-id="bb56e-122">period</span></span>    | <span data-ttu-id="bb56e-123">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bb56e-123">string</span></span> | <span data-ttu-id="bb56e-124">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="bb56e-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="bb56e-125">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="bb56e-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="bb56e-126">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="bb56e-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="bb56e-127">data</span><span class="sxs-lookup"><span data-stu-id="bb56e-127">date</span></span>      | <span data-ttu-id="bb56e-128">Data</span><span class="sxs-lookup"><span data-stu-id="bb56e-128">Date</span></span>   | <span data-ttu-id="bb56e-129">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="bb56e-129">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="bb56e-130">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="bb56e-130">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="bb56e-131">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="bb56e-131">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="bb56e-132">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="bb56e-132">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bb56e-133">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bb56e-133">Request headers</span></span>

| <span data-ttu-id="bb56e-134">Nome</span><span class="sxs-lookup"><span data-stu-id="bb56e-134">Name</span></span>          | <span data-ttu-id="bb56e-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb56e-135">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="bb56e-136">Autorização</span><span class="sxs-lookup"><span data-stu-id="bb56e-136">Authorization</span></span> | <span data-ttu-id="bb56e-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bb56e-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="bb56e-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb56e-139">Response</span></span>

<span data-ttu-id="bb56e-140">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="bb56e-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="bb56e-141">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="bb56e-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="bb56e-142">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="bb56e-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="bb56e-143">O arquivo CSV possui os seguintes cabeçalhos para colunas:</span><span class="sxs-lookup"><span data-stu-id="bb56e-143">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="bb56e-144">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="bb56e-144">Report Refresh Date</span></span>
- <span data-ttu-id="bb56e-145">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="bb56e-145">User Principal Name</span></span>
- <span data-ttu-id="bb56e-146">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="bb56e-146">Last Activity Date</span></span>
- <span data-ttu-id="bb56e-147">Excluído</span><span class="sxs-lookup"><span data-stu-id="bb56e-147">Is Deleted</span></span>
- <span data-ttu-id="bb56e-148">Data de exclusão</span><span class="sxs-lookup"><span data-stu-id="bb56e-148">Deleted Date</span></span>
- <span data-ttu-id="bb56e-149">Produtos Atribuídos</span><span class="sxs-lookup"><span data-stu-id="bb56e-149">Assigned Products</span></span>
- <span data-ttu-id="bb56e-150">Número de mensagens de chat de equipe</span><span class="sxs-lookup"><span data-stu-id="bb56e-150">Team Chat Message Count</span></span>
- <span data-ttu-id="bb56e-151">Contagem de mensagens de chat privadas</span><span class="sxs-lookup"><span data-stu-id="bb56e-151">Private Chat Message Count</span></span>
- <span data-ttu-id="bb56e-152">Contagem de chamadas</span><span class="sxs-lookup"><span data-stu-id="bb56e-152">Call Count</span></span>
- <span data-ttu-id="bb56e-153">Contagem de reuniões</span><span class="sxs-lookup"><span data-stu-id="bb56e-153">Meeting Count</span></span>
- <span data-ttu-id="bb56e-154">Tem outra ação</span><span class="sxs-lookup"><span data-stu-id="bb56e-154">Has Other Action</span></span>
- <span data-ttu-id="bb56e-155">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="bb56e-155">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="bb56e-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bb56e-156">Example</span></span>

#### <a name="request"></a><span data-ttu-id="bb56e-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bb56e-157">Request</span></span>

<span data-ttu-id="bb56e-158">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bb56e-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getTeamsUserActivityUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="bb56e-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb56e-159">Response</span></span>

<span data-ttu-id="bb56e-160">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bb56e-160">The following is an example of the response.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="bb56e-161">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="bb56e-161">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="bb56e-162">C#</span><span class="sxs-lookup"><span data-stu-id="bb56e-162">C</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getteamsuseractivityuserdetail-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bb56e-163">Javascript</span><span class="sxs-lookup"><span data-stu-id="bb56e-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getteamsuseractivityuserdetail-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="bb56e-164">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="bb56e-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Last Activity Date,Is Deleted,Deleted Date,Assigned Products,Team Chat Message Count,Private Chat Message Count,Call Count,Meeting Count,Has Other Action,Report Period
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
    "Error: /api-reference/v1.0/api/reportroot-getteamsuseractivityuserdetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/reportroot-getteamsuseractivityuserdetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
