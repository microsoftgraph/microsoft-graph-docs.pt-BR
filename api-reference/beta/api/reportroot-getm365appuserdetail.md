---
title: 'reportRoot: getM365AppUserDetail'
description: Obtenha um relatório que fornece os detalhes sobre quais aplicativos e plataformas os usuários usaram.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 7940a4fed4b11d54e9dddf98b192346eb184c698
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48975977"
---
# <a name="reportroot-getm365appuserdetail"></a><span data-ttu-id="642a3-103">reportRoot: getM365AppUserDetail</span><span class="sxs-lookup"><span data-stu-id="642a3-103">reportRoot: getM365AppUserDetail</span></span>

<span data-ttu-id="642a3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="642a3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="642a3-105">Obtenha um relatório que fornece os detalhes sobre quais aplicativos e plataformas os usuários usaram.</span><span class="sxs-lookup"><span data-stu-id="642a3-105">Get a report that provides the details about which apps and platforms users have used.</span></span>

> <span data-ttu-id="642a3-106">**Observação:** Para obter detalhes sobre diferentes modos de exibição e nomes de relatórios, consulte [microsoft 365 Reports-microsoft 365 apps Usage](/microsoft-365/admin/activity-reports/microsoft365-apps-usage).</span><span class="sxs-lookup"><span data-stu-id="642a3-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Microsoft 365 Apps usage](/microsoft-365/admin/activity-reports/microsoft365-apps-usage).</span></span>

## <a name="permissions"></a><span data-ttu-id="642a3-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="642a3-107">Permissions</span></span>

<span data-ttu-id="642a3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="642a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="642a3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="642a3-110">Permission type</span></span>                        | <span data-ttu-id="642a3-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="642a3-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="642a3-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="642a3-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="642a3-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="642a3-113">Reports.Read.All</span></span>                            |
| <span data-ttu-id="642a3-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="642a3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="642a3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="642a3-115">Not supported.</span></span>                              |
| <span data-ttu-id="642a3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="642a3-116">Application</span></span>                            | <span data-ttu-id="642a3-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="642a3-117">Reports.Read.All</span></span>                            |

> <span data-ttu-id="642a3-118">**Observação:** Para permissões delegadas para permitir que os aplicativos leiam relatórios de uso do serviço em nome de um usuário, o administrador do locatário deve ter atribuído ao usuário a função de administrador limitada do Azure AD apropriada.</span><span class="sxs-lookup"><span data-stu-id="642a3-118">**Note:** For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="642a3-119">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="642a3-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="642a3-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="642a3-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getM365AppUserDetail(period='{period_value}')
GET /reports/getM365AppUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="642a3-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="642a3-121">Function parameters</span></span>

<span data-ttu-id="642a3-122">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="642a3-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="642a3-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="642a3-123">Parameter</span></span> | <span data-ttu-id="642a3-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="642a3-124">Type</span></span>   | <span data-ttu-id="642a3-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="642a3-125">Description</span></span>                                                                                                                                                                                                                                             |
| :-------- | :----- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="642a3-126">ponto</span><span class="sxs-lookup"><span data-stu-id="642a3-126">period</span></span>    | <span data-ttu-id="642a3-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="642a3-127">string</span></span> | <span data-ttu-id="642a3-128">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="642a3-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="642a3-129">Os valores com suporte para {period_value} são: `D7` , `D30` , `D90` , e `D180` .</span><span class="sxs-lookup"><span data-stu-id="642a3-129">The supported values for {period_value} are: `D7`, `D30`, `D90`, and `D180`.</span></span> <span data-ttu-id="642a3-130">Eles seguem o formato D *n* , em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="642a3-130">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="642a3-131">data</span><span class="sxs-lookup"><span data-stu-id="642a3-131">date</span></span>      | <span data-ttu-id="642a3-132">Data</span><span class="sxs-lookup"><span data-stu-id="642a3-132">Date</span></span>   | <span data-ttu-id="642a3-133">Especifica a data para a qual você deseja visualizar os usuários que realizaram qualquer atividade.</span><span class="sxs-lookup"><span data-stu-id="642a3-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="642a3-134">{date_value} deve ter um formato de AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="642a3-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="642a3-135">Como este relatório está disponível apenas para os últimos 30 dias, {date_value} deve ser uma data desse intervalo.</span><span class="sxs-lookup"><span data-stu-id="642a3-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span>          |

