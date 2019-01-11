---
title: 'reportRoot: getOffice365GroupsActivityCounts'
description: Obtenha o número de atividades de grupo em todas as cargas de trabalho de grupo.
localization_priority: Normal
ms.openlocfilehash: d63655d136acee1d5d911e8e7b437560826043cf
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27846169"
---
# <a name="reportroot-getoffice365groupsactivitycounts"></a><span data-ttu-id="4c54b-103">reportRoot: getOffice365GroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="4c54b-103">reportRoot: getOffice365GroupsActivityCounts</span></span>

<span data-ttu-id="4c54b-104">Obtenha o número de atividades de grupo em todas as cargas de trabalho de grupo.</span><span class="sxs-lookup"><span data-stu-id="4c54b-104">Get the number of group activities across group workloads.</span></span>

> <span data-ttu-id="4c54b-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Grupos do Office 365](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span><span class="sxs-lookup"><span data-stu-id="4c54b-105">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="4c54b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4c54b-106">Permissions</span></span>

<span data-ttu-id="4c54b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c54b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4c54b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4c54b-109">Permission type</span></span>                        | <span data-ttu-id="4c54b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4c54b-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="4c54b-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4c54b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4c54b-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4c54b-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="4c54b-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4c54b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c54b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4c54b-114">Not supported.</span></span>                           |
| <span data-ttu-id="4c54b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4c54b-115">Application</span></span>                            | <span data-ttu-id="4c54b-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4c54b-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="4c54b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4c54b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="4c54b-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="4c54b-118">Function parameters</span></span>

<span data-ttu-id="4c54b-119">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="4c54b-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="4c54b-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="4c54b-120">Parameter</span></span> | <span data-ttu-id="4c54b-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="4c54b-121">Type</span></span>   | <span data-ttu-id="4c54b-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c54b-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="4c54b-123">ponto</span><span class="sxs-lookup"><span data-stu-id="4c54b-123">period</span></span>    | <span data-ttu-id="4c54b-124">string</span><span class="sxs-lookup"><span data-stu-id="4c54b-124">string</span></span> | <span data-ttu-id="4c54b-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="4c54b-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="4c54b-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="4c54b-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="4c54b-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="4c54b-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="4c54b-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4c54b-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="4c54b-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4c54b-129">Request headers</span></span>

| <span data-ttu-id="4c54b-130">Nome</span><span class="sxs-lookup"><span data-stu-id="4c54b-130">Name</span></span>          | <span data-ttu-id="4c54b-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c54b-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="4c54b-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="4c54b-132">Authorization</span></span> | <span data-ttu-id="4c54b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4c54b-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="4c54b-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="4c54b-135">If-None-Match</span></span> | <span data-ttu-id="4c54b-136">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="4c54b-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="4c54b-137">Opcional.</span><span class="sxs-lookup"><span data-stu-id="4c54b-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="4c54b-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c54b-138">Response</span></span>

<span data-ttu-id="4c54b-139">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="4c54b-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="4c54b-140">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="4c54b-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="4c54b-141">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="4c54b-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="4c54b-142">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="4c54b-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="4c54b-143">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="4c54b-143">Report Refresh Date</span></span>
- <span data-ttu-id="4c54b-144">Emails recebidos do Exchange</span><span class="sxs-lookup"><span data-stu-id="4c54b-144">Exchange Emails Received</span></span>
- <span data-ttu-id="4c54b-145">Mensagens postadas do Yammer</span><span class="sxs-lookup"><span data-stu-id="4c54b-145">Yammer Messages Posted</span></span>
- <span data-ttu-id="4c54b-146">Mensagens lidas do Yammer</span><span class="sxs-lookup"><span data-stu-id="4c54b-146">Yammer Messages Read</span></span>
- <span data-ttu-id="4c54b-147">Mensagens curtidas do Yammer</span><span class="sxs-lookup"><span data-stu-id="4c54b-147">Yammer Messages Liked</span></span>
- <span data-ttu-id="4c54b-148">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="4c54b-148">Report Date</span></span>
- <span data-ttu-id="4c54b-149">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="4c54b-149">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="4c54b-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4c54b-150">Example</span></span>

#### <a name="request"></a><span data-ttu-id="4c54b-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4c54b-151">Request</span></span>

<span data-ttu-id="4c54b-152">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4c54b-152">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365groupsactivitycounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365GroupsActivityCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="4c54b-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c54b-153">Response</span></span>

<span data-ttu-id="4c54b-154">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4c54b-154">The following is an example of the response.</span></span>

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

<span data-ttu-id="4c54b-155">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="4c54b-155">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Exchange Emails Received,Yammer Messages Posted,Yammer Messages Read,Yammer Messages Liked,Report Date,Report Period
```
