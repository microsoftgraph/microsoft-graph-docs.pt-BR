---
title: 'reportRoot: getOffice365ActivationsUserDetail'
description: Obtenha dados sobre usuários que ativaram o Office 365.
ms.openlocfilehash: 1dbbfefc7ea620f0926b037bd138bb04ed362c5d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035407"
---
# <a name="reportroot-getoffice365activationsuserdetail"></a><span data-ttu-id="e6442-103">reportRoot: getOffice365ActivationsUserDetail</span><span class="sxs-lookup"><span data-stu-id="e6442-103">reportRoot: getOffice365ActivationsUserDetail</span></span>

> <span data-ttu-id="e6442-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e6442-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e6442-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e6442-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e6442-106">Obtenha dados sobre usuários que ativaram o Office 365.</span><span class="sxs-lookup"><span data-stu-id="e6442-106">Get details about users who have activated Office 365.</span></span>

> <span data-ttu-id="e6442-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Ativações do Microsoft Office](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="e6442-107">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="e6442-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="e6442-108">Permissions</span></span>

<span data-ttu-id="e6442-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6442-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e6442-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e6442-111">Permission type</span></span>                        | <span data-ttu-id="e6442-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e6442-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="e6442-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e6442-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="e6442-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e6442-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="e6442-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e6442-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e6442-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e6442-116">Not supported.</span></span>                           |
| <span data-ttu-id="e6442-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e6442-117">Application</span></span>                            | <span data-ttu-id="e6442-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e6442-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="e6442-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e6442-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserDetail
```

## <a name="query-parameters"></a><span data-ttu-id="e6442-120">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="e6442-120">Query parameters</span></span>

<span data-ttu-id="e6442-121">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$format`, `$top` e `$skipToken` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="e6442-121">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="e6442-122">O tipo de saída padrão é texto/csv.</span><span class="sxs-lookup"><span data-stu-id="e6442-122">The default output type is text/csv.</span></span> <span data-ttu-id="e6442-123">No entanto, se você deseja especificar o tipo de saída, você pode usar o parâmetro de consulta OData $format definido como texto/csv ou aplicativo/json.</span><span class="sxs-lookup"><span data-stu-id="e6442-123">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e6442-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e6442-124">Request headers</span></span>

| <span data-ttu-id="e6442-125">Nome</span><span class="sxs-lookup"><span data-stu-id="e6442-125">Name</span></span>          | <span data-ttu-id="e6442-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6442-126">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="e6442-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="e6442-127">Authorization</span></span> | <span data-ttu-id="e6442-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e6442-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="e6442-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6442-130">Response</span></span>

### <a name="csv"></a><span data-ttu-id="e6442-131">CSV</span><span class="sxs-lookup"><span data-stu-id="e6442-131">CSV</span></span>

<span data-ttu-id="e6442-132">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="e6442-132">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="e6442-133">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="e6442-133">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="e6442-134">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="e6442-134">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="e6442-135">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="e6442-135">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="e6442-136">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="e6442-136">Report Refresh Date</span></span>
- <span data-ttu-id="e6442-137">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="e6442-137">User Principal Name</span></span>
- <span data-ttu-id="e6442-138">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="e6442-138">Display Name</span></span>
- <span data-ttu-id="e6442-139">Tipo de produto</span><span class="sxs-lookup"><span data-stu-id="e6442-139">Product Type</span></span>
- <span data-ttu-id="e6442-140">Data da última ativação</span><span class="sxs-lookup"><span data-stu-id="e6442-140">Last Activated Date</span></span>
- <span data-ttu-id="e6442-141">Windows</span><span class="sxs-lookup"><span data-stu-id="e6442-141">Windows</span></span>
- <span data-ttu-id="e6442-142">Mac</span><span class="sxs-lookup"><span data-stu-id="e6442-142">Mac</span></span>
- <span data-ttu-id="e6442-143">Windows 10 Mobile</span><span class="sxs-lookup"><span data-stu-id="e6442-143">Windows 10 Mobile</span></span>
- <span data-ttu-id="e6442-144">iOS</span><span class="sxs-lookup"><span data-stu-id="e6442-144">iOS</span></span>
- <span data-ttu-id="e6442-145">Android</span><span class="sxs-lookup"><span data-stu-id="e6442-145">Android</span></span>
- <span data-ttu-id="e6442-146">Ativado no computador compartilhado</span><span class="sxs-lookup"><span data-stu-id="e6442-146">Activated On Shared Computer</span></span>

### <a name="json"></a><span data-ttu-id="e6442-147">JSON</span><span class="sxs-lookup"><span data-stu-id="e6442-147">JSON</span></span>

<span data-ttu-id="e6442-148">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **[office365ActivationsUserDetail](../resources/office365activationsuserdetail.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e6442-148">If successful, this method returns a `200 OK` response code and an **[office365ActivationsUserDetail](../resources/office365activationsuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="e6442-149">O tamanho de página padrão para essa solicitação é 200 itens.</span><span class="sxs-lookup"><span data-stu-id="e6442-149">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="e6442-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e6442-150">Example</span></span>

### <a name="csv"></a><span data-ttu-id="e6442-151">CSV</span><span class="sxs-lookup"><span data-stu-id="e6442-151">CSV</span></span>

<span data-ttu-id="e6442-152">O exemplo a seguir é um exemplo que emite CSV.</span><span class="sxs-lookup"><span data-stu-id="e6442-152">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="e6442-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e6442-153">Request</span></span>

<span data-ttu-id="e6442-154">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e6442-154">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationsuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationsUserDetail?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="e6442-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6442-155">Response</span></span>

<span data-ttu-id="e6442-156">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e6442-156">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="e6442-157">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="e6442-157">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="e6442-158">JSON</span><span class="sxs-lookup"><span data-stu-id="e6442-158">JSON</span></span>

<span data-ttu-id="e6442-159">O exemplo a seguir é um exemplo que retorne JSON.</span><span class="sxs-lookup"><span data-stu-id="e6442-159">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="e6442-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e6442-160">Request</span></span>

<span data-ttu-id="e6442-161">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e6442-161">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationsuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationsUserDetail?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="e6442-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6442-162">Response</span></span>

<span data-ttu-id="e6442-163">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e6442-163">The following is an example of the response.</span></span>

> <span data-ttu-id="e6442-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e6442-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