> <span data-ttu-id="642a3-136">**Observação:** Você precisa definir `period` ou `date` na URL.</span><span class="sxs-lookup"><span data-stu-id="642a3-136">**Note:** You need to set either `period` or `date` in the URL.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="642a3-137">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="642a3-137">Optional query parameters</span></span>

<span data-ttu-id="642a3-138">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="642a3-138">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="642a3-139">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="642a3-139">The default output type is text/csv.</span></span> <span data-ttu-id="642a3-140">No entanto, se você quiser especificar o tipo de saída, poderá usar o `$format` parâmetro de consulta OData para definir a saída padrão como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="642a3-140">However, if you want to specify the output type, you can use the OData `$format` query parameter to set the default output to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="642a3-141">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="642a3-141">Request headers</span></span>

| <span data-ttu-id="642a3-142">Nome</span><span class="sxs-lookup"><span data-stu-id="642a3-142">Name</span></span>          | <span data-ttu-id="642a3-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="642a3-143">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="642a3-144">Autorização</span><span class="sxs-lookup"><span data-stu-id="642a3-144">Authorization</span></span> | <span data-ttu-id="642a3-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="642a3-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="642a3-147">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="642a3-147">Request body</span></span>

<span data-ttu-id="642a3-148">Não forneça um corpo de solicitação com esse método.</span><span class="sxs-lookup"><span data-stu-id="642a3-148">Do not supply a request body with this method.</span></span>

## <a name="response"></a><span data-ttu-id="642a3-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="642a3-149">Response</span></span>

<span data-ttu-id="642a3-150">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [Report](../resources/intune-shared-report.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="642a3-150">If successful, this method returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) object in the response body.</span></span> <span data-ttu-id="642a3-151">Os dados do relatório estão contidos na propriedade de **conteúdo** do objeto **Report** .</span><span class="sxs-lookup"><span data-stu-id="642a3-151">Report data is contained in the **content** property of the **report** object.</span></span>

### <a name="csv"></a><span data-ttu-id="642a3-152">CSV</span><span class="sxs-lookup"><span data-stu-id="642a3-152">CSV</span></span>

