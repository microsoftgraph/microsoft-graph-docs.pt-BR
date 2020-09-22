---
title: 'reportRoot: getOffice365ActivationsUserDetail'
description: Obtenha detalhes sobre os usuários que ativaram o Microsoft 365.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 758bad37777b55c3a611f3c949cc5d96c3c953d2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48067691"
---
# <a name="reportroot-getoffice365activationsuserdetail"></a><span data-ttu-id="2f210-103">reportRoot: getOffice365ActivationsUserDetail</span><span class="sxs-lookup"><span data-stu-id="2f210-103">reportRoot: getOffice365ActivationsUserDetail</span></span>

<span data-ttu-id="2f210-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f210-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f210-105">Obtenha detalhes sobre os usuários que ativaram o Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="2f210-105">Get details about users who have activated Microsoft 365.</span></span>

> <span data-ttu-id="2f210-106">**Observação:** Para obter detalhes sobre diferentes modos de exibição e nomes de relatórios, consulte [microsoft 365 Reports-Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="2f210-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="2f210-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="2f210-107">Permissions</span></span>

<span data-ttu-id="2f210-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f210-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2f210-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2f210-110">Permission type</span></span>                        | <span data-ttu-id="2f210-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2f210-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="2f210-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2f210-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="2f210-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2f210-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="2f210-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2f210-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2f210-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2f210-115">Not supported.</span></span>                           |
| <span data-ttu-id="2f210-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2f210-116">Application</span></span>                            | <span data-ttu-id="2f210-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2f210-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="2f210-118">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="2f210-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="2f210-119">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="2f210-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="2f210-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2f210-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserDetail
```

## <a name="query-parameters"></a><span data-ttu-id="2f210-121">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="2f210-121">Query parameters</span></span>

<span data-ttu-id="2f210-122">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="2f210-122">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="2f210-123">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="2f210-123">The default output type is text/csv.</span></span> <span data-ttu-id="2f210-124">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="2f210-124">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2f210-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2f210-125">Request headers</span></span>

| <span data-ttu-id="2f210-126">Nome</span><span class="sxs-lookup"><span data-stu-id="2f210-126">Name</span></span>          | <span data-ttu-id="2f210-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f210-127">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="2f210-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="2f210-128">Authorization</span></span> | <span data-ttu-id="2f210-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2f210-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="2f210-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f210-131">Response</span></span>

### <a name="csv"></a><span data-ttu-id="2f210-132">CSV</span><span class="sxs-lookup"><span data-stu-id="2f210-132">CSV</span></span>

<span data-ttu-id="2f210-133">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="2f210-133">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="2f210-134">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="2f210-134">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="2f210-135">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="2f210-135">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="2f210-136">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="2f210-136">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="2f210-137">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="2f210-137">Report Refresh Date</span></span>
- <span data-ttu-id="2f210-138">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="2f210-138">User Principal Name</span></span>
- <span data-ttu-id="2f210-139">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="2f210-139">Display Name</span></span>
- <span data-ttu-id="2f210-140">Tipo de produto</span><span class="sxs-lookup"><span data-stu-id="2f210-140">Product Type</span></span>
- <span data-ttu-id="2f210-141">Data da última ativação</span><span class="sxs-lookup"><span data-stu-id="2f210-141">Last Activated Date</span></span>
- <span data-ttu-id="2f210-142">Windows</span><span class="sxs-lookup"><span data-stu-id="2f210-142">Windows</span></span>
- <span data-ttu-id="2f210-143">Mac</span><span class="sxs-lookup"><span data-stu-id="2f210-143">Mac</span></span>
- <span data-ttu-id="2f210-144">Windows 10 Mobile</span><span class="sxs-lookup"><span data-stu-id="2f210-144">Windows 10 Mobile</span></span>
- <span data-ttu-id="2f210-145">iOS</span><span class="sxs-lookup"><span data-stu-id="2f210-145">iOS</span></span>
- <span data-ttu-id="2f210-146">Android</span><span class="sxs-lookup"><span data-stu-id="2f210-146">Android</span></span>
- <span data-ttu-id="2f210-147">Ativado no computador compartilhado</span><span class="sxs-lookup"><span data-stu-id="2f210-147">Activated On Shared Computer</span></span>

### <a name="json"></a><span data-ttu-id="2f210-148">JSON</span><span class="sxs-lookup"><span data-stu-id="2f210-148">JSON</span></span>

<span data-ttu-id="2f210-149">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **[office365ActivationsUserDetail](../resources/office365activationsuserdetail.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2f210-149">If successful, this method returns a `200 OK` response code and an **[office365ActivationsUserDetail](../resources/office365activationsuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="2f210-150">O tamanho de página padrão para essa solicitação é de 200 itens.</span><span class="sxs-lookup"><span data-stu-id="2f210-150">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="2f210-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2f210-151">Example</span></span>

### <a name="csv"></a><span data-ttu-id="2f210-152">CSV</span><span class="sxs-lookup"><span data-stu-id="2f210-152">CSV</span></span>

<span data-ttu-id="2f210-153">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="2f210-153">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="2f210-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f210-154">Request</span></span>

<span data-ttu-id="2f210-155">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2f210-155">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getoffice365activationsuserdetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationsUserDetail?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="2f210-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f210-156">Response</span></span>

<span data-ttu-id="2f210-157">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2f210-157">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="2f210-158">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="2f210-158">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="2f210-159">JSON</span><span class="sxs-lookup"><span data-stu-id="2f210-159">JSON</span></span>

<span data-ttu-id="2f210-160">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="2f210-160">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="2f210-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f210-161">Request</span></span>

<span data-ttu-id="2f210-162">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2f210-162">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getoffice365activationsuserdetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationsUserDetail?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="2f210-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f210-163">Response</span></span>

<span data-ttu-id="2f210-164">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2f210-164">The following is an example of the response.</span></span>

> <span data-ttu-id="2f210-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2f210-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


