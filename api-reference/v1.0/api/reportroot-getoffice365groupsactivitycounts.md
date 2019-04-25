---
title: 'reportRoot: getOffice365GroupsActivityCounts'
description: Obtenha o número de atividades de grupo em todas as cargas de trabalho de grupo.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 8166a9c07809ce5fbd5544ed0576582a43787e63
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582220"
---
# <a name="reportroot-getoffice365groupsactivitycounts"></a><span data-ttu-id="91e87-103">reportRoot: getOffice365GroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="91e87-103">reportRoot: getOffice365GroupsActivityCounts</span></span>

<span data-ttu-id="91e87-104">Obtenha o número de atividades de grupo em todas as cargas de trabalho de grupo.</span><span class="sxs-lookup"><span data-stu-id="91e87-104">Get the number of group activities across group workloads.</span></span>

> <span data-ttu-id="91e87-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Grupos do Office 365](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span><span class="sxs-lookup"><span data-stu-id="91e87-105">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="91e87-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="91e87-106">Permissions</span></span>

<span data-ttu-id="91e87-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91e87-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="91e87-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="91e87-109">Permission type</span></span>                        | <span data-ttu-id="91e87-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="91e87-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="91e87-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="91e87-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="91e87-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="91e87-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="91e87-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="91e87-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91e87-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="91e87-114">Not supported.</span></span>                           |
| <span data-ttu-id="91e87-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="91e87-115">Application</span></span>                            | <span data-ttu-id="91e87-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="91e87-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="91e87-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="91e87-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="91e87-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="91e87-118">Function parameters</span></span>

<span data-ttu-id="91e87-119">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="91e87-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="91e87-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="91e87-120">Parameter</span></span> | <span data-ttu-id="91e87-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="91e87-121">Type</span></span>   | <span data-ttu-id="91e87-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="91e87-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="91e87-123">ponto</span><span class="sxs-lookup"><span data-stu-id="91e87-123">period</span></span>    | <span data-ttu-id="91e87-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="91e87-124">string</span></span> | <span data-ttu-id="91e87-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="91e87-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="91e87-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="91e87-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="91e87-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="91e87-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="91e87-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="91e87-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="91e87-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="91e87-129">Request headers</span></span>

| <span data-ttu-id="91e87-130">Nome</span><span class="sxs-lookup"><span data-stu-id="91e87-130">Name</span></span>          | <span data-ttu-id="91e87-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="91e87-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="91e87-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="91e87-132">Authorization</span></span> | <span data-ttu-id="91e87-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="91e87-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="91e87-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="91e87-135">If-None-Match</span></span> | <span data-ttu-id="91e87-136">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="91e87-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="91e87-137">Opcional.</span><span class="sxs-lookup"><span data-stu-id="91e87-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="91e87-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="91e87-138">Response</span></span>

<span data-ttu-id="91e87-139">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="91e87-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="91e87-140">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="91e87-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="91e87-141">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="91e87-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="91e87-142">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="91e87-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="91e87-143">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="91e87-143">Report Refresh Date</span></span>
- <span data-ttu-id="91e87-144">Emails recebidos do Exchange</span><span class="sxs-lookup"><span data-stu-id="91e87-144">Exchange Emails Received</span></span>
- <span data-ttu-id="91e87-145">Mensagens postadas do Yammer</span><span class="sxs-lookup"><span data-stu-id="91e87-145">Yammer Messages Posted</span></span>
- <span data-ttu-id="91e87-146">Mensagens lidas do Yammer</span><span class="sxs-lookup"><span data-stu-id="91e87-146">Yammer Messages Read</span></span>
- <span data-ttu-id="91e87-147">Mensagens curtidas do Yammer</span><span class="sxs-lookup"><span data-stu-id="91e87-147">Yammer Messages Liked</span></span>
- <span data-ttu-id="91e87-148">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="91e87-148">Report Date</span></span>
- <span data-ttu-id="91e87-149">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="91e87-149">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="91e87-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="91e87-150">Example</span></span>

#### <a name="request"></a><span data-ttu-id="91e87-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="91e87-151">Request</span></span>

<span data-ttu-id="91e87-152">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="91e87-152">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365groupsactivitycounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365GroupsActivityCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="91e87-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="91e87-153">Response</span></span>

<span data-ttu-id="91e87-154">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="91e87-154">The following is an example of the response.</span></span>

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

<span data-ttu-id="91e87-155">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="91e87-155">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Exchange Emails Received,Yammer Messages Posted,Yammer Messages Read,Yammer Messages Liked,Report Date,Report Period
```