<span data-ttu-id="642a3-153">Se tiver êxito, solicitar a propriedade **Content** retornará uma `302 Found` resposta que REDIRECIONA para uma URL de download autenticado para o relatório.</span><span class="sxs-lookup"><span data-stu-id="642a3-153">If successful, requesting the **content** property returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="642a3-154">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="642a3-154">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="642a3-155">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="642a3-155">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="642a3-156">O arquivo CSV possui os seguintes cabeçalhos para colunas:</span><span class="sxs-lookup"><span data-stu-id="642a3-156">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="642a3-157">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="642a3-157">Report Refresh Date</span></span>
- <span data-ttu-id="642a3-158">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="642a3-158">User Principal Name</span></span>
- <span data-ttu-id="642a3-159">Data da última ativação</span><span class="sxs-lookup"><span data-stu-id="642a3-159">Last Activation Date</span></span>
- <span data-ttu-id="642a3-160">Data da última atividade</span><span class="sxs-lookup"><span data-stu-id="642a3-160">Last Activity Date</span></span>
- <span data-ttu-id="642a3-161">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="642a3-161">Report Period</span></span>
- <span data-ttu-id="642a3-162">Windows</span><span class="sxs-lookup"><span data-stu-id="642a3-162">Windows</span></span>
- <span data-ttu-id="642a3-163">Mac</span><span class="sxs-lookup"><span data-stu-id="642a3-163">Mac</span></span>
- <span data-ttu-id="642a3-164">Mobile</span><span class="sxs-lookup"><span data-stu-id="642a3-164">Mobile</span></span>
- <span data-ttu-id="642a3-165">Web</span><span class="sxs-lookup"><span data-stu-id="642a3-165">Web</span></span>
- <span data-ttu-id="642a3-166">Outlook</span><span class="sxs-lookup"><span data-stu-id="642a3-166">Outlook</span></span>
- <span data-ttu-id="642a3-167">Word</span><span class="sxs-lookup"><span data-stu-id="642a3-167">Word</span></span>
- <span data-ttu-id="642a3-168">Excel</span><span class="sxs-lookup"><span data-stu-id="642a3-168">Excel</span></span>
- <span data-ttu-id="642a3-169">PowerPoint</span><span class="sxs-lookup"><span data-stu-id="642a3-169">PowerPoint</span></span>
- <span data-ttu-id="642a3-170">OneNote</span><span class="sxs-lookup"><span data-stu-id="642a3-170">OneNote</span></span>
- <span data-ttu-id="642a3-171">Teams</span><span class="sxs-lookup"><span data-stu-id="642a3-171">Teams</span></span>
- <span data-ttu-id="642a3-172">Outlook (Windows)</span><span class="sxs-lookup"><span data-stu-id="642a3-172">Outlook (Windows)</span></span>
- <span data-ttu-id="642a3-173">Word (Windows)</span><span class="sxs-lookup"><span data-stu-id="642a3-173">Word (Windows)</span></span>
- <span data-ttu-id="642a3-174">Excel (Windows)</span><span class="sxs-lookup"><span data-stu-id="642a3-174">Excel (Windows)</span></span>
- <span data-ttu-id="642a3-175">PowerPoint (Windows)</span><span class="sxs-lookup"><span data-stu-id="642a3-175">PowerPoint (Windows)</span></span>
- <span data-ttu-id="642a3-176">OneNote (Windows)</span><span class="sxs-lookup"><span data-stu-id="642a3-176">OneNote (Windows)</span></span>
- <span data-ttu-id="642a3-177">Teams (Windows)</span><span class="sxs-lookup"><span data-stu-id="642a3-177">Teams (Windows)</span></span>
- <span data-ttu-id="642a3-178">Outlook (Mac)</span><span class="sxs-lookup"><span data-stu-id="642a3-178">Outlook (Mac)</span></span>
- <span data-ttu-id="642a3-179">Word (Mac)</span><span class="sxs-lookup"><span data-stu-id="642a3-179">Word (Mac)</span></span>
- <span data-ttu-id="642a3-180">Excel (Mac)</span><span class="sxs-lookup"><span data-stu-id="642a3-180">Excel (Mac)</span></span>
- <span data-ttu-id="642a3-181">PowerPoint (Mac)</span><span class="sxs-lookup"><span data-stu-id="642a3-181">PowerPoint (Mac)</span></span>
- <span data-ttu-id="642a3-182">OneNote (Mac)</span><span class="sxs-lookup"><span data-stu-id="642a3-182">OneNote (Mac)</span></span>
- <span data-ttu-id="642a3-183">Teams (Mac)</span><span class="sxs-lookup"><span data-stu-id="642a3-183">Teams (Mac)</span></span>
- <span data-ttu-id="642a3-184">Outlook (celular)</span><span class="sxs-lookup"><span data-stu-id="642a3-184">Outlook (Mobile)</span></span>
- <span data-ttu-id="642a3-185">Word (celular)</span><span class="sxs-lookup"><span data-stu-id="642a3-185">Word (Mobile)</span></span>
- <span data-ttu-id="642a3-186">Excel (celular)</span><span class="sxs-lookup"><span data-stu-id="642a3-186">Excel (Mobile)</span></span>
- <span data-ttu-id="642a3-187">PowerPoint (móvel)</span><span class="sxs-lookup"><span data-stu-id="642a3-187">PowerPoint (Mobile)</span></span>
- <span data-ttu-id="642a3-188">OneNote (celular)</span><span class="sxs-lookup"><span data-stu-id="642a3-188">OneNote (Mobile)</span></span>
- <span data-ttu-id="642a3-189">Teams (celular)</span><span class="sxs-lookup"><span data-stu-id="642a3-189">Teams (Mobile)</span></span>
- <span data-ttu-id="642a3-190">Outlook (Web)</span><span class="sxs-lookup"><span data-stu-id="642a3-190">Outlook (Web)</span></span>
- <span data-ttu-id="642a3-191">Word (Web)</span><span class="sxs-lookup"><span data-stu-id="642a3-191">Word (Web)</span></span>
- <span data-ttu-id="642a3-192">Excel (Web)</span><span class="sxs-lookup"><span data-stu-id="642a3-192">Excel (Web)</span></span>
- <span data-ttu-id="642a3-193">PowerPoint (Web)</span><span class="sxs-lookup"><span data-stu-id="642a3-193">PowerPoint (Web)</span></span>
- <span data-ttu-id="642a3-194">OneNote (Web)</span><span class="sxs-lookup"><span data-stu-id="642a3-194">OneNote (Web)</span></span>
- <span data-ttu-id="642a3-195">Teams (Web)</span><span class="sxs-lookup"><span data-stu-id="642a3-195">Teams (Web)</span></span>

