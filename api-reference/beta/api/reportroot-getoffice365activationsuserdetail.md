---
title: 'reportRoot: getOffice365ActivationsUserDetail'
description: Obtenha dados sobre usuários que ativaram o Office 365.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 8109acf37ee1f281b50b6fbfd304fa879e24cf6c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35988241"
---
# <a name="reportroot-getoffice365activationsuserdetail"></a><span data-ttu-id="791ab-103">reportRoot: getOffice365ActivationsUserDetail</span><span class="sxs-lookup"><span data-stu-id="791ab-103">reportRoot: getOffice365ActivationsUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="791ab-104">Obtenha dados sobre usuários que ativaram o Office 365.</span><span class="sxs-lookup"><span data-stu-id="791ab-104">Get details about users who have activated Office 365.</span></span>

> <span data-ttu-id="791ab-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Ativações do Microsoft Office](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="791ab-105">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="791ab-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="791ab-106">Permissions</span></span>

<span data-ttu-id="791ab-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="791ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="791ab-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="791ab-109">Permission type</span></span>                        | <span data-ttu-id="791ab-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="791ab-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="791ab-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="791ab-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="791ab-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="791ab-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="791ab-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="791ab-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="791ab-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="791ab-114">Not supported.</span></span>                           |
| <span data-ttu-id="791ab-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="791ab-115">Application</span></span>                            | <span data-ttu-id="791ab-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="791ab-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="791ab-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="791ab-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserDetail
```

## <a name="query-parameters"></a><span data-ttu-id="791ab-118">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="791ab-118">Query parameters</span></span>

<span data-ttu-id="791ab-119">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="791ab-119">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="791ab-120">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="791ab-120">The default output type is text/csv.</span></span> <span data-ttu-id="791ab-121">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="791ab-121">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="791ab-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="791ab-122">Request headers</span></span>

| <span data-ttu-id="791ab-123">Nome</span><span class="sxs-lookup"><span data-stu-id="791ab-123">Name</span></span>          | <span data-ttu-id="791ab-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="791ab-124">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="791ab-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="791ab-125">Authorization</span></span> | <span data-ttu-id="791ab-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="791ab-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="791ab-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="791ab-128">Response</span></span>

### <a name="csv"></a><span data-ttu-id="791ab-129">CSV</span><span class="sxs-lookup"><span data-stu-id="791ab-129">CSV</span></span>

<span data-ttu-id="791ab-130">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="791ab-130">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="791ab-131">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="791ab-131">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="791ab-132">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="791ab-132">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="791ab-133">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="791ab-133">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="791ab-134">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="791ab-134">Report Refresh Date</span></span>
- <span data-ttu-id="791ab-135">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="791ab-135">User Principal Name</span></span>
- <span data-ttu-id="791ab-136">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="791ab-136">Display Name</span></span>
- <span data-ttu-id="791ab-137">Tipo de produto</span><span class="sxs-lookup"><span data-stu-id="791ab-137">Product Type</span></span>
- <span data-ttu-id="791ab-138">Data da última ativação</span><span class="sxs-lookup"><span data-stu-id="791ab-138">Last Activated Date</span></span>
- <span data-ttu-id="791ab-139">Windows</span><span class="sxs-lookup"><span data-stu-id="791ab-139">Windows</span></span>
- <span data-ttu-id="791ab-140">Mac</span><span class="sxs-lookup"><span data-stu-id="791ab-140">Mac</span></span>
- <span data-ttu-id="791ab-141">Windows 10 Mobile</span><span class="sxs-lookup"><span data-stu-id="791ab-141">Windows 10 Mobile</span></span>
- <span data-ttu-id="791ab-142">iOS</span><span class="sxs-lookup"><span data-stu-id="791ab-142">iOS</span></span>
- <span data-ttu-id="791ab-143">Android</span><span class="sxs-lookup"><span data-stu-id="791ab-143">Android</span></span>
- <span data-ttu-id="791ab-144">Ativado no computador compartilhado</span><span class="sxs-lookup"><span data-stu-id="791ab-144">Activated On Shared Computer</span></span>

### <a name="json"></a><span data-ttu-id="791ab-145">JSON</span><span class="sxs-lookup"><span data-stu-id="791ab-145">JSON</span></span>

<span data-ttu-id="791ab-146">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[office365ActivationsUserDetail](../resources/office365activationsuserdetail.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="791ab-146">If successful, this method returns a `200 OK` response code and an **[office365ActivationsUserDetail](../resources/office365activationsuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="791ab-147">O tamanho de página padrão para essa solicitação é de 200 itens.</span><span class="sxs-lookup"><span data-stu-id="791ab-147">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="791ab-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="791ab-148">Example</span></span>

### <a name="csv"></a><span data-ttu-id="791ab-149">CSV</span><span class="sxs-lookup"><span data-stu-id="791ab-149">CSV</span></span>

<span data-ttu-id="791ab-150">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="791ab-150">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="791ab-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="791ab-151">Request</span></span>

<span data-ttu-id="791ab-152">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="791ab-152">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="791ab-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="791ab-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationsuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationsUserDetail?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="791ab-154">C#</span><span class="sxs-lookup"><span data-stu-id="791ab-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activationsuserdetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="791ab-155">Javascript</span><span class="sxs-lookup"><span data-stu-id="791ab-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activationsuserdetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="791ab-156">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="791ab-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activationsuserdetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="791ab-157">Java</span><span class="sxs-lookup"><span data-stu-id="791ab-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getoffice365activationsuserdetail-csv-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="791ab-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="791ab-158">Response</span></span>

<span data-ttu-id="791ab-159">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="791ab-159">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="791ab-160">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="791ab-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Product Type,Last Activated Date,Windows,Mac,Windows 10 Mobile,iOS,Android,Activated On Shared Computer
```

### <a name="json"></a><span data-ttu-id="791ab-161">JSON</span><span class="sxs-lookup"><span data-stu-id="791ab-161">JSON</span></span>

<span data-ttu-id="791ab-162">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="791ab-162">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="791ab-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="791ab-163">Request</span></span>

<span data-ttu-id="791ab-164">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="791ab-164">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="791ab-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="791ab-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationsuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationsUserDetail?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="791ab-166">C#</span><span class="sxs-lookup"><span data-stu-id="791ab-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activationsuserdetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="791ab-167">Javascript</span><span class="sxs-lookup"><span data-stu-id="791ab-167">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activationsuserdetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="791ab-168">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="791ab-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activationsuserdetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="791ab-169">Java</span><span class="sxs-lookup"><span data-stu-id="791ab-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getoffice365activationsuserdetail-json-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="791ab-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="791ab-170">Response</span></span>

<span data-ttu-id="791ab-171">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="791ab-171">The following is an example of the response.</span></span>

> <span data-ttu-id="791ab-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="791ab-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365ActivationsUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 400

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365ActivationsUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userprincipalname-value", 
      "displayName": "displayname-value", 
      "userActivationCounts": [
        {
          "productType": "Project Client", 
          "lastActivatedDate": "2017-08-20", 
          "windows": 5, 
          "mac": 0, 
          "windows10Mobile": 0, 
          "ios": 0, 
          "android": 2,
          "activatedOnSharedComputer": true
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
