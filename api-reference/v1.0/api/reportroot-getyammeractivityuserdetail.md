---
title: 'reportRoot: getYammerActivityUserDetail'
description: Obtenha dados sobre as atividades do Yammer por usuário.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: cb3f46ddaf52f306fc6452b96f1534e7e921fffb
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44898286"
---
# <a name="reportroot-getyammeractivityuserdetail"></a><span data-ttu-id="081cb-103">reportRoot: getYammerActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="081cb-103">reportRoot: getYammerActivityUserDetail</span></span>

<span data-ttu-id="081cb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="081cb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="081cb-105">Obtenha dados sobre as atividades do Yammer por usuário.</span><span class="sxs-lookup"><span data-stu-id="081cb-105">Get details about Yammer activity by user.</span></span>

> <span data-ttu-id="081cb-106">**Observação:** Para obter detalhes sobre diferentes modos de exibição e nomes de relatórios, consulte [Microsoft 365 Reports-Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span><span class="sxs-lookup"><span data-stu-id="081cb-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="permissions"></a><span data-ttu-id="081cb-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="081cb-107">Permissions</span></span>

<span data-ttu-id="081cb-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="081cb-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="081cb-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="081cb-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="081cb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="081cb-110">Permission type</span></span>                        | <span data-ttu-id="081cb-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="081cb-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="081cb-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="081cb-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="081cb-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="081cb-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="081cb-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="081cb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="081cb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="081cb-115">Not supported.</span></span>                           |
| <span data-ttu-id="081cb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="081cb-116">Application</span></span>                            | <span data-ttu-id="081cb-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="081cb-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="081cb-118">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="081cb-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="081cb-119">Para obter mais detalhes, consulte [Authorization for APIs to read Microsoft 365 Usage Reports](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="081cb-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="081cb-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="081cb-120">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerActivityUserDetail(period='{period_value}')
GET /reports/getYammerActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="081cb-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="081cb-121">Function parameters</span></span>

<span data-ttu-id="081cb-122">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="081cb-122">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="081cb-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="081cb-123">Parameter</span></span> | <span data-ttu-id="081cb-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="081cb-124">Type</span></span>   | <span data-ttu-id="081cb-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="081cb-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="081cb-126">ponto</span><span class="sxs-lookup"><span data-stu-id="081cb-126">period</span></span>    | <span data-ttu-id="081cb-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="081cb-127">string</span></span> | <span data-ttu-id="081cb-128">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="081cb-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="081cb-129">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="081cb-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="081cb-130">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="081cb-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="081cb-131">data</span><span class="sxs-lookup"><span data-stu-id="081cb-131">date</span></span>      | <span data-ttu-id="081cb-132">Data</span><span class="sxs-lookup"><span data-stu-id="081cb-132">Date</span></span>   | <span data-ttu-id="081cb-133">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="081cb-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="081cb-134">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="081cb-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="081cb-135">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="081cb-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="081cb-136">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="081cb-136">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="081cb-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="081cb-137">Request headers</span></span>

| <span data-ttu-id="081cb-138">Nome</span><span class="sxs-lookup"><span data-stu-id="081cb-138">Name</span></span>          | <span data-ttu-id="081cb-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="081cb-139">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="081cb-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="081cb-140">Authorization</span></span> | <span data-ttu-id="081cb-141">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="081cb-141">Bearer {token}.</span></span> <span data-ttu-id="081cb-142">Required.</span><span class="sxs-lookup"><span data-stu-id="081cb-142">Required.</span></span>                |
| <span data-ttu-id="081cb-143">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="081cb-143">If-None-Match</span></span> | <span data-ttu-id="081cb-144">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="081cb-144">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="081cb-145">Opcional.</span><span class="sxs-lookup"><span data-stu-id="081cb-145">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="081cb-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="081cb-146">Response</span></span>

<span data-ttu-id="081cb-147">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="081cb-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="081cb-148">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="081cb-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="081cb-149">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="081cb-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="081cb-150">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="081cb-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="081cb-151">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="081cb-151">Report Refresh Date</span></span>
- <span data-ttu-id="081cb-152">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="081cb-152">User Principal Name</span></span>
- <span data-ttu-id="081cb-153">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="081cb-153">Display Name</span></span>
- <span data-ttu-id="081cb-154">Estado do usuário</span><span class="sxs-lookup"><span data-stu-id="081cb-154">User State</span></span>
- <span data-ttu-id="081cb-155">Data de alteração de estado</span><span class="sxs-lookup"><span data-stu-id="081cb-155">State Change Date</span></span>
- <span data-ttu-id="081cb-156">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="081cb-156">Last Activity Date</span></span>
- <span data-ttu-id="081cb-157">Contagem de Postagens</span><span class="sxs-lookup"><span data-stu-id="081cb-157">Posted Count</span></span>
- <span data-ttu-id="081cb-158">Contagem de Leituras</span><span class="sxs-lookup"><span data-stu-id="081cb-158">Read Count</span></span>
- <span data-ttu-id="081cb-159">Contagem de Curtidas</span><span class="sxs-lookup"><span data-stu-id="081cb-159">Liked Count</span></span>
- <span data-ttu-id="081cb-160">Produtos Atribuídos</span><span class="sxs-lookup"><span data-stu-id="081cb-160">Assigned Products</span></span>
- <span data-ttu-id="081cb-161">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="081cb-161">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="081cb-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="081cb-162">Example</span></span>

#### <a name="request"></a><span data-ttu-id="081cb-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="081cb-163">Request</span></span>

<span data-ttu-id="081cb-164">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="081cb-164">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getyammeractivityuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getYammerActivityUserDetail(period='D7')
```


#### <a name="response"></a><span data-ttu-id="081cb-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="081cb-165">Response</span></span>

<span data-ttu-id="081cb-166">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="081cb-166">The following is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.report" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

#### <a name="request"></a><span data-ttu-id="081cb-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="081cb-167">Request</span></span>

<span data-ttu-id="081cb-168">Se o `date` parâmetro for especificado, o relatório será delimitado às atividades que ocorreram na data especificada.</span><span class="sxs-lookup"><span data-stu-id="081cb-168">If the `date` parameter is specified, the report is scoped to activities that took place on the given date.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammeractivityuserdetail_date"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerActivityUserDetail(date='2018-03-05')
```

#### <a name="response"></a><span data-ttu-id="081cb-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="081cb-169">Response</span></span>

<span data-ttu-id="081cb-170">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="081cb-170">The following is an example of the response.</span></span>

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


<span data-ttu-id="081cb-171">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="081cb-171">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,User State,State Change Date,Last Activity Date,Posted Count,Read Count,Liked Count,Assigned Products,Report Period
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