### <a name="json"></a><span data-ttu-id="642a3-196">JSON</span><span class="sxs-lookup"><span data-stu-id="642a3-196">JSON</span></span>

<span data-ttu-id="642a3-197">Se bem-sucedido, solicitar a propriedade **Content** retorna um `200 OK` código de resposta e um objeto JSON no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="642a3-197">If successful, requesting the **content** property returns a `200 OK` response code and a JSON object in response body.</span></span>

<span data-ttu-id="642a3-198">O tamanho de página padrão para essa solicitação é de 200 itens.</span><span class="sxs-lookup"><span data-stu-id="642a3-198">The default page size for this request is 200 items.</span></span>

## <a name="examples"></a><span data-ttu-id="642a3-199">Exemplos</span><span class="sxs-lookup"><span data-stu-id="642a3-199">Examples</span></span>

### <a name="example-1-csv-output"></a><span data-ttu-id="642a3-200">Exemplo 1: saída CSV</span><span class="sxs-lookup"><span data-stu-id="642a3-200">Example 1: CSV output</span></span>

<span data-ttu-id="642a3-201">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="642a3-201">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="642a3-202">Solicitação</span><span class="sxs-lookup"><span data-stu-id="642a3-202">Request</span></span>

<span data-ttu-id="642a3-203">Veja a seguir um exemplo da solicitação para obter a propriedade de **conteúdo** .</span><span class="sxs-lookup"><span data-stu-id="642a3-203">The following is an example of the request to get the **content** property.</span></span>



# <a name="http"></a>[<span data-ttu-id="642a3-204">HTTP</span><span class="sxs-lookup"><span data-stu-id="642a3-204">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getM365AppUserCounDetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getM365AppUserDetail(period='D7')/content?$format=text/csv
```
# <a name="c"></a>[<span data-ttu-id="642a3-205">C#</span><span class="sxs-lookup"><span data-stu-id="642a3-205">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getm365appusercoundetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="642a3-206">JavaScript</span><span class="sxs-lookup"><span data-stu-id="642a3-206">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getm365appusercoundetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="642a3-207">Objective-C</span><span class="sxs-lookup"><span data-stu-id="642a3-207">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getm365appusercoundetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="642a3-208">Java</span><span class="sxs-lookup"><span data-stu-id="642a3-208">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getm365appusercoundetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="642a3-209">Resposta</span><span class="sxs-lookup"><span data-stu-id="642a3-209">Response</span></span>

<span data-ttu-id="642a3-210">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="642a3-210">The following is an example of the response.</span></span>

<!-- { "blockType": "response" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="642a3-211">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="642a3-211">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Last Activation Date,Last Activity Date,Report Period,Windows,Mac,Mobile,Web,Outlook,Word,Excel,PowerPoint,OneNote,Teams,Outlook (Windows),Word (Windows),Excel (Windows),PowerPoint (Windows),OneNote (Windows),Teams (Windows),Outlook (Mac),Word (Mac),Excel (Mac),PowerPoint (Mac),OneNote (Mac),Teams (Mac),Outlook (Mobile),Word (Mobile),Excel (Mobile),PowerPoint (Mobile),OneNote (Mobile),Teams (Mobile),Outlook (Web),Word (Web),Excel (Web),PowerPoint (Web),OneNote (Web),Teams (Web)
```

