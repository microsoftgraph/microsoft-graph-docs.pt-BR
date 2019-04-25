---
title: 'reportRoot: getOneDriveActivityUserDetail'
description: Obtenha dados sobre as atividades do OneDrive por usuário.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 2349aaec209f64f5e447731faa9d77ba8787a44d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32574226"
---
# <a name="reportroot-getonedriveactivityuserdetail"></a><span data-ttu-id="aecca-103">reportRoot: getOneDriveActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="aecca-103">reportRoot: getOneDriveActivityUserDetail</span></span>

<span data-ttu-id="aecca-104">Obtenha dados sobre as atividades do OneDrive por usuário.</span><span class="sxs-lookup"><span data-stu-id="aecca-104">Get details about OneDrive activity by user.</span></span>

> <span data-ttu-id="aecca-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do OneDrive for Business](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span><span class="sxs-lookup"><span data-stu-id="aecca-105">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="permissions"></a><span data-ttu-id="aecca-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="aecca-106">Permissions</span></span>

<span data-ttu-id="aecca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aecca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="aecca-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aecca-109">Permission type</span></span>                        | <span data-ttu-id="aecca-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="aecca-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="aecca-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aecca-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="aecca-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="aecca-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="aecca-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aecca-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aecca-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aecca-114">Not supported.</span></span>                           |
| <span data-ttu-id="aecca-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aecca-115">Application</span></span>                            | <span data-ttu-id="aecca-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="aecca-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="aecca-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aecca-117">HTTP request</span></span>

<!-- { "blockType": "samples" } --> 

```http
GET /reports/getOneDriveActivityUserDetail(period='{period_value}')
GET /reports/getOneDriveActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="aecca-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="aecca-118">Function parameters</span></span>

<span data-ttu-id="aecca-119">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="aecca-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="aecca-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="aecca-120">Parameter</span></span> | <span data-ttu-id="aecca-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="aecca-121">Type</span></span>   | <span data-ttu-id="aecca-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="aecca-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="aecca-123">ponto</span><span class="sxs-lookup"><span data-stu-id="aecca-123">period</span></span>    | <span data-ttu-id="aecca-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aecca-124">string</span></span> | <span data-ttu-id="aecca-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="aecca-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="aecca-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="aecca-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="aecca-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="aecca-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="aecca-128">data</span><span class="sxs-lookup"><span data-stu-id="aecca-128">date</span></span>      | <span data-ttu-id="aecca-129">Data</span><span class="sxs-lookup"><span data-stu-id="aecca-129">Date</span></span>   | <span data-ttu-id="aecca-130">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="aecca-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="aecca-131">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="aecca-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="aecca-132">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="aecca-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="aecca-133">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="aecca-133">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="aecca-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aecca-134">Request headers</span></span>

| <span data-ttu-id="aecca-135">Nome</span><span class="sxs-lookup"><span data-stu-id="aecca-135">Name</span></span>          | <span data-ttu-id="aecca-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="aecca-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="aecca-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="aecca-137">Authorization</span></span> | <span data-ttu-id="aecca-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aecca-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="aecca-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="aecca-140">If-None-Match</span></span> | <span data-ttu-id="aecca-141">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="aecca-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="aecca-142">Opcional.</span><span class="sxs-lookup"><span data-stu-id="aecca-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="aecca-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="aecca-143">Response</span></span>

<span data-ttu-id="aecca-144">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="aecca-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="aecca-145">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="aecca-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="aecca-146">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="aecca-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="aecca-147">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="aecca-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="aecca-148">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="aecca-148">Report Refresh Date</span></span>
- <span data-ttu-id="aecca-149">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="aecca-149">User Principal Name</span></span>
- <span data-ttu-id="aecca-150">Excluído</span><span class="sxs-lookup"><span data-stu-id="aecca-150">Is Deleted</span></span>
- <span data-ttu-id="aecca-151">Data de exclusão</span><span class="sxs-lookup"><span data-stu-id="aecca-151">Deleted Date</span></span>
- <span data-ttu-id="aecca-152">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="aecca-152">Last Activity Date</span></span>
- <span data-ttu-id="aecca-153">Contagem de arquivos exibidos ou editados</span><span class="sxs-lookup"><span data-stu-id="aecca-153">Viewed Or Edited File Count</span></span>
- <span data-ttu-id="aecca-154">Contagem de arquivos sincronizados</span><span class="sxs-lookup"><span data-stu-id="aecca-154">Synced File Count</span></span>
- <span data-ttu-id="aecca-155">Contagem de arquivos compartilhados internamente</span><span class="sxs-lookup"><span data-stu-id="aecca-155">Shared Internally File Count</span></span>
- <span data-ttu-id="aecca-156">Contagem de arquivos compartilhados externamente</span><span class="sxs-lookup"><span data-stu-id="aecca-156">Shared Externally File Count</span></span>
- <span data-ttu-id="aecca-157">Produtos Atribuídos</span><span class="sxs-lookup"><span data-stu-id="aecca-157">Assigned Products</span></span>
- <span data-ttu-id="aecca-158">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="aecca-158">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="aecca-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aecca-159">Example</span></span>

#### <a name="request"></a><span data-ttu-id="aecca-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aecca-160">Request</span></span>

<span data-ttu-id="aecca-161">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="aecca-161">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getonedriveactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOneDriveActivityUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="aecca-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="aecca-162">Response</span></span>

<span data-ttu-id="aecca-163">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="aecca-163">The following is an example of the response.</span></span>

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

<span data-ttu-id="aecca-164">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="aecca-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Is Deleted,Deleted Date,Last Activity Date,Viewed Or Edited File Count,Synced File Count,Shared Internally File Count,Shared Externally File Count,Assigned Products,Report Period
```
