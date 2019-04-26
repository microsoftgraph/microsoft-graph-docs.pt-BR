---
title: 'reportRoot: getEmailAppUsageAppsUserCounts'
description: Obtenha a contagem de usuários únicos por aplicativo de email.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: d962e06f08710b8ddaab0e8259a1f6739dd8c375
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33331812"
---
# <a name="reportroot-getemailappusageappsusercounts"></a><span data-ttu-id="c4f7d-103">reportRoot: getEmailAppUsageAppsUserCounts</span><span class="sxs-lookup"><span data-stu-id="c4f7d-103">reportRoot: getEmailAppUsageAppsUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4f7d-104">Obtenha a contagem de usuários únicos por aplicativo de email.</span><span class="sxs-lookup"><span data-stu-id="c4f7d-104">Get the count of unique users per email app.</span></span>

> <span data-ttu-id="c4f7d-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Uso de aplicativos de email](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span><span class="sxs-lookup"><span data-stu-id="c4f7d-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="c4f7d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c4f7d-106">Permissions</span></span>

<span data-ttu-id="c4f7d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4f7d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c4f7d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c4f7d-109">Permission type</span></span>                        | <span data-ttu-id="c4f7d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c4f7d-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="c4f7d-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c4f7d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c4f7d-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c4f7d-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="c4f7d-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c4f7d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4f7d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c4f7d-114">Not supported.</span></span>                           |
| <span data-ttu-id="c4f7d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c4f7d-115">Application</span></span>                            | <span data-ttu-id="c4f7d-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c4f7d-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="c4f7d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c4f7d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailAppUsageAppsUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="c4f7d-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="c4f7d-118">Function parameters</span></span>

<span data-ttu-id="c4f7d-119">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="c4f7d-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="c4f7d-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="c4f7d-120">Parameter</span></span> | <span data-ttu-id="c4f7d-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="c4f7d-121">Type</span></span>   | <span data-ttu-id="c4f7d-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c4f7d-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="c4f7d-123">ponto</span><span class="sxs-lookup"><span data-stu-id="c4f7d-123">period</span></span>    | <span data-ttu-id="c4f7d-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c4f7d-124">string</span></span> | <span data-ttu-id="c4f7d-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="c4f7d-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="c4f7d-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="c4f7d-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="c4f7d-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="c4f7d-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="c4f7d-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c4f7d-128">Required.</span></span> |

<span data-ttu-id="c4f7d-129">Este método dá suporte `$format` ao [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c4f7d-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="c4f7d-130">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="c4f7d-130">The default output type is text/csv.</span></span> <span data-ttu-id="c4f7d-131">No enTanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="c4f7d-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c4f7d-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c4f7d-132">Request headers</span></span>

| <span data-ttu-id="c4f7d-133">Nome</span><span class="sxs-lookup"><span data-stu-id="c4f7d-133">Name</span></span>          | <span data-ttu-id="c4f7d-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="c4f7d-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="c4f7d-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="c4f7d-135">Authorization</span></span> | <span data-ttu-id="c4f7d-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c4f7d-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="c4f7d-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4f7d-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="c4f7d-139">CSV</span><span class="sxs-lookup"><span data-stu-id="c4f7d-139">CSV</span></span>

<span data-ttu-id="c4f7d-140">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="c4f7d-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="c4f7d-141">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="c4f7d-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="c4f7d-142">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="c4f7d-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="c4f7d-143">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="c4f7d-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="c4f7d-144">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="c4f7d-144">Report Refresh Date</span></span>
- <span data-ttu-id="c4f7d-145">Mail para Mac</span><span class="sxs-lookup"><span data-stu-id="c4f7d-145">Mail For Mac</span></span>
- <span data-ttu-id="c4f7d-146">Outlook para Mac</span><span class="sxs-lookup"><span data-stu-id="c4f7d-146">Outlook For Mac</span></span>
- <span data-ttu-id="c4f7d-147">Outlook para Windows</span><span class="sxs-lookup"><span data-stu-id="c4f7d-147">Outlook For Windows</span></span>
- <span data-ttu-id="c4f7d-148">Outlook para Celular</span><span class="sxs-lookup"><span data-stu-id="c4f7d-148">Outlook For Mobile</span></span>
- <span data-ttu-id="c4f7d-149">Outro para Celular</span><span class="sxs-lookup"><span data-stu-id="c4f7d-149">Other For Mobile</span></span>
- <span data-ttu-id="c4f7d-150">Outlook para Web</span><span class="sxs-lookup"><span data-stu-id="c4f7d-150">Outlook For Web</span></span>
- <span data-ttu-id="c4f7d-151">Aplicativo POP3</span><span class="sxs-lookup"><span data-stu-id="c4f7d-151">POP3 App</span></span>
- <span data-ttu-id="c4f7d-152">Aplicativo IMAP4</span><span class="sxs-lookup"><span data-stu-id="c4f7d-152">IMAP4 App</span></span>
- <span data-ttu-id="c4f7d-153">Aplicativo SMTP</span><span class="sxs-lookup"><span data-stu-id="c4f7d-153">SMTP App</span></span>
- <span data-ttu-id="c4f7d-154">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="c4f7d-154">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="c4f7d-155">JSON</span><span class="sxs-lookup"><span data-stu-id="c4f7d-155">JSON</span></span>

<span data-ttu-id="c4f7d-156">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[emailAppUsageAppsUserCounts](../resources/emailappusageappsusercounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c4f7d-156">If successful, this method returns a `200 OK` response code and an **[emailAppUsageAppsUserCounts](../resources/emailappusageappsusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4f7d-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c4f7d-157">Example</span></span>

### <a name="csv"></a><span data-ttu-id="c4f7d-158">CSV</span><span class="sxs-lookup"><span data-stu-id="c4f7d-158">CSV</span></span>

<span data-ttu-id="c4f7d-159">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="c4f7d-159">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="c4f7d-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c4f7d-160">Request</span></span>

<span data-ttu-id="c4f7d-161">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c4f7d-161">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageappsusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageAppsUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="c4f7d-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4f7d-162">Response</span></span>

<span data-ttu-id="c4f7d-163">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c4f7d-163">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="c4f7d-164">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="c4f7d-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Mail For Mac,Outlook For Mac,Outlook For Windows,Outlook For Mobile,Other For Mobile,Outlook For Web,POP3 App,IMAP4 App,SMTP App,Report Period
```

### <a name="json"></a><span data-ttu-id="c4f7d-165">JSON</span><span class="sxs-lookup"><span data-stu-id="c4f7d-165">JSON</span></span>

<span data-ttu-id="c4f7d-166">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="c4f7d-166">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="c4f7d-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c4f7d-167">Request</span></span>

<span data-ttu-id="c4f7d-168">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c4f7d-168">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageappsusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageAppsUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="c4f7d-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4f7d-169">Response</span></span>

<span data-ttu-id="c4f7d-170">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c4f7d-170">The following is an example of the response.</span></span>

> <span data-ttu-id="c4f7d-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c4f7d-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailAppUsageAppsUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 345

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.emailAppUsageAppsUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "mailForMac": 4, 
      "outlookForMac": 105, 
      "outlookForWindows": 1589, 
      "outlookForMobile": 1116, 
      "otherForMobile": 485, 
      "outlookForWeb": 753, 
      "pop3App": 0, 
      "imap4App": 0, 
      "smtpApp": 0, 
      "reportPeriod": "7"
    }
  ]
}
```
