---
title: 'reportRoot: getOffice365ActiveUserCounts'
description: Obtenha a contagem de usuários ativos diários no período de relatório por produto.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 3469cbcf2dee789ca848f88d43d8eb3ff640f9c7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980031"
---
# <a name="reportroot-getoffice365activeusercounts"></a><span data-ttu-id="b6de5-103">reportRoot: getOffice365ActiveUserCounts</span><span class="sxs-lookup"><span data-stu-id="b6de5-103">reportRoot: getOffice365ActiveUserCounts</span></span>

<span data-ttu-id="b6de5-104">Obtenha a contagem de usuários ativos diários no período de relatório por produto.</span><span class="sxs-lookup"><span data-stu-id="b6de5-104">Get the count of daily active users in the reporting period by product.</span></span>

> <span data-ttu-id="b6de5-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Usuários ativos](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="b6de5-105">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="b6de5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b6de5-106">Permissions</span></span>

<span data-ttu-id="b6de5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6de5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b6de5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b6de5-109">Permission type</span></span>                        | <span data-ttu-id="b6de5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b6de5-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="b6de5-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b6de5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b6de5-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b6de5-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="b6de5-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b6de5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b6de5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6de5-114">Not supported.</span></span>                           |
| <span data-ttu-id="b6de5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b6de5-115">Application</span></span>                            | <span data-ttu-id="b6de5-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b6de5-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="b6de5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b6de5-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActiveUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="b6de5-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="b6de5-118">Function parameters</span></span>

<span data-ttu-id="b6de5-119">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="b6de5-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="b6de5-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b6de5-120">Parameter</span></span> | <span data-ttu-id="b6de5-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="b6de5-121">Type</span></span>   | <span data-ttu-id="b6de5-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6de5-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="b6de5-123">ponto</span><span class="sxs-lookup"><span data-stu-id="b6de5-123">period</span></span>    | <span data-ttu-id="b6de5-124">string</span><span class="sxs-lookup"><span data-stu-id="b6de5-124">string</span></span> | <span data-ttu-id="b6de5-125">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="b6de5-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="b6de5-126">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="b6de5-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="b6de5-127">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="b6de5-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="b6de5-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b6de5-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="b6de5-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b6de5-129">Request headers</span></span>

| <span data-ttu-id="b6de5-130">Nome</span><span class="sxs-lookup"><span data-stu-id="b6de5-130">Name</span></span>          | <span data-ttu-id="b6de5-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6de5-131">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="b6de5-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="b6de5-132">Authorization</span></span> | <span data-ttu-id="b6de5-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b6de5-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="b6de5-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6de5-135">Response</span></span>

<span data-ttu-id="b6de5-136">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="b6de5-136">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="b6de5-137">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="b6de5-137">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="b6de5-138">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="b6de5-138">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="b6de5-139">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="b6de5-139">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="b6de5-140">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="b6de5-140">Report Refresh Date</span></span>
- <span data-ttu-id="b6de5-141">Office 365</span><span class="sxs-lookup"><span data-stu-id="b6de5-141">Office 365</span></span>
- <span data-ttu-id="b6de5-142">Exchange</span><span class="sxs-lookup"><span data-stu-id="b6de5-142">Exchange</span></span>
- <span data-ttu-id="b6de5-143">OneDrive</span><span class="sxs-lookup"><span data-stu-id="b6de5-143">OneDrive</span></span>
- <span data-ttu-id="b6de5-144">SharePoint</span><span class="sxs-lookup"><span data-stu-id="b6de5-144">SharePoint</span></span>
- <span data-ttu-id="b6de5-145">Skype for Business</span><span class="sxs-lookup"><span data-stu-id="b6de5-145">Skype For Business</span></span> 
- <span data-ttu-id="b6de5-146">Yammer</span><span class="sxs-lookup"><span data-stu-id="b6de5-146">Yammer</span></span>
- <span data-ttu-id="b6de5-147">Teams</span><span class="sxs-lookup"><span data-stu-id="b6de5-147">Teams</span></span>
- <span data-ttu-id="b6de5-148">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="b6de5-148">Report Date</span></span>
- <span data-ttu-id="b6de5-149">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="b6de5-149">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="b6de5-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b6de5-150">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b6de5-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b6de5-151">Request</span></span>

<span data-ttu-id="b6de5-152">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b6de5-152">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activeusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActiveUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="b6de5-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6de5-153">Response</span></span>

<span data-ttu-id="b6de5-154">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b6de5-154">The following is an example of the response.</span></span>

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

<span data-ttu-id="b6de5-155">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="b6de5-155">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Office 365,Exchange,OneDrive,SharePoint,Skype For Business,Yammer,Teams,Report Date,Report Period
```
