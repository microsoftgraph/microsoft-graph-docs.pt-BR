---
title: 'reportRoot: getOneDriveUsageAccountCounts'
description: Obtenha a tendência no número de sites ativos do OneDrive for Business. Qualquer site em que usuários visualizaram, modificaram, carregaram, baixaram, compartilharam ou sincronizaram arquivos é considerado um site ativo.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 9f79cccf4a490345b322d6d7cba52e0f4ee11ef9
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49983472"
---
# <a name="reportroot-getonedriveusageaccountcounts"></a><span data-ttu-id="a1c02-104">reportRoot: getOneDriveUsageAccountCounts</span><span class="sxs-lookup"><span data-stu-id="a1c02-104">reportRoot: getOneDriveUsageAccountCounts</span></span>

<span data-ttu-id="a1c02-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a1c02-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a1c02-106">Obtenha a tendência no número de sites ativos do OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="a1c02-106">Get the trend in the number of active OneDrive for Business sites.</span></span> <span data-ttu-id="a1c02-107">Qualquer site em que usuários visualizaram, modificaram, carregaram, baixaram, compartilharam ou sincronizaram arquivos é considerado um site ativo.</span><span class="sxs-lookup"><span data-stu-id="a1c02-107">Any site on which users viewed, modified, uploaded, downloaded, shared, or synced files is considered an active site.</span></span>

> <span data-ttu-id="a1c02-108">**Observação:** Para obter detalhes sobre diferentes visualizações e nomes de relatórios, confira relatórios do [Microsoft 365 - uso do OneDrive for Business.](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680)</span><span class="sxs-lookup"><span data-stu-id="a1c02-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="a1c02-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="a1c02-109">Permissions</span></span>

<span data-ttu-id="a1c02-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1c02-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a1c02-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a1c02-112">Permission type</span></span>                        | <span data-ttu-id="a1c02-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a1c02-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="a1c02-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a1c02-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="a1c02-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a1c02-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="a1c02-116">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a1c02-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a1c02-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1c02-117">Not supported.</span></span>                           |
| <span data-ttu-id="a1c02-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a1c02-118">Application</span></span>                            | <span data-ttu-id="a1c02-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a1c02-119">Reports.Read.All</span></span>                         |

<span data-ttu-id="a1c02-120">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="a1c02-120">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="a1c02-121">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="a1c02-121">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="a1c02-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a1c02-122">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageAccountCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="a1c02-123">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="a1c02-123">Function parameters</span></span>

<span data-ttu-id="a1c02-124">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="a1c02-124">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="a1c02-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="a1c02-125">Parameter</span></span> | <span data-ttu-id="a1c02-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="a1c02-126">Type</span></span>   | <span data-ttu-id="a1c02-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1c02-127">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="a1c02-128">ponto</span><span class="sxs-lookup"><span data-stu-id="a1c02-128">period</span></span>    | <span data-ttu-id="a1c02-129">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a1c02-129">string</span></span> | <span data-ttu-id="a1c02-130">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="a1c02-130">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="a1c02-131">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="a1c02-131">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="a1c02-132">Eles seguem o formato D *n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="a1c02-132">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="a1c02-133">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a1c02-133">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="a1c02-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a1c02-134">Request headers</span></span>

| <span data-ttu-id="a1c02-135">Nome</span><span class="sxs-lookup"><span data-stu-id="a1c02-135">Name</span></span>          | <span data-ttu-id="a1c02-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1c02-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="a1c02-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="a1c02-137">Authorization</span></span> | <span data-ttu-id="a1c02-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a1c02-p106">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="a1c02-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="a1c02-140">If-None-Match</span></span> | <span data-ttu-id="a1c02-141">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="a1c02-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="a1c02-142">Opcional.</span><span class="sxs-lookup"><span data-stu-id="a1c02-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="a1c02-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1c02-143">Response</span></span>

<span data-ttu-id="a1c02-144">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="a1c02-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="a1c02-145">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="a1c02-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="a1c02-146">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="a1c02-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="a1c02-147">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="a1c02-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="a1c02-148">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="a1c02-148">Report Refresh Date</span></span>
- <span data-ttu-id="a1c02-149">Tipo de site</span><span class="sxs-lookup"><span data-stu-id="a1c02-149">Site Type</span></span>
- <span data-ttu-id="a1c02-150">Total</span><span class="sxs-lookup"><span data-stu-id="a1c02-150">Total</span></span>
- <span data-ttu-id="a1c02-151">Ativo</span><span class="sxs-lookup"><span data-stu-id="a1c02-151">Active</span></span>
- <span data-ttu-id="a1c02-152">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="a1c02-152">Report Date</span></span>
- <span data-ttu-id="a1c02-153">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="a1c02-153">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="a1c02-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a1c02-154">Example</span></span>

#### <a name="request"></a><span data-ttu-id="a1c02-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a1c02-155">Request</span></span>

<span data-ttu-id="a1c02-156">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a1c02-156">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getonedriveusageaccountcounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getOneDriveUsageAccountCounts(period='D7')
```


#### <a name="response"></a><span data-ttu-id="a1c02-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1c02-157">Response</span></span>

<span data-ttu-id="a1c02-158">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a1c02-158">The following is an example of the response.</span></span>

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

<span data-ttu-id="a1c02-159">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="a1c02-159">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

