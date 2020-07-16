---
title: 'reportRoot: getOffice365GroupsActivityCounts'
description: Obtenha o número de atividades de grupo em todas as cargas de trabalho de grupo.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 7323c8be8496e6e715d29af7318bbba74e77e269
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897376"
---
# <a name="reportroot-getoffice365groupsactivitycounts"></a><span data-ttu-id="83a05-103">reportRoot: getOffice365GroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="83a05-103">reportRoot: getOffice365GroupsActivityCounts</span></span>

<span data-ttu-id="83a05-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="83a05-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="83a05-105">Obtenha o número de atividades de grupo em todas as cargas de trabalho de grupo.</span><span class="sxs-lookup"><span data-stu-id="83a05-105">Get the number of group activities across group workloads.</span></span>

> <span data-ttu-id="83a05-106">**Observação:** Para obter detalhes sobre diferentes modos de exibição e nomes de relatórios, consulte [microsoft 365 Reports-microsoft 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span><span class="sxs-lookup"><span data-stu-id="83a05-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Microsoft 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="83a05-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="83a05-107">Permissions</span></span>

<span data-ttu-id="83a05-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83a05-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="83a05-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="83a05-110">Permission type</span></span>                        | <span data-ttu-id="83a05-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="83a05-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="83a05-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="83a05-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="83a05-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="83a05-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="83a05-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="83a05-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="83a05-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="83a05-115">Not supported.</span></span>                           |
| <span data-ttu-id="83a05-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="83a05-116">Application</span></span>                            | <span data-ttu-id="83a05-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="83a05-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="83a05-118">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="83a05-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="83a05-119">Para obter mais detalhes, consulte [Authorization for APIs to read Microsoft 365 Usage Reports](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="83a05-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="83a05-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="83a05-120">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="83a05-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="83a05-121">Function parameters</span></span>

<span data-ttu-id="83a05-122">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="83a05-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="83a05-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="83a05-123">Parameter</span></span> | <span data-ttu-id="83a05-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="83a05-124">Type</span></span>   | <span data-ttu-id="83a05-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="83a05-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="83a05-126">ponto</span><span class="sxs-lookup"><span data-stu-id="83a05-126">period</span></span>    | <span data-ttu-id="83a05-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="83a05-127">string</span></span> | <span data-ttu-id="83a05-128">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="83a05-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="83a05-129">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="83a05-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="83a05-130">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="83a05-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="83a05-131">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="83a05-131">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="83a05-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="83a05-132">Request headers</span></span>

| <span data-ttu-id="83a05-133">Nome</span><span class="sxs-lookup"><span data-stu-id="83a05-133">Name</span></span>          | <span data-ttu-id="83a05-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="83a05-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="83a05-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="83a05-135">Authorization</span></span> | <span data-ttu-id="83a05-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="83a05-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="83a05-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="83a05-138">If-None-Match</span></span> | <span data-ttu-id="83a05-139">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="83a05-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="83a05-140">Opcional.</span><span class="sxs-lookup"><span data-stu-id="83a05-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="83a05-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="83a05-141">Response</span></span>

<span data-ttu-id="83a05-142">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="83a05-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="83a05-143">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="83a05-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="83a05-144">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="83a05-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="83a05-145">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="83a05-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="83a05-146">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="83a05-146">Report Refresh Date</span></span>
- <span data-ttu-id="83a05-147">Emails recebidos do Exchange</span><span class="sxs-lookup"><span data-stu-id="83a05-147">Exchange Emails Received</span></span>
- <span data-ttu-id="83a05-148">Mensagens postadas do Yammer</span><span class="sxs-lookup"><span data-stu-id="83a05-148">Yammer Messages Posted</span></span>
- <span data-ttu-id="83a05-149">Mensagens lidas do Yammer</span><span class="sxs-lookup"><span data-stu-id="83a05-149">Yammer Messages Read</span></span>
- <span data-ttu-id="83a05-150">Mensagens curtidas do Yammer</span><span class="sxs-lookup"><span data-stu-id="83a05-150">Yammer Messages Liked</span></span>
- <span data-ttu-id="83a05-151">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="83a05-151">Report Date</span></span>
- <span data-ttu-id="83a05-152">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="83a05-152">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="83a05-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="83a05-153">Example</span></span>

#### <a name="request"></a><span data-ttu-id="83a05-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="83a05-154">Request</span></span>

<span data-ttu-id="83a05-155">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="83a05-155">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getoffice365groupsactivitycounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getOffice365GroupsActivityCounts(period='D7')
```


#### <a name="response"></a><span data-ttu-id="83a05-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="83a05-156">Response</span></span>

<span data-ttu-id="83a05-157">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="83a05-157">The following is an example of the response.</span></span>

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

<span data-ttu-id="83a05-158">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="83a05-158">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Exchange Emails Received,Yammer Messages Posted,Yammer Messages Read,Yammer Messages Liked,Report Date,Report Period
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
