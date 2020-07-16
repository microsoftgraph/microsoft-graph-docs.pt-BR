---
title: 'reportRoot: getEmailAppUsageAppsUserCounts'
description: Obtenha a contagem de usuários únicos por aplicativo de email.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: a7aeb6faa93d4d6ddc654a08daa7bf2095b35846
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44898223"
---
# <a name="reportroot-getemailappusageappsusercounts"></a><span data-ttu-id="e6556-103">reportRoot: getEmailAppUsageAppsUserCounts</span><span class="sxs-lookup"><span data-stu-id="e6556-103">reportRoot: getEmailAppUsageAppsUserCounts</span></span>

<span data-ttu-id="e6556-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6556-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e6556-105">Obtenha a contagem de usuários únicos por aplicativo de email.</span><span class="sxs-lookup"><span data-stu-id="e6556-105">Get the count of unique users per email app.</span></span>

> <span data-ttu-id="e6556-106">**Observação:** Para obter detalhes sobre diferentes modos de exibição e nomes de relatórios, consulte [Microsoft 365 Reports-uso de aplicativos de email](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span><span class="sxs-lookup"><span data-stu-id="e6556-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="e6556-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="e6556-107">Permissions</span></span>

<span data-ttu-id="e6556-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6556-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e6556-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e6556-110">Permission type</span></span>                        | <span data-ttu-id="e6556-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e6556-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="e6556-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e6556-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="e6556-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e6556-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="e6556-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e6556-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e6556-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e6556-115">Not supported.</span></span>                           |
| <span data-ttu-id="e6556-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e6556-116">Application</span></span>                            | <span data-ttu-id="e6556-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e6556-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="e6556-118">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="e6556-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="e6556-119">Para obter mais detalhes, consulte [Authorization for APIs to read Microsoft 365 Usage Reports](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="e6556-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="e6556-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e6556-120">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailAppUsageAppsUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="e6556-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="e6556-121">Function parameters</span></span>

<span data-ttu-id="e6556-122">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="e6556-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="e6556-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="e6556-123">Parameter</span></span> | <span data-ttu-id="e6556-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="e6556-124">Type</span></span>   | <span data-ttu-id="e6556-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6556-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="e6556-126">ponto</span><span class="sxs-lookup"><span data-stu-id="e6556-126">period</span></span>    | <span data-ttu-id="e6556-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6556-127">string</span></span> | <span data-ttu-id="e6556-128">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="e6556-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="e6556-129">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="e6556-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="e6556-130">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="e6556-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="e6556-131">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e6556-131">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="e6556-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e6556-132">Request headers</span></span>

| <span data-ttu-id="e6556-133">Nome</span><span class="sxs-lookup"><span data-stu-id="e6556-133">Name</span></span>          | <span data-ttu-id="e6556-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6556-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="e6556-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="e6556-135">Authorization</span></span> | <span data-ttu-id="e6556-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e6556-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="e6556-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="e6556-138">If-None-Match</span></span> | <span data-ttu-id="e6556-139">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="e6556-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="e6556-140">Opcional.</span><span class="sxs-lookup"><span data-stu-id="e6556-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="e6556-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6556-141">Response</span></span>

<span data-ttu-id="e6556-142">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="e6556-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="e6556-143">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="e6556-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="e6556-144">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="e6556-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="e6556-145">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="e6556-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="e6556-146">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="e6556-146">Report Refresh Date</span></span>
- <span data-ttu-id="e6556-147">Mail para Mac</span><span class="sxs-lookup"><span data-stu-id="e6556-147">Mail For Mac</span></span>
- <span data-ttu-id="e6556-148">Outlook para Mac</span><span class="sxs-lookup"><span data-stu-id="e6556-148">Outlook For Mac</span></span>
- <span data-ttu-id="e6556-149">Outlook para Windows</span><span class="sxs-lookup"><span data-stu-id="e6556-149">Outlook For Windows</span></span>
- <span data-ttu-id="e6556-150">Outlook para Celular</span><span class="sxs-lookup"><span data-stu-id="e6556-150">Outlook For Mobile</span></span>
- <span data-ttu-id="e6556-151">Outro para Celular</span><span class="sxs-lookup"><span data-stu-id="e6556-151">Other For Mobile</span></span>
- <span data-ttu-id="e6556-152">Outlook para Web</span><span class="sxs-lookup"><span data-stu-id="e6556-152">Outlook For Web</span></span>
- <span data-ttu-id="e6556-153">Aplicativo POP3</span><span class="sxs-lookup"><span data-stu-id="e6556-153">POP3 App</span></span>
- <span data-ttu-id="e6556-154">Aplicativo IMAP4</span><span class="sxs-lookup"><span data-stu-id="e6556-154">IMAP4 App</span></span>
- <span data-ttu-id="e6556-155">Aplicativo SMTP</span><span class="sxs-lookup"><span data-stu-id="e6556-155">SMTP App</span></span>
- <span data-ttu-id="e6556-156">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="e6556-156">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="e6556-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e6556-157">Example</span></span>

#### <a name="request"></a><span data-ttu-id="e6556-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e6556-158">Request</span></span>

<span data-ttu-id="e6556-159">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e6556-159">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getemailappusageappsusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getEmailAppUsageAppsUserCounts(period='D7')
```


#### <a name="response"></a><span data-ttu-id="e6556-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6556-160">Response</span></span>

<span data-ttu-id="e6556-161">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e6556-161">The following is an example of the response.</span></span>

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

<span data-ttu-id="e6556-162">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="e6556-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Mail For Mac,Outlook For Mac,Outlook For Windows,Outlook For Mobile,Other For Mobile,Outlook For Web,POP3 App,IMAP4 App,SMTP App,Report Period
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
