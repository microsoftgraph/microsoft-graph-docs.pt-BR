---
title: 'reportRoot: getMailboxUsageStorage'
description: Obtenha a quantidade de armazenamento usada em sua organização.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: f2423c13102bd3fdf648765fe59df99aca61cf64
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981638"
---
# <a name="reportroot-getmailboxusagestorage"></a><span data-ttu-id="38439-103">reportRoot: getMailboxUsageStorage</span><span class="sxs-lookup"><span data-stu-id="38439-103">reportRoot: getMailboxUsageStorage</span></span>

<span data-ttu-id="38439-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38439-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38439-105">Obtenha a quantidade de armazenamento usada em sua organização.</span><span class="sxs-lookup"><span data-stu-id="38439-105">Get the amount of storage used in your organization.</span></span>

> <span data-ttu-id="38439-106">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Microsoft 365 - Uso da caixa de correio](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span><span class="sxs-lookup"><span data-stu-id="38439-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="38439-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="38439-107">Permissions</span></span>

<span data-ttu-id="38439-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38439-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="38439-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="38439-110">Permission type</span></span>                        | <span data-ttu-id="38439-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="38439-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="38439-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="38439-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="38439-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="38439-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="38439-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="38439-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="38439-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="38439-115">Not supported.</span></span>                           |
| <span data-ttu-id="38439-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="38439-116">Application</span></span>                            | <span data-ttu-id="38439-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="38439-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="38439-118">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="38439-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="38439-119">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="38439-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="38439-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="38439-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageStorage(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="38439-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="38439-121">Function parameters</span></span>

<span data-ttu-id="38439-122">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="38439-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="38439-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="38439-123">Parameter</span></span> | <span data-ttu-id="38439-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="38439-124">Type</span></span>   | <span data-ttu-id="38439-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="38439-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="38439-126">ponto</span><span class="sxs-lookup"><span data-stu-id="38439-126">period</span></span>    | <span data-ttu-id="38439-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="38439-127">string</span></span> | <span data-ttu-id="38439-128">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="38439-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="38439-129">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="38439-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="38439-130">Eles seguem o formato D *n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="38439-130">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="38439-131">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="38439-131">Required.</span></span> |

<span data-ttu-id="38439-132">Esse método dá suporte ao`$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="38439-132">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="38439-133">O tipo de saída padrão é texto/csv.</span><span class="sxs-lookup"><span data-stu-id="38439-133">The default output type is text/csv.</span></span> <span data-ttu-id="38439-134">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta $format OData definido como text/csv ou application/json.</span><span class="sxs-lookup"><span data-stu-id="38439-134">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="38439-135">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="38439-135">Request headers</span></span>

| <span data-ttu-id="38439-136">Nome</span><span class="sxs-lookup"><span data-stu-id="38439-136">Name</span></span>          | <span data-ttu-id="38439-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="38439-137">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="38439-138">Autorização</span><span class="sxs-lookup"><span data-stu-id="38439-138">Authorization</span></span> | <span data-ttu-id="38439-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="38439-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="38439-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="38439-141">Response</span></span>

### <a name="csv"></a><span data-ttu-id="38439-142">CSV</span><span class="sxs-lookup"><span data-stu-id="38439-142">CSV</span></span>

<span data-ttu-id="38439-143">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="38439-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="38439-144">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="38439-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="38439-145">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="38439-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="38439-146">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="38439-146">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="38439-147">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="38439-147">Report Refresh Date</span></span>
- <span data-ttu-id="38439-148">Armazenamento utilizado (bytes)</span><span class="sxs-lookup"><span data-stu-id="38439-148">Storage Used (Byte)</span></span>
- <span data-ttu-id="38439-149">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="38439-149">Report Date</span></span>
- <span data-ttu-id="38439-150">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="38439-150">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="38439-151">JSON</span><span class="sxs-lookup"><span data-stu-id="38439-151">JSON</span></span>

<span data-ttu-id="38439-152">Se bem-sucedido, este método retorna um código de resposta e um objeto `200 OK` **[mailboxUsageStorage](../resources/mailboxusagestorage.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="38439-152">If successful, this method returns a `200 OK` response code and a **[mailboxUsageStorage](../resources/mailboxusagestorage.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38439-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="38439-153">Example</span></span>

### <a name="csv"></a><span data-ttu-id="38439-154">CSV</span><span class="sxs-lookup"><span data-stu-id="38439-154">CSV</span></span>

<span data-ttu-id="38439-155">A seguir está um exemplo que saída CSV.</span><span class="sxs-lookup"><span data-stu-id="38439-155">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="38439-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="38439-156">Request</span></span>

<span data-ttu-id="38439-157">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="38439-157">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getmailboxusagestorage_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getMailboxUsageStorage(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="38439-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="38439-158">Response</span></span>

<span data-ttu-id="38439-159">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="38439-159">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="38439-160">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="38439-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Storage Used (Byte),Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="38439-161">JSON</span><span class="sxs-lookup"><span data-stu-id="38439-161">JSON</span></span>

<span data-ttu-id="38439-162">A seguir está um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="38439-162">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="38439-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="38439-163">Request</span></span>

<span data-ttu-id="38439-164">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="38439-164">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getmailboxusagestorage_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getMailboxUsageStorage(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="38439-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="38439-165">Response</span></span>

<span data-ttu-id="38439-166">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="38439-166">The following is an example of the response.</span></span>

> <span data-ttu-id="38439-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="38439-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxUsageStorage"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 235

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.mailboxUsageStorage)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "storageUsedInBytes": 5159432679270, 
      "reportDate": "2017-09-01", 
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


