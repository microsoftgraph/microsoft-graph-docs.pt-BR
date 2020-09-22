---
title: 'reportRoot: getOneDriveUsageAccountCounts'
description: Obtenha a tendência no número de sites ativos do OneDrive for Business. Qualquer site em que usuários visualizaram, modificaram, carregaram, baixaram, compartilharam ou sincronizaram arquivos é considerado um site ativo.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 7f524fd58c10788308562c8deff136ef15484402
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48015649"
---
# <a name="reportroot-getonedriveusageaccountcounts"></a><span data-ttu-id="d7d81-104">reportRoot: getOneDriveUsageAccountCounts</span><span class="sxs-lookup"><span data-stu-id="d7d81-104">reportRoot: getOneDriveUsageAccountCounts</span></span>

<span data-ttu-id="d7d81-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d7d81-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d7d81-106">Obtenha a tendência no número de sites ativos do OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="d7d81-106">Get the trend in the number of active OneDrive for Business sites.</span></span> <span data-ttu-id="d7d81-107">Qualquer site em que usuários visualizaram, modificaram, carregaram, baixaram, compartilharam ou sincronizaram arquivos é considerado um site ativo.</span><span class="sxs-lookup"><span data-stu-id="d7d81-107">Any site on which users viewed, modified, uploaded, downloaded, shared, or synced files is considered an active site.</span></span>

> <span data-ttu-id="d7d81-108">**Observação:** Para obter detalhes sobre diferentes modos de exibição de relatórios e nomes, consulte [Microsoft 365 Reports-uso do onedrive for Business](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span><span class="sxs-lookup"><span data-stu-id="d7d81-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="d7d81-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="d7d81-109">Permissions</span></span>

<span data-ttu-id="d7d81-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7d81-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d7d81-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d7d81-112">Permission type</span></span>                        | <span data-ttu-id="d7d81-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d7d81-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="d7d81-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d7d81-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="d7d81-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d7d81-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="d7d81-116">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d7d81-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7d81-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d7d81-117">Not supported.</span></span>                           |
| <span data-ttu-id="d7d81-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d7d81-118">Application</span></span>                            | <span data-ttu-id="d7d81-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d7d81-119">Reports.Read.All</span></span>                         |

<span data-ttu-id="d7d81-120">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="d7d81-120">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="d7d81-121">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="d7d81-121">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="d7d81-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d7d81-122">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageAccountCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="d7d81-123">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="d7d81-123">Function parameters</span></span>

<span data-ttu-id="d7d81-124">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="d7d81-124">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="d7d81-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d7d81-125">Parameter</span></span> | <span data-ttu-id="d7d81-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="d7d81-126">Type</span></span>   | <span data-ttu-id="d7d81-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7d81-127">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="d7d81-128">ponto</span><span class="sxs-lookup"><span data-stu-id="d7d81-128">period</span></span>    | <span data-ttu-id="d7d81-129">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d7d81-129">string</span></span> | <span data-ttu-id="d7d81-130">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="d7d81-130">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="d7d81-131">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="d7d81-131">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="d7d81-132">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="d7d81-132">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="d7d81-133">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d7d81-133">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="d7d81-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d7d81-134">Request headers</span></span>

| <span data-ttu-id="d7d81-135">Nome</span><span class="sxs-lookup"><span data-stu-id="d7d81-135">Name</span></span>          | <span data-ttu-id="d7d81-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7d81-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="d7d81-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="d7d81-137">Authorization</span></span> | <span data-ttu-id="d7d81-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d7d81-p106">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="d7d81-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="d7d81-140">If-None-Match</span></span> | <span data-ttu-id="d7d81-141">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="d7d81-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="d7d81-142">Opcional.</span><span class="sxs-lookup"><span data-stu-id="d7d81-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="d7d81-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7d81-143">Response</span></span>

<span data-ttu-id="d7d81-144">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="d7d81-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="d7d81-145">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="d7d81-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="d7d81-146">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="d7d81-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="d7d81-147">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="d7d81-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="d7d81-148">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="d7d81-148">Report Refresh Date</span></span>
- <span data-ttu-id="d7d81-149">Tipo de site</span><span class="sxs-lookup"><span data-stu-id="d7d81-149">Site Type</span></span>
- <span data-ttu-id="d7d81-150">Total</span><span class="sxs-lookup"><span data-stu-id="d7d81-150">Total</span></span>
- <span data-ttu-id="d7d81-151">Ativo</span><span class="sxs-lookup"><span data-stu-id="d7d81-151">Active</span></span>
- <span data-ttu-id="d7d81-152">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="d7d81-152">Report Date</span></span>
- <span data-ttu-id="d7d81-153">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="d7d81-153">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="d7d81-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d7d81-154">Example</span></span>

#### <a name="request"></a><span data-ttu-id="d7d81-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d7d81-155">Request</span></span>

<span data-ttu-id="d7d81-156">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d7d81-156">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getonedriveusageaccountcounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getOneDriveUsageAccountCounts(period='D7')
```


#### <a name="response"></a><span data-ttu-id="d7d81-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7d81-157">Response</span></span>

<span data-ttu-id="d7d81-158">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d7d81-158">The following is an example of the response.</span></span>

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

<span data-ttu-id="d7d81-159">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="d7d81-159">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Total,Active,Report Date,Report Period
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

