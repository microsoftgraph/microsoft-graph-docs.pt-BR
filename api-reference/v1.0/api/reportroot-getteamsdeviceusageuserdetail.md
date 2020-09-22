---
title: 'reportRoot: getTeamsDeviceUsageUserDetail'
description: Obtém detalhes sobre o uso de dispositivos do Microsoft Teams por usuário.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 0363eaff9c5d80faf7f0517b1105a321ae0efb65
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48069649"
---
# <a name="reportroot-getteamsdeviceusageuserdetail"></a><span data-ttu-id="aeac8-103">reportRoot: getTeamsDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="aeac8-103">reportRoot: getTeamsDeviceUsageUserDetail</span></span>

<span data-ttu-id="aeac8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aeac8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="aeac8-105">Obtém detalhes sobre o uso de dispositivos do Microsoft Teams por usuário.</span><span class="sxs-lookup"><span data-stu-id="aeac8-105">Get details about Microsoft Teams device usage by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="aeac8-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="aeac8-106">Permissions</span></span>

<span data-ttu-id="aeac8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aeac8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="aeac8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aeac8-109">Permission type</span></span>                        | <span data-ttu-id="aeac8-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="aeac8-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="aeac8-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aeac8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="aeac8-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="aeac8-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="aeac8-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aeac8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aeac8-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aeac8-114">Not supported.</span></span>                           |
| <span data-ttu-id="aeac8-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aeac8-115">Application</span></span>                            | <span data-ttu-id="aeac8-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="aeac8-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="aeac8-117">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="aeac8-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="aeac8-118">Para saber mais, confira a [Autorização para APIs lerem os relatórios de uso do Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="aeac8-118">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="aeac8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aeac8-119">HTTP request</span></span>

<!-- { "blockType": "samples" } -->

```http
GET /reports/getTeamsDeviceUsageUserDetail(period='{period_value}')
GET /reports/getTeamsDeviceUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="aeac8-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="aeac8-120">Function parameters</span></span>

<span data-ttu-id="aeac8-121">Na URL da solicitação, forneça um valor válido a um dos seguintes parâmetros.</span><span class="sxs-lookup"><span data-stu-id="aeac8-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="aeac8-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="aeac8-122">Parameter</span></span> | <span data-ttu-id="aeac8-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="aeac8-123">Type</span></span>   | <span data-ttu-id="aeac8-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="aeac8-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="aeac8-125">ponto</span><span class="sxs-lookup"><span data-stu-id="aeac8-125">period</span></span>    | <span data-ttu-id="aeac8-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aeac8-126">string</span></span> | <span data-ttu-id="aeac8-127">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="aeac8-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="aeac8-128">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="aeac8-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="aeac8-129">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="aeac8-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="aeac8-130">data</span><span class="sxs-lookup"><span data-stu-id="aeac8-130">date</span></span>      | <span data-ttu-id="aeac8-131">Data</span><span class="sxs-lookup"><span data-stu-id="aeac8-131">Date</span></span>   | <span data-ttu-id="aeac8-132">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="aeac8-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="aeac8-133">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="aeac8-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="aeac8-134">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="aeac8-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="aeac8-135">**Observação:** você precisa definir o período ou data na URL.</span><span class="sxs-lookup"><span data-stu-id="aeac8-135">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="aeac8-136">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aeac8-136">Request headers</span></span>

| <span data-ttu-id="aeac8-137">Nome</span><span class="sxs-lookup"><span data-stu-id="aeac8-137">Name</span></span>          | <span data-ttu-id="aeac8-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="aeac8-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="aeac8-139">Autorização</span><span class="sxs-lookup"><span data-stu-id="aeac8-139">Authorization</span></span> | <span data-ttu-id="aeac8-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aeac8-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="aeac8-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="aeac8-142">Response</span></span>

<span data-ttu-id="aeac8-143">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="aeac8-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="aeac8-144">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="aeac8-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="aeac8-145">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="aeac8-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="aeac8-146">O arquivo CSV possui os seguintes cabeçalhos para colunas:</span><span class="sxs-lookup"><span data-stu-id="aeac8-146">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="aeac8-147">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="aeac8-147">Report Refresh Date</span></span>
- <span data-ttu-id="aeac8-148">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="aeac8-148">User Principal Name</span></span>
- <span data-ttu-id="aeac8-149">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="aeac8-149">Last Activity Date</span></span>
- <span data-ttu-id="aeac8-150">Excluído</span><span class="sxs-lookup"><span data-stu-id="aeac8-150">Is Deleted</span></span>
- <span data-ttu-id="aeac8-151">Data de exclusão</span><span class="sxs-lookup"><span data-stu-id="aeac8-151">Deleted Date</span></span>
- <span data-ttu-id="aeac8-152">Usou Web</span><span class="sxs-lookup"><span data-stu-id="aeac8-152">Used Web</span></span>
- <span data-ttu-id="aeac8-153">Usou Windows Phone</span><span class="sxs-lookup"><span data-stu-id="aeac8-153">Used Windows Phone</span></span>
- <span data-ttu-id="aeac8-154">Usou iOS</span><span class="sxs-lookup"><span data-stu-id="aeac8-154">Used iOS</span></span>
- <span data-ttu-id="aeac8-155">Usou Mac</span><span class="sxs-lookup"><span data-stu-id="aeac8-155">Used Mac</span></span>
- <span data-ttu-id="aeac8-156">Usou telefone Android</span><span class="sxs-lookup"><span data-stu-id="aeac8-156">Used Android Phone</span></span>
- <span data-ttu-id="aeac8-157">Usou Windows</span><span class="sxs-lookup"><span data-stu-id="aeac8-157">Used Windows</span></span>
- <span data-ttu-id="aeac8-158">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="aeac8-158">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="aeac8-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aeac8-159">Example</span></span>

#### <a name="request"></a><span data-ttu-id="aeac8-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aeac8-160">Request</span></span>

<span data-ttu-id="aeac8-161">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="aeac8-161">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsdeviceusageuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getTeamsDeviceUsageUserDetail(period='D7')
```


#### <a name="response"></a><span data-ttu-id="aeac8-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="aeac8-162">Response</span></span>

<span data-ttu-id="aeac8-163">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="aeac8-163">The following is an example of the response.</span></span>

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

<span data-ttu-id="aeac8-164">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="aeac8-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Last Activity Date,Is Deleted,Deleted Date,Used Web,Used Windows Phone,Used iOS,Used Mac,Used Android Phone,Used Windows,Report Period
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

