---
title: 'reportRoot: getEmailAppUsageAppsUserCounts'
description: Obtenha a contagem de usuários únicos por aplicativo de email.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: a4a53b7f0acd79594f4e567efe60fa2eefd775d3
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896396"
---
# <a name="reportroot-getemailappusageappsusercounts"></a><span data-ttu-id="a8bb8-103">reportRoot: getEmailAppUsageAppsUserCounts</span><span class="sxs-lookup"><span data-stu-id="a8bb8-103">reportRoot: getEmailAppUsageAppsUserCounts</span></span>

<span data-ttu-id="a8bb8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a8bb8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a8bb8-105">Obtenha a contagem de usuários únicos por aplicativo de email.</span><span class="sxs-lookup"><span data-stu-id="a8bb8-105">Get the count of unique users per email app.</span></span>

> <span data-ttu-id="a8bb8-106">**Observação:** Para obter detalhes sobre diferentes modos de exibição e nomes de relatórios, consulte [Microsoft 365 Reports-uso de aplicativos de email](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span><span class="sxs-lookup"><span data-stu-id="a8bb8-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="a8bb8-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="a8bb8-107">Permissions</span></span>

<span data-ttu-id="a8bb8-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="a8bb8-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="a8bb8-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8bb8-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a8bb8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a8bb8-110">Permission type</span></span>                        | <span data-ttu-id="a8bb8-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a8bb8-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="a8bb8-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a8bb8-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="a8bb8-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a8bb8-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="a8bb8-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a8bb8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a8bb8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a8bb8-115">Not supported.</span></span>                           |
| <span data-ttu-id="a8bb8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a8bb8-116">Application</span></span>                            | <span data-ttu-id="a8bb8-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a8bb8-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="a8bb8-118">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="a8bb8-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="a8bb8-119">Para obter mais detalhes, consulte [Authorization for APIs to read Microsoft 365 Usage Reports](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="a8bb8-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="a8bb8-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a8bb8-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailAppUsageAppsUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="a8bb8-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="a8bb8-121">Function parameters</span></span>

<span data-ttu-id="a8bb8-122">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="a8bb8-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="a8bb8-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="a8bb8-123">Parameter</span></span> | <span data-ttu-id="a8bb8-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="a8bb8-124">Type</span></span>   | <span data-ttu-id="a8bb8-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8bb8-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="a8bb8-126">ponto</span><span class="sxs-lookup"><span data-stu-id="a8bb8-126">period</span></span>    | <span data-ttu-id="a8bb8-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a8bb8-127">string</span></span> | <span data-ttu-id="a8bb8-128">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="a8bb8-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="a8bb8-129">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="a8bb8-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="a8bb8-130">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="a8bb8-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="a8bb8-131">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a8bb8-131">Required.</span></span> |

<span data-ttu-id="a8bb8-132">Esse método dá suporte ao`$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a8bb8-132">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="a8bb8-133">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="a8bb8-133">The default output type is text/csv.</span></span> <span data-ttu-id="a8bb8-134">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="a8bb8-134">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a8bb8-135">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a8bb8-135">Request headers</span></span>

| <span data-ttu-id="a8bb8-136">Nome</span><span class="sxs-lookup"><span data-stu-id="a8bb8-136">Name</span></span>          | <span data-ttu-id="a8bb8-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8bb8-137">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="a8bb8-138">Autorização</span><span class="sxs-lookup"><span data-stu-id="a8bb8-138">Authorization</span></span> | <span data-ttu-id="a8bb8-139">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="a8bb8-139">Bearer {token}.</span></span> <span data-ttu-id="a8bb8-140">Required.</span><span class="sxs-lookup"><span data-stu-id="a8bb8-140">Required.</span></span> |

## <a name="response"></a><span data-ttu-id="a8bb8-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8bb8-141">Response</span></span>

### <a name="csv"></a><span data-ttu-id="a8bb8-142">CSV</span><span class="sxs-lookup"><span data-stu-id="a8bb8-142">CSV</span></span>

<span data-ttu-id="a8bb8-143">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="a8bb8-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="a8bb8-144">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="a8bb8-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="a8bb8-145">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="a8bb8-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="a8bb8-146">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="a8bb8-146">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="a8bb8-147">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="a8bb8-147">Report Refresh Date</span></span>
- <span data-ttu-id="a8bb8-148">Mail para Mac</span><span class="sxs-lookup"><span data-stu-id="a8bb8-148">Mail For Mac</span></span>
- <span data-ttu-id="a8bb8-149">Outlook para Mac</span><span class="sxs-lookup"><span data-stu-id="a8bb8-149">Outlook For Mac</span></span>
- <span data-ttu-id="a8bb8-150">Outlook para Windows</span><span class="sxs-lookup"><span data-stu-id="a8bb8-150">Outlook For Windows</span></span>
- <span data-ttu-id="a8bb8-151">Outlook para Celular</span><span class="sxs-lookup"><span data-stu-id="a8bb8-151">Outlook For Mobile</span></span>
- <span data-ttu-id="a8bb8-152">Outro para Celular</span><span class="sxs-lookup"><span data-stu-id="a8bb8-152">Other For Mobile</span></span>
- <span data-ttu-id="a8bb8-153">Outlook para Web</span><span class="sxs-lookup"><span data-stu-id="a8bb8-153">Outlook For Web</span></span>
- <span data-ttu-id="a8bb8-154">Aplicativo POP3</span><span class="sxs-lookup"><span data-stu-id="a8bb8-154">POP3 App</span></span>
- <span data-ttu-id="a8bb8-155">Aplicativo IMAP4</span><span class="sxs-lookup"><span data-stu-id="a8bb8-155">IMAP4 App</span></span>
- <span data-ttu-id="a8bb8-156">Aplicativo SMTP</span><span class="sxs-lookup"><span data-stu-id="a8bb8-156">SMTP App</span></span>
- <span data-ttu-id="a8bb8-157">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="a8bb8-157">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="a8bb8-158">JSON</span><span class="sxs-lookup"><span data-stu-id="a8bb8-158">JSON</span></span>

<span data-ttu-id="a8bb8-159">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **[emailAppUsageAppsUserCounts](../resources/emailappusageappsusercounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a8bb8-159">If successful, this method returns a `200 OK` response code and an **[emailAppUsageAppsUserCounts](../resources/emailappusageappsusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8bb8-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a8bb8-160">Example</span></span>

### <a name="csv"></a><span data-ttu-id="a8bb8-161">CSV</span><span class="sxs-lookup"><span data-stu-id="a8bb8-161">CSV</span></span>

<span data-ttu-id="a8bb8-162">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="a8bb8-162">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="a8bb8-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a8bb8-163">Request</span></span>

<span data-ttu-id="a8bb8-164">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a8bb8-164">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getemailappusageappsusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageAppsUserCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="a8bb8-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8bb8-165">Response</span></span>

<span data-ttu-id="a8bb8-166">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a8bb8-166">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="a8bb8-167">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="a8bb8-167">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="a8bb8-168">JSON</span><span class="sxs-lookup"><span data-stu-id="a8bb8-168">JSON</span></span>

<span data-ttu-id="a8bb8-169">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="a8bb8-169">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="a8bb8-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a8bb8-170">Request</span></span>

<span data-ttu-id="a8bb8-171">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a8bb8-171">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getemailappusageappsusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageAppsUserCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="a8bb8-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8bb8-172">Response</span></span>

<span data-ttu-id="a8bb8-173">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a8bb8-173">The following is an example of the response.</span></span>

> <span data-ttu-id="a8bb8-174">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="a8bb8-174">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a8bb8-175">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="a8bb8-175">All the properties will be returned from an actual call.</span></span>

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
