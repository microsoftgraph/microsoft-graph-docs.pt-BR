---
title: 'reportRoot: getSkypeForBusinessActivityUserCounts'
description: Obtenha as tendências de quantos usuários únicos organizaram e participaram de sessões de conferência realizadas em sua organização através do Skype for Business. O relatório também inclui o número de sessões ponto a ponto.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 0d39f96a27bdbf8a81c660621728b4ff6e821a98
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572819"
---
# <a name="reportroot-getskypeforbusinessactivityusercounts"></a><span data-ttu-id="93fdc-104">reportRoot: getSkypeForBusinessActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="93fdc-104">reportRoot: getSkypeForBusinessActivityUserCounts</span></span>

<span data-ttu-id="93fdc-105">Obtenha as tendências de quantos usuários únicos organizaram e participaram de sessões de conferência realizadas em sua organização através do Skype for Business.</span><span class="sxs-lookup"><span data-stu-id="93fdc-105">Get the trends on how many unique users organized and participated in conference sessions held in your organization through Skype for Business.</span></span> <span data-ttu-id="93fdc-106">O relatório também inclui o número de sessões ponto a ponto.</span><span class="sxs-lookup"><span data-stu-id="93fdc-106">The report also includes the number of peer-to-peer sessions.</span></span>

> <span data-ttu-id="93fdc-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do Skype for Business](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span><span class="sxs-lookup"><span data-stu-id="93fdc-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="permissions"></a><span data-ttu-id="93fdc-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="93fdc-108">Permissions</span></span>

<span data-ttu-id="93fdc-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93fdc-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="93fdc-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="93fdc-111">Permission type</span></span>                        | <span data-ttu-id="93fdc-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="93fdc-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="93fdc-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="93fdc-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="93fdc-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="93fdc-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="93fdc-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="93fdc-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="93fdc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="93fdc-116">Not supported.</span></span>                           |
| <span data-ttu-id="93fdc-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="93fdc-117">Application</span></span>                            | <span data-ttu-id="93fdc-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="93fdc-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="93fdc-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="93fdc-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="93fdc-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="93fdc-120">Function parameters</span></span>

<span data-ttu-id="93fdc-121">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="93fdc-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="93fdc-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="93fdc-122">Parameter</span></span> | <span data-ttu-id="93fdc-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="93fdc-123">Type</span></span>   | <span data-ttu-id="93fdc-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="93fdc-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="93fdc-125">ponto</span><span class="sxs-lookup"><span data-stu-id="93fdc-125">period</span></span>    | <span data-ttu-id="93fdc-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="93fdc-126">string</span></span> | <span data-ttu-id="93fdc-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="93fdc-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="93fdc-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="93fdc-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="93fdc-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="93fdc-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="93fdc-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="93fdc-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="93fdc-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="93fdc-131">Request headers</span></span>

| <span data-ttu-id="93fdc-132">Nome</span><span class="sxs-lookup"><span data-stu-id="93fdc-132">Name</span></span>          | <span data-ttu-id="93fdc-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="93fdc-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="93fdc-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="93fdc-134">Authorization</span></span> | <span data-ttu-id="93fdc-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="93fdc-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="93fdc-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="93fdc-137">If-None-Match</span></span> | <span data-ttu-id="93fdc-138">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="93fdc-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="93fdc-139">Opcional.</span><span class="sxs-lookup"><span data-stu-id="93fdc-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="93fdc-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="93fdc-140">Response</span></span>

<span data-ttu-id="93fdc-141">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="93fdc-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="93fdc-142">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="93fdc-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="93fdc-143">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="93fdc-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="93fdc-144">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="93fdc-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="93fdc-145">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="93fdc-145">Report Refresh Date</span></span>
- <span data-ttu-id="93fdc-146">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="93fdc-146">Report Date</span></span>
- <span data-ttu-id="93fdc-147">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="93fdc-147">Report Period</span></span>
- <span data-ttu-id="93fdc-148">Ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="93fdc-148">Peer-to-peer</span></span>
- <span data-ttu-id="93fdc-149">Organizadas</span><span class="sxs-lookup"><span data-stu-id="93fdc-149">Organized</span></span>
- <span data-ttu-id="93fdc-150">Participadas</span><span class="sxs-lookup"><span data-stu-id="93fdc-150">Participated</span></span>

## <a name="example"></a><span data-ttu-id="93fdc-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="93fdc-151">Example</span></span>

#### <a name="request"></a><span data-ttu-id="93fdc-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="93fdc-152">Request</span></span>

<span data-ttu-id="93fdc-153">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="93fdc-153">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessactivityusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessActivityUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="93fdc-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="93fdc-154">Response</span></span>

<span data-ttu-id="93fdc-155">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="93fdc-155">The following is an example of the response.</span></span>

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

<span data-ttu-id="93fdc-156">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="93fdc-156">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,Peer-to-peer,Organized,Participated
```
