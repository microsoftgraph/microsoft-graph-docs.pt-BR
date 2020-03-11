---
title: 'reportRoot: getOffice365ActiveUserCounts'
description: Obtenha a contagem de usuários ativos diários no período de relatório por produto.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 05a2bef267a20d8566ac96baf4f0eee222e9d577
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2020
ms.locfileid: "42591296"
---
# <a name="reportroot-getoffice365activeusercounts"></a><span data-ttu-id="76176-103">reportRoot: getOffice365ActiveUserCounts</span><span class="sxs-lookup"><span data-stu-id="76176-103">reportRoot: getOffice365ActiveUserCounts</span></span>

<span data-ttu-id="76176-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76176-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="76176-105">Obtenha a contagem de usuários ativos diários no período de relatório por produto.</span><span class="sxs-lookup"><span data-stu-id="76176-105">Get the count of daily active users in the reporting period by product.</span></span>

> <span data-ttu-id="76176-106">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Usuários ativos](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="76176-106">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="76176-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="76176-107">Permissions</span></span>

<span data-ttu-id="76176-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76176-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="76176-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="76176-110">Permission type</span></span>                        | <span data-ttu-id="76176-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="76176-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="76176-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="76176-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="76176-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="76176-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="76176-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="76176-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="76176-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="76176-115">Not supported.</span></span>                           |
| <span data-ttu-id="76176-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="76176-116">Application</span></span>                            | <span data-ttu-id="76176-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="76176-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="76176-118">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="76176-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="76176-119">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="76176-119">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="76176-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="76176-120">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActiveUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="76176-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="76176-121">Function parameters</span></span>

<span data-ttu-id="76176-122">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="76176-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="76176-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="76176-123">Parameter</span></span> | <span data-ttu-id="76176-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="76176-124">Type</span></span>   | <span data-ttu-id="76176-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="76176-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="76176-126">ponto</span><span class="sxs-lookup"><span data-stu-id="76176-126">period</span></span>    | <span data-ttu-id="76176-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="76176-127">string</span></span> | <span data-ttu-id="76176-128">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="76176-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="76176-129">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="76176-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="76176-130">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="76176-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="76176-131">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="76176-131">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="76176-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="76176-132">Request headers</span></span>

| <span data-ttu-id="76176-133">Nome</span><span class="sxs-lookup"><span data-stu-id="76176-133">Name</span></span>          | <span data-ttu-id="76176-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="76176-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="76176-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="76176-135">Authorization</span></span> | <span data-ttu-id="76176-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="76176-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="76176-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="76176-138">Response</span></span>

<span data-ttu-id="76176-139">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="76176-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="76176-140">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="76176-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="76176-141">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="76176-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="76176-142">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="76176-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="76176-143">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="76176-143">Report Refresh Date</span></span>
- <span data-ttu-id="76176-144">Office 365</span><span class="sxs-lookup"><span data-stu-id="76176-144">Office 365</span></span>
- <span data-ttu-id="76176-145">Exchange</span><span class="sxs-lookup"><span data-stu-id="76176-145">Exchange</span></span>
- <span data-ttu-id="76176-146">OneDrive</span><span class="sxs-lookup"><span data-stu-id="76176-146">OneDrive</span></span>
- <span data-ttu-id="76176-147">SharePoint</span><span class="sxs-lookup"><span data-stu-id="76176-147">SharePoint</span></span>
- <span data-ttu-id="76176-148">Skype for Business</span><span class="sxs-lookup"><span data-stu-id="76176-148">Skype For Business</span></span> 
- <span data-ttu-id="76176-149">Yammer</span><span class="sxs-lookup"><span data-stu-id="76176-149">Yammer</span></span>
- <span data-ttu-id="76176-150">Teams</span><span class="sxs-lookup"><span data-stu-id="76176-150">Teams</span></span>
- <span data-ttu-id="76176-151">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="76176-151">Report Date</span></span>
- <span data-ttu-id="76176-152">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="76176-152">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="76176-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="76176-153">Example</span></span>

#### <a name="request"></a><span data-ttu-id="76176-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="76176-154">Request</span></span>

<span data-ttu-id="76176-155">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="76176-155">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getoffice365activeusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActiveUserCounts(period='D7')
```


#### <a name="response"></a><span data-ttu-id="76176-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="76176-156">Response</span></span>

<span data-ttu-id="76176-157">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="76176-157">The following is an example of the response.</span></span>

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

<span data-ttu-id="76176-158">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="76176-158">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Office 365,Exchange,OneDrive,SharePoint,Skype For Business,Yammer,Teams,Report Date,Report Period
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
