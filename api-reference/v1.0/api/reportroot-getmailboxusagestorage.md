---
title: 'reportRoot: getMailboxUsageStorage'
description: Obtenha a quantidade de armazenamento usada em sua organização.
localization_priority: Normal
ms.openlocfilehash: 4fa3b10d2f654389d07f751513e2fed2e2c329ab
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822740"
---
# <a name="reportroot-getmailboxusagestorage"></a><span data-ttu-id="d639e-103">reportRoot: getMailboxUsageStorage</span><span class="sxs-lookup"><span data-stu-id="d639e-103">reportRoot: getMailboxUsageStorage</span></span>

<span data-ttu-id="d639e-104">Obtenha a quantidade de armazenamento usada em sua organização.</span><span class="sxs-lookup"><span data-stu-id="d639e-104">Get the amount of storage used in your organization.</span></span>

> <span data-ttu-id="d639e-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso da caixa de correio](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span><span class="sxs-lookup"><span data-stu-id="d639e-105">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="d639e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d639e-106">Permissions</span></span>

<span data-ttu-id="d639e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d639e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d639e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d639e-109">Permission type</span></span>                        | <span data-ttu-id="d639e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d639e-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="d639e-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d639e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d639e-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d639e-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="d639e-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d639e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d639e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d639e-114">Not supported.</span></span>                           |
| <span data-ttu-id="d639e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d639e-115">Application</span></span>                            | <span data-ttu-id="d639e-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d639e-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="d639e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d639e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageStorage(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="d639e-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="d639e-118">Function parameters</span></span>

<span data-ttu-id="d639e-119">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="d639e-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="d639e-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d639e-120">Parameter</span></span> | <span data-ttu-id="d639e-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="d639e-121">Type</span></span>   | <span data-ttu-id="d639e-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="d639e-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="d639e-123">ponto</span><span class="sxs-lookup"><span data-stu-id="d639e-123">period</span></span>    | <span data-ttu-id="d639e-124">string</span><span class="sxs-lookup"><span data-stu-id="d639e-124">string</span></span> | <span data-ttu-id="d639e-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="d639e-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="d639e-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="d639e-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="d639e-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="d639e-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="d639e-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d639e-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="d639e-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d639e-129">Request headers</span></span>

| <span data-ttu-id="d639e-130">Nome</span><span class="sxs-lookup"><span data-stu-id="d639e-130">Name</span></span>          | <span data-ttu-id="d639e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d639e-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="d639e-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="d639e-132">Authorization</span></span> | <span data-ttu-id="d639e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d639e-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="d639e-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="d639e-135">If-None-Match</span></span> | <span data-ttu-id="d639e-136">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="d639e-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="d639e-137">Opcional.</span><span class="sxs-lookup"><span data-stu-id="d639e-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="d639e-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="d639e-138">Response</span></span>

<span data-ttu-id="d639e-139">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="d639e-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="d639e-140">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="d639e-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="d639e-141">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="d639e-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="d639e-142">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="d639e-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="d639e-143">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="d639e-143">Report Refresh Date</span></span>
- <span data-ttu-id="d639e-144">Armazenamento utilizado (bytes)</span><span class="sxs-lookup"><span data-stu-id="d639e-144">Storage Used (Byte)</span></span>
- <span data-ttu-id="d639e-145">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="d639e-145">Report Date</span></span>
- <span data-ttu-id="d639e-146">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="d639e-146">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="d639e-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d639e-147">Example</span></span>

#### <a name="request"></a><span data-ttu-id="d639e-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d639e-148">Request</span></span>

<span data-ttu-id="d639e-149">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d639e-149">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getmailboxusagestorage"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getMailboxUsageStorage(period='D7')
```

#### <a name="response"></a><span data-ttu-id="d639e-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="d639e-150">Response</span></span>

<span data-ttu-id="d639e-151">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d639e-151">The following is an example of the response.</span></span>

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

<span data-ttu-id="d639e-152">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="d639e-152">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Storage Used (Byte),Report Date,Report Period
```
