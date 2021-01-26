---
title: 'reportRoot: getOffice365ActivationsUserCounts'
description: Obter a contagem de usuários que estão habilitados e aqueles que ativaram a assinatura do Office em computadores desktop ou dispositivos ou computadores compartilhados.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: a93a4207285d84dc9a9d748d85e43908aff2d13d
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49983724"
---
# <a name="reportroot-getoffice365activationsusercounts"></a><span data-ttu-id="321fe-103">reportRoot: getOffice365ActivationsUserCounts</span><span class="sxs-lookup"><span data-stu-id="321fe-103">reportRoot: getOffice365ActivationsUserCounts</span></span>

<span data-ttu-id="321fe-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="321fe-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="321fe-105">Obter a contagem de usuários que estão habilitados e aqueles que ativaram a assinatura do Office em computadores desktop ou dispositivos ou computadores compartilhados.</span><span class="sxs-lookup"><span data-stu-id="321fe-105">Get the count of users that are enabled and those that have activated the Office subscription on desktop or devices or shared computers.</span></span>

> <span data-ttu-id="321fe-106">**Observação:** Para obter detalhes sobre diferentes visualizações e nomes de relatórios, consulte [relatórios do Microsoft 365 - ativações do Microsoft Office.](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)</span><span class="sxs-lookup"><span data-stu-id="321fe-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="321fe-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="321fe-107">Permissions</span></span>

<span data-ttu-id="321fe-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="321fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="321fe-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="321fe-110">Permission type</span></span>                        | <span data-ttu-id="321fe-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="321fe-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="321fe-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="321fe-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="321fe-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="321fe-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="321fe-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="321fe-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="321fe-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="321fe-115">Not supported.</span></span>                           |
| <span data-ttu-id="321fe-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="321fe-116">Application</span></span>                            | <span data-ttu-id="321fe-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="321fe-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="321fe-118">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="321fe-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="321fe-119">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="321fe-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="321fe-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="321fe-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserCounts
```

## <a name="query-parameters"></a><span data-ttu-id="321fe-121">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="321fe-121">Query parameters</span></span>

<span data-ttu-id="321fe-122">Esse método dá suporte ao`$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="321fe-122">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="321fe-123">O tipo de saída padrão é texto/csv.</span><span class="sxs-lookup"><span data-stu-id="321fe-123">The default output type is text/csv.</span></span> <span data-ttu-id="321fe-124">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta $format OData definido como text/csv ou application/json.</span><span class="sxs-lookup"><span data-stu-id="321fe-124">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="321fe-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="321fe-125">Request headers</span></span>

| <span data-ttu-id="321fe-126">Nome</span><span class="sxs-lookup"><span data-stu-id="321fe-126">Name</span></span>          | <span data-ttu-id="321fe-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="321fe-127">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="321fe-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="321fe-128">Authorization</span></span> | <span data-ttu-id="321fe-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="321fe-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="321fe-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="321fe-131">Response</span></span>

### <a name="csv"></a><span data-ttu-id="321fe-132">CSV</span><span class="sxs-lookup"><span data-stu-id="321fe-132">CSV</span></span>

<span data-ttu-id="321fe-133">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="321fe-133">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="321fe-134">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="321fe-134">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="321fe-135">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="321fe-135">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="321fe-136">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="321fe-136">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="321fe-137">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="321fe-137">Report Refresh Date</span></span>
- <span data-ttu-id="321fe-138">Tipo de produto</span><span class="sxs-lookup"><span data-stu-id="321fe-138">Product Type</span></span>
- <span data-ttu-id="321fe-139">Atribuído</span><span class="sxs-lookup"><span data-stu-id="321fe-139">Assigned</span></span>
- <span data-ttu-id="321fe-140">Ativado</span><span class="sxs-lookup"><span data-stu-id="321fe-140">Activated</span></span>
- <span data-ttu-id="321fe-141">Ativação de computador compartilhado</span><span class="sxs-lookup"><span data-stu-id="321fe-141">Shared Computer Activation</span></span>

### <a name="json"></a><span data-ttu-id="321fe-142">JSON</span><span class="sxs-lookup"><span data-stu-id="321fe-142">JSON</span></span>

<span data-ttu-id="321fe-143">Se tiver êxito, este método retornará um código de resposta e um objeto `200 OK` **[office365ActivationsUserCounts](../resources/office365activationsusercounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="321fe-143">If successful, this method returns a `200 OK` response code and an **[office365ActivationsUserCounts](../resources/office365activationsusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="321fe-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="321fe-144">Example</span></span>

### <a name="csv"></a><span data-ttu-id="321fe-145">CSV</span><span class="sxs-lookup"><span data-stu-id="321fe-145">CSV</span></span>

<span data-ttu-id="321fe-146">A seguir está um exemplo que saída CSV.</span><span class="sxs-lookup"><span data-stu-id="321fe-146">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="321fe-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="321fe-147">Request</span></span>

<span data-ttu-id="321fe-148">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="321fe-148">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getoffice365activationsusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationsUserCounts?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="321fe-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="321fe-149">Response</span></span>

<span data-ttu-id="321fe-150">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="321fe-150">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="321fe-151">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="321fe-151">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Product Type,Assigned,Activated,Shared Computer Activation
```

### <a name="json"></a><span data-ttu-id="321fe-152">JSON</span><span class="sxs-lookup"><span data-stu-id="321fe-152">JSON</span></span>

<span data-ttu-id="321fe-153">A seguir está um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="321fe-153">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="321fe-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="321fe-154">Request</span></span>

<span data-ttu-id="321fe-155">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="321fe-155">The following example shows the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getoffice365activationsusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ActivationsUserCounts?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="321fe-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="321fe-156">Response</span></span>

<span data-ttu-id="321fe-157">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="321fe-157">The following example shows the response.</span></span>

> <span data-ttu-id="321fe-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="321fe-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365ActivationsUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 233

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365ActivationsUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "productType": "Microsoft 365 Apps for enterprise", 
      "assigned": 2679, 
      "activated": 1710,
      "sharedComputerActivation": 1024
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


