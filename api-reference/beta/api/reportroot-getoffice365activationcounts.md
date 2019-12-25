---
title: 'reportRoot: getOffice365ActivationCounts'
description: Obtenha a contagem de ativações do Office 365 em desktops e dispositivos.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: f71a38c9c3d2264a0414bf03041d7a9132bfccb9
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40869148"
---
# <a name="reportroot-getoffice365activationcounts"></a><span data-ttu-id="37fec-103">reportRoot: getOffice365ActivationCounts</span><span class="sxs-lookup"><span data-stu-id="37fec-103">reportRoot: getOffice365ActivationCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37fec-104">Obtenha a contagem de ativações do Office 365 em desktops e dispositivos.</span><span class="sxs-lookup"><span data-stu-id="37fec-104">Get the count of Office 365 activations on desktops and devices.</span></span>

> <span data-ttu-id="37fec-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Ativações do Microsoft Office](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="37fec-105">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="37fec-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="37fec-106">Permissions</span></span>

<span data-ttu-id="37fec-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37fec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="37fec-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="37fec-109">Permission type</span></span>                        | <span data-ttu-id="37fec-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="37fec-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="37fec-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="37fec-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="37fec-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="37fec-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="37fec-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="37fec-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37fec-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="37fec-114">Not supported.</span></span>                           |
| <span data-ttu-id="37fec-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="37fec-115">Application</span></span>                            | <span data-ttu-id="37fec-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="37fec-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="37fec-117">**Observação**: para permissões delegadas para permitir que os aplicativos leiam relatórios de uso do serviço em nome de um usuário, o administrador do locatário deve ter atribuído ao usuário a função de administrador limitada do Azure ad apropriada.</span><span class="sxs-lookup"><span data-stu-id="37fec-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="37fec-118">Para obter mais detalhes, consulte [Authorization for APIs to read Office 365 Usage Reports](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="37fec-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="37fec-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="37fec-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationCounts
```

## <a name="query-parameters"></a><span data-ttu-id="37fec-120">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="37fec-120">Query parameters</span></span>

<span data-ttu-id="37fec-121">Esse método dá suporte ao`$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="37fec-121">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="37fec-122">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="37fec-122">The default output type is text/csv.</span></span> <span data-ttu-id="37fec-123">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="37fec-123">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="37fec-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="37fec-124">Request headers</span></span>

| <span data-ttu-id="37fec-125">Nome</span><span class="sxs-lookup"><span data-stu-id="37fec-125">Name</span></span>          | <span data-ttu-id="37fec-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="37fec-126">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="37fec-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="37fec-127">Authorization</span></span> | <span data-ttu-id="37fec-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="37fec-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="37fec-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="37fec-130">Response</span></span>

### <a name="csv"></a><span data-ttu-id="37fec-131">CSV</span><span class="sxs-lookup"><span data-stu-id="37fec-131">CSV</span></span>

<span data-ttu-id="37fec-132">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="37fec-132">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="37fec-133">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="37fec-133">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="37fec-134">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="37fec-134">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="37fec-135">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="37fec-135">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="37fec-136">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="37fec-136">Report Refresh Date</span></span>
- <span data-ttu-id="37fec-137">Tipo de produto</span><span class="sxs-lookup"><span data-stu-id="37fec-137">Product Type</span></span>
- <span data-ttu-id="37fec-138">Windows</span><span class="sxs-lookup"><span data-stu-id="37fec-138">Windows</span></span>
- <span data-ttu-id="37fec-139">Mac</span><span class="sxs-lookup"><span data-stu-id="37fec-139">Mac</span></span>
- <span data-ttu-id="37fec-140">Android</span><span class="sxs-lookup"><span data-stu-id="37fec-140">Android</span></span>
- <span data-ttu-id="37fec-141">iOS</span><span class="sxs-lookup"><span data-stu-id="37fec-141">iOS</span></span>
- <span data-ttu-id="37fec-142">Windows 10 Mobile</span><span class="sxs-lookup"><span data-stu-id="37fec-142">Windows 10 Mobile</span></span>

### <a name="json"></a><span data-ttu-id="37fec-143">JSON</span><span class="sxs-lookup"><span data-stu-id="37fec-143">JSON</span></span>

<span data-ttu-id="37fec-144">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[office365ActivationCounts](../resources/office365activationcounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="37fec-144">If successful, this method returns a `200 OK` response code and an **[office365ActivationCounts](../resources/office365activationcounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37fec-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="37fec-145">Example</span></span>

### <a name="csv"></a><span data-ttu-id="37fec-146">CSV</span><span class="sxs-lookup"><span data-stu-id="37fec-146">CSV</span></span>

<span data-ttu-id="37fec-147">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="37fec-147">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="37fec-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="37fec-148">Request</span></span>

<span data-ttu-id="37fec-149">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="37fec-149">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="37fec-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="37fec-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationcounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationCounts?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="37fec-151">C#</span><span class="sxs-lookup"><span data-stu-id="37fec-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activationcounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="37fec-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="37fec-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activationcounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="37fec-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="37fec-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activationcounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="37fec-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="37fec-154">Response</span></span>

<span data-ttu-id="37fec-155">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="37fec-155">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="37fec-156">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="37fec-156">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Product Type,Windows,Mac,Android,iOS,Windows 10 Mobile
```

### <a name="json"></a><span data-ttu-id="37fec-157">JSON</span><span class="sxs-lookup"><span data-stu-id="37fec-157">JSON</span></span>

<span data-ttu-id="37fec-158">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="37fec-158">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="37fec-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="37fec-159">Request</span></span>

<span data-ttu-id="37fec-160">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="37fec-160">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="37fec-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="37fec-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationcounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationCounts?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="37fec-162">C#</span><span class="sxs-lookup"><span data-stu-id="37fec-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activationcounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="37fec-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="37fec-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activationcounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="37fec-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="37fec-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activationcounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="37fec-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="37fec-165">Response</span></span>

<span data-ttu-id="37fec-166">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="37fec-166">The following example shows the response.</span></span>

> <span data-ttu-id="37fec-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="37fec-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365ActivationCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 268

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365ActivationCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "productType": "Office 365 ProPlus", 
      "windows": 9157, 
      "mac": 576, 
      "android": 358, 
      "ios": 1452, 
      "windows10Mobile": 2309
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
