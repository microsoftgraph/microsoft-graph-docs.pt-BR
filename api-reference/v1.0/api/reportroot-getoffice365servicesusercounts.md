---
title: 'reportRoot: getOffice365ServicesUserCounts'
description: Obtenha a contagem de usuários por tipo de atividade e serviço.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 0b505ed58691cd965cb055818a1cb233b212252d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949056"
---
# <a name="reportroot-getoffice365servicesusercounts"></a><span data-ttu-id="66381-103">reportRoot: getOffice365ServicesUserCounts</span><span class="sxs-lookup"><span data-stu-id="66381-103">reportRoot: getOffice365ServicesUserCounts</span></span>

<span data-ttu-id="66381-104">Obtenha a contagem de usuários por tipo de atividade e serviço.</span><span class="sxs-lookup"><span data-stu-id="66381-104">Get the count of users by activity type and service.</span></span>

> <span data-ttu-id="66381-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Usuários ativos](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="66381-105">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="66381-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="66381-106">Permissions</span></span>

<span data-ttu-id="66381-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66381-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="66381-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="66381-109">Permission type</span></span>                        | <span data-ttu-id="66381-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="66381-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="66381-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="66381-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="66381-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="66381-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="66381-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="66381-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66381-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="66381-114">Not supported.</span></span>                           |
| <span data-ttu-id="66381-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="66381-115">Application</span></span>                            | <span data-ttu-id="66381-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="66381-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="66381-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="66381-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ServicesUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="66381-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="66381-118">Function parameters</span></span>

<span data-ttu-id="66381-119">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="66381-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="66381-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="66381-120">Parameter</span></span> | <span data-ttu-id="66381-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="66381-121">Type</span></span>   | <span data-ttu-id="66381-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="66381-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="66381-123">ponto</span><span class="sxs-lookup"><span data-stu-id="66381-123">period</span></span>    | <span data-ttu-id="66381-124">string</span><span class="sxs-lookup"><span data-stu-id="66381-124">string</span></span> | <span data-ttu-id="66381-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="66381-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="66381-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="66381-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="66381-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="66381-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="66381-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="66381-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="66381-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="66381-129">Request headers</span></span>

| <span data-ttu-id="66381-130">Nome</span><span class="sxs-lookup"><span data-stu-id="66381-130">Name</span></span>          | <span data-ttu-id="66381-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="66381-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="66381-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="66381-132">Authorization</span></span> | <span data-ttu-id="66381-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="66381-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="66381-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="66381-135">If-None-Match</span></span> | <span data-ttu-id="66381-136">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="66381-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="66381-137">Opcional.</span><span class="sxs-lookup"><span data-stu-id="66381-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="66381-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="66381-138">Response</span></span>

<span data-ttu-id="66381-139">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="66381-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="66381-140">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="66381-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="66381-141">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="66381-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="66381-142">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="66381-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="66381-143">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="66381-143">Report Refresh Date</span></span>
- <span data-ttu-id="66381-144">Exchange ativo</span><span class="sxs-lookup"><span data-stu-id="66381-144">Exchange Active</span></span>
- <span data-ttu-id="66381-145">Exchange inativo</span><span class="sxs-lookup"><span data-stu-id="66381-145">Exchange Inactive</span></span>
- <span data-ttu-id="66381-146">OneDrive ativo</span><span class="sxs-lookup"><span data-stu-id="66381-146">OneDrive Active</span></span>
- <span data-ttu-id="66381-147">OneDrive inativo</span><span class="sxs-lookup"><span data-stu-id="66381-147">OneDrive Inactive</span></span>
- <span data-ttu-id="66381-148">SharePoint ativo</span><span class="sxs-lookup"><span data-stu-id="66381-148">SharePoint Active</span></span>
- <span data-ttu-id="66381-149">SharePoint inativo</span><span class="sxs-lookup"><span data-stu-id="66381-149">SharePoint Inactive</span></span>
- <span data-ttu-id="66381-150">Skype for Business ativo</span><span class="sxs-lookup"><span data-stu-id="66381-150">Skype For Business Active</span></span>
- <span data-ttu-id="66381-151">Skype for Business inativo</span><span class="sxs-lookup"><span data-stu-id="66381-151">Skype For Business Inactive</span></span>
- <span data-ttu-id="66381-152">Yammer ativa</span><span class="sxs-lookup"><span data-stu-id="66381-152">Yammer Active</span></span>
- <span data-ttu-id="66381-153">Yammer inativa</span><span class="sxs-lookup"><span data-stu-id="66381-153">Yammer Inactive</span></span>
- <span data-ttu-id="66381-154">Teams ativo</span><span class="sxs-lookup"><span data-stu-id="66381-154">Teams Active</span></span>
- <span data-ttu-id="66381-155">Teams inativo</span><span class="sxs-lookup"><span data-stu-id="66381-155">Teams Inactive</span></span>
- <span data-ttu-id="66381-156">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="66381-156">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="66381-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="66381-157">Example</span></span>

#### <a name="request"></a><span data-ttu-id="66381-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="66381-158">Request</span></span>

<span data-ttu-id="66381-159">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="66381-159">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365servicesusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ServicesUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="66381-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="66381-160">Response</span></span>

<span data-ttu-id="66381-161">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="66381-161">The following is an example of the response.</span></span>

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

<span data-ttu-id="66381-162">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="66381-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Exchange Active,Exchange Inactive,OneDrive Active,OneDrive Inactive,SharePoint Active,SharePoint Inactive,Skype For Business Active,Skype For Business Inactive,Yammer Active,Yammer Inactive,Teams Active,Teams Inactive,Report Period
```
