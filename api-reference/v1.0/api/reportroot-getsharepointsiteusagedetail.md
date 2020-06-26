---
title: 'reportRoot: getSharePointSiteUsageDetail'
description: Obtenha dados sobre o uso do site do SharePoint.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 7e092fdb3de3a481c6857d706ffe274246f66b11
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897908"
---
# <a name="reportroot-getsharepointsiteusagedetail"></a><span data-ttu-id="28b59-103">reportRoot: getSharePointSiteUsageDetail</span><span class="sxs-lookup"><span data-stu-id="28b59-103">reportRoot: getSharePointSiteUsageDetail</span></span>

<span data-ttu-id="28b59-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28b59-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="28b59-105">Obtenha dados sobre o uso do site do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="28b59-105">Get details about SharePoint site usage.</span></span>

> <span data-ttu-id="28b59-106">**Observação:** Para obter detalhes sobre diferentes modos de exibição de relatórios e nomes, consulte [Microsoft 365 Reports-uso do site do SharePoint](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span><span class="sxs-lookup"><span data-stu-id="28b59-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="28b59-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="28b59-107">Permissions</span></span>

<span data-ttu-id="28b59-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="28b59-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="28b59-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28b59-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="28b59-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="28b59-110">Permission type</span></span>                        | <span data-ttu-id="28b59-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="28b59-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="28b59-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="28b59-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="28b59-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="28b59-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="28b59-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="28b59-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28b59-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="28b59-115">Not supported.</span></span>                           |
| <span data-ttu-id="28b59-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="28b59-116">Application</span></span>                            | <span data-ttu-id="28b59-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="28b59-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="28b59-118">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="28b59-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="28b59-119">Para obter mais detalhes, consulte [Authorization for APIs to read Microsoft 365 Usage Reports](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="28b59-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="28b59-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="28b59-120">HTTP request</span></span>


<!-- { "blockType": "samples" } --> 

```http
GET /reports/getSharePointSiteUsageDetail(period='{period_value}')
GET /reports/getSharePointSiteUsageDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="28b59-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="28b59-121">Function parameters</span></span>

<span data-ttu-id="28b59-122">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="28b59-122">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="28b59-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="28b59-123">Parameter</span></span> | <span data-ttu-id="28b59-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="28b59-124">Type</span></span>   | <span data-ttu-id="28b59-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="28b59-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="28b59-126">ponto</span><span class="sxs-lookup"><span data-stu-id="28b59-126">period</span></span>    | <span data-ttu-id="28b59-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="28b59-127">string</span></span> | <span data-ttu-id="28b59-128">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="28b59-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="28b59-129">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="28b59-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="28b59-130">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="28b59-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="28b59-131">data</span><span class="sxs-lookup"><span data-stu-id="28b59-131">date</span></span>      | <span data-ttu-id="28b59-132">Data</span><span class="sxs-lookup"><span data-stu-id="28b59-132">Date</span></span>   | <span data-ttu-id="28b59-133">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="28b59-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="28b59-134">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="28b59-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="28b59-135">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="28b59-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="28b59-136">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="28b59-136">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="28b59-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="28b59-137">Request headers</span></span>

| <span data-ttu-id="28b59-138">Nome</span><span class="sxs-lookup"><span data-stu-id="28b59-138">Name</span></span>          | <span data-ttu-id="28b59-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="28b59-139">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="28b59-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="28b59-140">Authorization</span></span> | <span data-ttu-id="28b59-141">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="28b59-141">Bearer {token}.</span></span> <span data-ttu-id="28b59-142">Required.</span><span class="sxs-lookup"><span data-stu-id="28b59-142">Required.</span></span>                |
| <span data-ttu-id="28b59-143">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="28b59-143">If-None-Match</span></span> | <span data-ttu-id="28b59-144">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="28b59-144">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="28b59-145">Opcional.</span><span class="sxs-lookup"><span data-stu-id="28b59-145">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="28b59-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="28b59-146">Response</span></span>

<span data-ttu-id="28b59-147">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="28b59-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="28b59-148">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="28b59-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="28b59-149">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="28b59-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="28b59-150">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="28b59-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="28b59-151">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="28b59-151">Report Refresh Date</span></span>
- <span data-ttu-id="28b59-152">ID de site</span><span class="sxs-lookup"><span data-stu-id="28b59-152">Site Id</span></span>
- <span data-ttu-id="28b59-153">URL do site</span><span class="sxs-lookup"><span data-stu-id="28b59-153">Site URL</span></span>
- <span data-ttu-id="28b59-154">Nome de exibição do proprietário</span><span class="sxs-lookup"><span data-stu-id="28b59-154">Owner Display Name</span></span>
- <span data-ttu-id="28b59-155">Excluído</span><span class="sxs-lookup"><span data-stu-id="28b59-155">Is Deleted</span></span>
- <span data-ttu-id="28b59-156">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="28b59-156">Last Activity Date</span></span>
- <span data-ttu-id="28b59-157">Contagem de arquivos</span><span class="sxs-lookup"><span data-stu-id="28b59-157">File Count</span></span>
- <span data-ttu-id="28b59-158">Contagem de arquivos ativos</span><span class="sxs-lookup"><span data-stu-id="28b59-158">Active File Count</span></span>
- <span data-ttu-id="28b59-159">Contagem de visualização de página</span><span class="sxs-lookup"><span data-stu-id="28b59-159">Page View Count</span></span>
- <span data-ttu-id="28b59-160">Contagem de páginas visitadas</span><span class="sxs-lookup"><span data-stu-id="28b59-160">Visited Page Count</span></span>
- <span data-ttu-id="28b59-161">Armazenamento utilizado (bytes)</span><span class="sxs-lookup"><span data-stu-id="28b59-161">Storage Used (Byte)</span></span>
- <span data-ttu-id="28b59-162">Armazenamento alocado (bytes)</span><span class="sxs-lookup"><span data-stu-id="28b59-162">Storage Allocated (Byte)</span></span>
- <span data-ttu-id="28b59-163">Modelo de Web raiz</span><span class="sxs-lookup"><span data-stu-id="28b59-163">Root Web Template</span></span>
- <span data-ttu-id="28b59-164">Nome principal do proprietário</span><span class="sxs-lookup"><span data-stu-id="28b59-164">Owner Principal Name</span></span>
- <span data-ttu-id="28b59-165">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="28b59-165">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="28b59-166">Exemplo</span><span class="sxs-lookup"><span data-stu-id="28b59-166">Example</span></span>

#### <a name="request"></a><span data-ttu-id="28b59-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="28b59-167">Request</span></span>

<span data-ttu-id="28b59-168">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="28b59-168">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getsharepointsiteusageuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getSharePointSiteUsageDetail(period='D7')
```


#### <a name="response"></a><span data-ttu-id="28b59-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="28b59-169">Response</span></span>

<span data-ttu-id="28b59-170">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="28b59-170">The following is an example of the response.</span></span>

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

<span data-ttu-id="28b59-171">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="28b59-171">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Id,Site URL,Owner Display Name,Is Deleted,Last Activity Date,File Count,Active File Count,Page View Count,Visited Page Count,Storage Used (Byte),Storage Allocated (Byte),Root Web Template,Owner Principal Name,Report Period
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
