---
title: 'reportRoot: getOneDriveUsageAccountDetail'
description: Obtenha dados sobre o uso do OneDrive por conta.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 79aec888e18207ba6b9e83a4dd8ab65a4cb3248b
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897670"
---
# <a name="reportroot-getonedriveusageaccountdetail"></a><span data-ttu-id="d3fff-103">reportRoot: getOneDriveUsageAccountDetail</span><span class="sxs-lookup"><span data-stu-id="d3fff-103">reportRoot: getOneDriveUsageAccountDetail</span></span>

<span data-ttu-id="d3fff-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3fff-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d3fff-105">Obtenha dados sobre o uso do OneDrive por conta.</span><span class="sxs-lookup"><span data-stu-id="d3fff-105">Get details about OneDrive usage by account.</span></span>

> <span data-ttu-id="d3fff-106">**Observação:** Para obter detalhes sobre diferentes modos de exibição de relatórios e nomes, consulte [Microsoft 365 Reports-uso do onedrive for Business](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span><span class="sxs-lookup"><span data-stu-id="d3fff-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="d3fff-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="d3fff-107">Permissions</span></span>

<span data-ttu-id="d3fff-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="d3fff-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="d3fff-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3fff-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d3fff-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d3fff-110">Permission type</span></span>                        | <span data-ttu-id="d3fff-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d3fff-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="d3fff-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d3fff-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="d3fff-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d3fff-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="d3fff-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d3fff-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d3fff-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d3fff-115">Not supported.</span></span>                           |
| <span data-ttu-id="d3fff-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d3fff-116">Application</span></span>                            | <span data-ttu-id="d3fff-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d3fff-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="d3fff-118">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="d3fff-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="d3fff-119">Para obter mais detalhes, consulte [Authorization for APIs to read Microsoft 365 Usage Reports](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="d3fff-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="d3fff-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d3fff-120">HTTP request</span></span>


<!-- { "blockType": "samples" } --> 

```http
GET /reports/getOneDriveUsageAccountDetail(period='{period_value}')
GET /reports/getOneDriveUsageAccountDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="d3fff-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="d3fff-121">Function parameters</span></span>

<span data-ttu-id="d3fff-122">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="d3fff-122">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="d3fff-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d3fff-123">Parameter</span></span> | <span data-ttu-id="d3fff-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="d3fff-124">Type</span></span>   | <span data-ttu-id="d3fff-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3fff-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="d3fff-126">ponto</span><span class="sxs-lookup"><span data-stu-id="d3fff-126">period</span></span>    | <span data-ttu-id="d3fff-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d3fff-127">string</span></span> | <span data-ttu-id="d3fff-128">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="d3fff-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="d3fff-129">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="d3fff-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="d3fff-130">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="d3fff-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="d3fff-131">data</span><span class="sxs-lookup"><span data-stu-id="d3fff-131">date</span></span>      | <span data-ttu-id="d3fff-132">Data</span><span class="sxs-lookup"><span data-stu-id="d3fff-132">Date</span></span>   | <span data-ttu-id="d3fff-133">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="d3fff-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="d3fff-134">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="d3fff-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="d3fff-135">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="d3fff-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="d3fff-136">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="d3fff-136">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d3fff-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d3fff-137">Request headers</span></span>

| <span data-ttu-id="d3fff-138">Nome</span><span class="sxs-lookup"><span data-stu-id="d3fff-138">Name</span></span>          | <span data-ttu-id="d3fff-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3fff-139">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="d3fff-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="d3fff-140">Authorization</span></span> | <span data-ttu-id="d3fff-141">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="d3fff-141">Bearer {token}.</span></span> <span data-ttu-id="d3fff-142">Required.</span><span class="sxs-lookup"><span data-stu-id="d3fff-142">Required.</span></span>                |
| <span data-ttu-id="d3fff-143">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="d3fff-143">If-None-Match</span></span> | <span data-ttu-id="d3fff-144">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="d3fff-144">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="d3fff-145">Opcional.</span><span class="sxs-lookup"><span data-stu-id="d3fff-145">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="d3fff-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3fff-146">Response</span></span>

<span data-ttu-id="d3fff-147">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="d3fff-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="d3fff-148">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="d3fff-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="d3fff-149">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="d3fff-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="d3fff-150">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="d3fff-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="d3fff-151">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="d3fff-151">Report Refresh Date</span></span>
- <span data-ttu-id="d3fff-152">URL do site</span><span class="sxs-lookup"><span data-stu-id="d3fff-152">Site URL</span></span>
- <span data-ttu-id="d3fff-153">Nome de exibição do proprietário</span><span class="sxs-lookup"><span data-stu-id="d3fff-153">Owner Display Name</span></span>
- <span data-ttu-id="d3fff-154">Excluído</span><span class="sxs-lookup"><span data-stu-id="d3fff-154">Is Deleted</span></span>
- <span data-ttu-id="d3fff-155">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="d3fff-155">Last Activity Date</span></span>
- <span data-ttu-id="d3fff-156">Contagem de arquivos</span><span class="sxs-lookup"><span data-stu-id="d3fff-156">File Count</span></span>
- <span data-ttu-id="d3fff-157">Contagem de arquivos ativos</span><span class="sxs-lookup"><span data-stu-id="d3fff-157">Active File Count</span></span>
- <span data-ttu-id="d3fff-158">Armazenamento utilizado (bytes)</span><span class="sxs-lookup"><span data-stu-id="d3fff-158">Storage Used (Byte)</span></span>
- <span data-ttu-id="d3fff-159">Armazenamento alocado (bytes)</span><span class="sxs-lookup"><span data-stu-id="d3fff-159">Storage Allocated (Byte)</span></span>
- <span data-ttu-id="d3fff-160">Nome principal do proprietário</span><span class="sxs-lookup"><span data-stu-id="d3fff-160">Owner Principal Name</span></span>
- <span data-ttu-id="d3fff-161">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="d3fff-161">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="d3fff-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d3fff-162">Example</span></span>

#### <a name="request"></a><span data-ttu-id="d3fff-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d3fff-163">Request</span></span>

<span data-ttu-id="d3fff-164">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d3fff-164">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getonedriveusageuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getOneDriveUsageAccountDetail(period='D7')
```


#### <a name="response"></a><span data-ttu-id="d3fff-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3fff-165">Response</span></span>

<span data-ttu-id="d3fff-166">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d3fff-166">The following is an example of the response.</span></span>

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

<span data-ttu-id="d3fff-167">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="d3fff-167">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site URL,Owner Display Name,Is Deleted,Last Activity Date,File Count,Active File Count,Storage Used (Byte),Storage Allocated (Byte),Owner Principal Name,Report Period
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