### <a name="example-2-json-output"></a><span data-ttu-id="642a3-212">Exemplo 2: saída JSON</span><span class="sxs-lookup"><span data-stu-id="642a3-212">Example 2: JSON output</span></span>

<span data-ttu-id="642a3-213">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="642a3-213">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="642a3-214">Solicitação</span><span class="sxs-lookup"><span data-stu-id="642a3-214">Request</span></span>

<span data-ttu-id="642a3-215">Veja a seguir um exemplo da solicitação para obter a propriedade de **conteúdo** .</span><span class="sxs-lookup"><span data-stu-id="642a3-215">The following is an example of the request to get the **content** property.</span></span>



# <a name="http"></a>[<span data-ttu-id="642a3-216">HTTP</span><span class="sxs-lookup"><span data-stu-id="642a3-216">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getM365AppUserCountDetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getM365AppUserDetail(period='D7')/content?$format=application/json
```
# <a name="c"></a>[<span data-ttu-id="642a3-217">C#</span><span class="sxs-lookup"><span data-stu-id="642a3-217">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getm365appusercountdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="642a3-218">JavaScript</span><span class="sxs-lookup"><span data-stu-id="642a3-218">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getm365appusercountdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="642a3-219">Objective-C</span><span class="sxs-lookup"><span data-stu-id="642a3-219">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getm365appusercountdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="642a3-220">Java</span><span class="sxs-lookup"><span data-stu-id="642a3-220">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getm365appusercountdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="642a3-221">Resposta</span><span class="sxs-lookup"><span data-stu-id="642a3-221">Response</span></span>

<span data-ttu-id="642a3-222">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="642a3-222">The following is an example of the response.</span></span>

> <span data-ttu-id="642a3-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="642a3-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 951

{
  "@odata.nextLink": "https://graph.microsoft.com/beta/reports/getM365AppUserDetail(period='D7')/content?$format=application/json&$skiptoken=AAAAA",
  "value": [
    {
      "reportRefreshDate": "2020-06-30",
      "userPrincipalName": "admin@contoso.com",
      "lastActivationDate": "2020-05-22",
      "lastActivityDate": "2020-06-30",
      "details": [
        {
          "reportPeriod": 7,
          "windows": true,
          "mac": false,
          "mobile": true,
          "web": false,
          "outlook": false,
          "word": false,
          "excel": false,
          "powerPoint": false,
          "oneNote": false,
          "teams": true,
          "outlookWindows": false,
          "wordWindows": false,
          "excelWindows": false,
          "powerPointWindows": false,
          "oneNoteWindows": false,
          "teamsWindows": true,
          "outlookMac": false,
          "wordMac": false,
          "excelMac": false,
          "powerPointMac": false,
          "oneNoteMac": false,
          "teamsMac": false,
          "outlookMobile": false,
          "wordMobile": false,
          "excelMobile": false,
          "powerPointMobile": false,
          "oneNoteMobile": false,
          "teamsMobile": true,
          "outlookWeb": false,
          "wordWeb": false,
          "excelWeb": false,
          "powerPointWeb": false,
          "oneNoteWeb": false,
          "teamsWeb": true
        }
      ]
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
