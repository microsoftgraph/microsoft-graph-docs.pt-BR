---
title: 'reportRoot: getOffice365ActivationsUserDetail'
description: Obtenha dados sobre usuários que ativaram o Office 365.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: bdab2bdfe628f8a1b9bffef59806969ad1d6c03a
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40869161"
---
# <a name="reportroot-getoffice365activationsuserdetail"></a><span data-ttu-id="89eeb-103">reportRoot: getOffice365ActivationsUserDetail</span><span class="sxs-lookup"><span data-stu-id="89eeb-103">reportRoot: getOffice365ActivationsUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="89eeb-104">Obtenha dados sobre usuários que ativaram o Office 365.</span><span class="sxs-lookup"><span data-stu-id="89eeb-104">Get details about users who have activated Office 365.</span></span>

> <span data-ttu-id="89eeb-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Ativações do Microsoft Office](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="89eeb-105">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="89eeb-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="89eeb-106">Permissions</span></span>

<span data-ttu-id="89eeb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89eeb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="89eeb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="89eeb-109">Permission type</span></span>                        | <span data-ttu-id="89eeb-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="89eeb-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="89eeb-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="89eeb-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="89eeb-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="89eeb-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="89eeb-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="89eeb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89eeb-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="89eeb-114">Not supported.</span></span>                           |
| <span data-ttu-id="89eeb-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="89eeb-115">Application</span></span>                            | <span data-ttu-id="89eeb-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="89eeb-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="89eeb-117">**Observação**: para permissões delegadas para permitir que os aplicativos leiam relatórios de uso do serviço em nome de um usuário, o administrador do locatário deve ter atribuído ao usuário a função de administrador limitada do Azure ad apropriada.</span><span class="sxs-lookup"><span data-stu-id="89eeb-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="89eeb-118">Para obter mais detalhes, consulte [Authorization for APIs to read Office 365 Usage Reports](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="89eeb-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="89eeb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="89eeb-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserDetail
```

## <a name="query-parameters"></a><span data-ttu-id="89eeb-120">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="89eeb-120">Query parameters</span></span>

<span data-ttu-id="89eeb-121">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="89eeb-121">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="89eeb-122">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="89eeb-122">The default output type is text/csv.</span></span> <span data-ttu-id="89eeb-123">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="89eeb-123">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="89eeb-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="89eeb-124">Request headers</span></span>

| <span data-ttu-id="89eeb-125">Nome</span><span class="sxs-lookup"><span data-stu-id="89eeb-125">Name</span></span>          | <span data-ttu-id="89eeb-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="89eeb-126">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="89eeb-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="89eeb-127">Authorization</span></span> | <span data-ttu-id="89eeb-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="89eeb-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="89eeb-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="89eeb-130">Response</span></span>

### <a name="csv"></a><span data-ttu-id="89eeb-131">CSV</span><span class="sxs-lookup"><span data-stu-id="89eeb-131">CSV</span></span>

<span data-ttu-id="89eeb-132">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="89eeb-132">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="89eeb-133">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="89eeb-133">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="89eeb-134">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="89eeb-134">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="89eeb-135">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="89eeb-135">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="89eeb-136">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="89eeb-136">Report Refresh Date</span></span>
- <span data-ttu-id="89eeb-137">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="89eeb-137">User Principal Name</span></span>
- <span data-ttu-id="89eeb-138">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="89eeb-138">Display Name</span></span>
- <span data-ttu-id="89eeb-139">Tipo de produto</span><span class="sxs-lookup"><span data-stu-id="89eeb-139">Product Type</span></span>
- <span data-ttu-id="89eeb-140">Data da última ativação</span><span class="sxs-lookup"><span data-stu-id="89eeb-140">Last Activated Date</span></span>
- <span data-ttu-id="89eeb-141">Windows</span><span class="sxs-lookup"><span data-stu-id="89eeb-141">Windows</span></span>
- <span data-ttu-id="89eeb-142">Mac</span><span class="sxs-lookup"><span data-stu-id="89eeb-142">Mac</span></span>
- <span data-ttu-id="89eeb-143">Windows 10 Mobile</span><span class="sxs-lookup"><span data-stu-id="89eeb-143">Windows 10 Mobile</span></span>
- <span data-ttu-id="89eeb-144">iOS</span><span class="sxs-lookup"><span data-stu-id="89eeb-144">iOS</span></span>
- <span data-ttu-id="89eeb-145">Android</span><span class="sxs-lookup"><span data-stu-id="89eeb-145">Android</span></span>
- <span data-ttu-id="89eeb-146">Ativado no computador compartilhado</span><span class="sxs-lookup"><span data-stu-id="89eeb-146">Activated On Shared Computer</span></span>

### <a name="json"></a><span data-ttu-id="89eeb-147">JSON</span><span class="sxs-lookup"><span data-stu-id="89eeb-147">JSON</span></span>

<span data-ttu-id="89eeb-148">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **[office365ActivationsUserDetail](../resources/office365activationsuserdetail.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="89eeb-148">If successful, this method returns a `200 OK` response code and an **[office365ActivationsUserDetail](../resources/office365activationsuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="89eeb-149">O tamanho de página padrão para essa solicitação é de 200 itens.</span><span class="sxs-lookup"><span data-stu-id="89eeb-149">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="89eeb-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="89eeb-150">Example</span></span>

### <a name="csv"></a><span data-ttu-id="89eeb-151">CSV</span><span class="sxs-lookup"><span data-stu-id="89eeb-151">CSV</span></span>

<span data-ttu-id="89eeb-152">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="89eeb-152">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="89eeb-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="89eeb-153">Request</span></span>

<span data-ttu-id="89eeb-154">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="89eeb-154">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="89eeb-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="89eeb-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationsuserdetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationsUserDetail?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="89eeb-156">C#</span><span class="sxs-lookup"><span data-stu-id="89eeb-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activationsuserdetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="89eeb-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="89eeb-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activationsuserdetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="89eeb-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="89eeb-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activationsuserdetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="89eeb-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="89eeb-159">Response</span></span>

<span data-ttu-id="89eeb-160">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="89eeb-160">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="89eeb-161">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="89eeb-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="89eeb-162">JSON</span><span class="sxs-lookup"><span data-stu-id="89eeb-162">JSON</span></span>

<span data-ttu-id="89eeb-163">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="89eeb-163">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="89eeb-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="89eeb-164">Request</span></span>

<span data-ttu-id="89eeb-165">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="89eeb-165">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="89eeb-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="89eeb-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationsuserdetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationsUserDetail?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="89eeb-167">C#</span><span class="sxs-lookup"><span data-stu-id="89eeb-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activationsuserdetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="89eeb-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="89eeb-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activationsuserdetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="89eeb-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="89eeb-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activationsuserdetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="89eeb-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="89eeb-170">Response</span></span>

<span data-ttu-id="89eeb-171">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="89eeb-171">The following is an example of the response.</span></span>

> <span data-ttu-id="89eeb-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="89eeb-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
