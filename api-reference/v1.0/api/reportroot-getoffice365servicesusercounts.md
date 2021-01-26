---
title: 'reportRoot: getOffice365ServicesUserCounts'
description: Obtenha a contagem de usuários por tipo de atividade e serviço.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 45ba2e17024a4635f5d0eb8d3b01050bbf5f6867
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49983479"
---
# <a name="reportroot-getoffice365servicesusercounts"></a><span data-ttu-id="f0ccf-103">reportRoot: getOffice365ServicesUserCounts</span><span class="sxs-lookup"><span data-stu-id="f0ccf-103">reportRoot: getOffice365ServicesUserCounts</span></span>

<span data-ttu-id="f0ccf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0ccf-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f0ccf-105">Obtenha a contagem de usuários por tipo de atividade e serviço.</span><span class="sxs-lookup"><span data-stu-id="f0ccf-105">Get the count of users by activity type and service.</span></span>

> <span data-ttu-id="f0ccf-106">**Observação:** Para saber mais sobre os diferentes modos de exibição de relatório e nomes, confira [Relatórios do Microsoft 365 - Usuários Ativos](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d). </span><span class="sxs-lookup"><span data-stu-id="f0ccf-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="f0ccf-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f0ccf-107">Permissions</span></span>

<span data-ttu-id="f0ccf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0ccf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f0ccf-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f0ccf-110">Permission type</span></span>                        | <span data-ttu-id="f0ccf-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f0ccf-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="f0ccf-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f0ccf-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="f0ccf-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f0ccf-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="f0ccf-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f0ccf-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0ccf-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f0ccf-115">Not supported.</span></span>                           |
| <span data-ttu-id="f0ccf-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f0ccf-116">Application</span></span>                            | <span data-ttu-id="f0ccf-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f0ccf-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="f0ccf-118">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="f0ccf-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="f0ccf-119">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="f0ccf-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="f0ccf-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f0ccf-120">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ServicesUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="f0ccf-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="f0ccf-121">Function parameters</span></span>

<span data-ttu-id="f0ccf-122">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="f0ccf-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="f0ccf-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f0ccf-123">Parameter</span></span> | <span data-ttu-id="f0ccf-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="f0ccf-124">Type</span></span>   | <span data-ttu-id="f0ccf-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0ccf-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="f0ccf-126">ponto</span><span class="sxs-lookup"><span data-stu-id="f0ccf-126">period</span></span>    | <span data-ttu-id="f0ccf-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f0ccf-127">string</span></span> | <span data-ttu-id="f0ccf-128">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="f0ccf-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="f0ccf-129">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="f0ccf-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="f0ccf-130">Eles seguem o formato D *n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="f0ccf-130">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="f0ccf-131">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f0ccf-131">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="f0ccf-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f0ccf-132">Request headers</span></span>

| <span data-ttu-id="f0ccf-133">Nome</span><span class="sxs-lookup"><span data-stu-id="f0ccf-133">Name</span></span>          | <span data-ttu-id="f0ccf-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0ccf-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="f0ccf-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="f0ccf-135">Authorization</span></span> | <span data-ttu-id="f0ccf-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f0ccf-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="f0ccf-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="f0ccf-138">If-None-Match</span></span> | <span data-ttu-id="f0ccf-139">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="f0ccf-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="f0ccf-140">Opcional.</span><span class="sxs-lookup"><span data-stu-id="f0ccf-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="f0ccf-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0ccf-141">Response</span></span>

<span data-ttu-id="f0ccf-142">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="f0ccf-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="f0ccf-143">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="f0ccf-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="f0ccf-144">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="f0ccf-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="f0ccf-145">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="f0ccf-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="f0ccf-146">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="f0ccf-146">Report Refresh Date</span></span>
- <span data-ttu-id="f0ccf-147">Exchange ativo</span><span class="sxs-lookup"><span data-stu-id="f0ccf-147">Exchange Active</span></span>
- <span data-ttu-id="f0ccf-148">Exchange inativo</span><span class="sxs-lookup"><span data-stu-id="f0ccf-148">Exchange Inactive</span></span>
- <span data-ttu-id="f0ccf-149">OneDrive ativo</span><span class="sxs-lookup"><span data-stu-id="f0ccf-149">OneDrive Active</span></span>
- <span data-ttu-id="f0ccf-150">OneDrive inativo</span><span class="sxs-lookup"><span data-stu-id="f0ccf-150">OneDrive Inactive</span></span>
- <span data-ttu-id="f0ccf-151">SharePoint ativo</span><span class="sxs-lookup"><span data-stu-id="f0ccf-151">SharePoint Active</span></span>
- <span data-ttu-id="f0ccf-152">SharePoint inativo</span><span class="sxs-lookup"><span data-stu-id="f0ccf-152">SharePoint Inactive</span></span>
- <span data-ttu-id="f0ccf-153">Skype for Business ativo</span><span class="sxs-lookup"><span data-stu-id="f0ccf-153">Skype For Business Active</span></span>
- <span data-ttu-id="f0ccf-154">Skype for Business inativo</span><span class="sxs-lookup"><span data-stu-id="f0ccf-154">Skype For Business Inactive</span></span>
- <span data-ttu-id="f0ccf-155">Yammer ativa</span><span class="sxs-lookup"><span data-stu-id="f0ccf-155">Yammer Active</span></span>
- <span data-ttu-id="f0ccf-156">Yammer inativa</span><span class="sxs-lookup"><span data-stu-id="f0ccf-156">Yammer Inactive</span></span>
- <span data-ttu-id="f0ccf-157">Teams ativo</span><span class="sxs-lookup"><span data-stu-id="f0ccf-157">Teams Active</span></span>
- <span data-ttu-id="f0ccf-158">Teams inativo</span><span class="sxs-lookup"><span data-stu-id="f0ccf-158">Teams Inactive</span></span>
- <span data-ttu-id="f0ccf-159">Office 365 Ativo</span><span class="sxs-lookup"><span data-stu-id="f0ccf-159">Office 365 Active</span></span>
- <span data-ttu-id="f0ccf-160">Office 365 Inativo</span><span class="sxs-lookup"><span data-stu-id="f0ccf-160">Office 365 Inactive</span></span>
- <span data-ttu-id="f0ccf-161">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="f0ccf-161">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="f0ccf-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f0ccf-162">Example</span></span>

#### <a name="request"></a><span data-ttu-id="f0ccf-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f0ccf-163">Request</span></span>

<span data-ttu-id="f0ccf-164">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f0ccf-164">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getoffice365servicesusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getOffice365ServicesUserCounts(period='D7')
```


#### <a name="response"></a><span data-ttu-id="f0ccf-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0ccf-165">Response</span></span>

<span data-ttu-id="f0ccf-166">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f0ccf-166">The following is an example of the response.</span></span>

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

<span data-ttu-id="f0ccf-167">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="f0ccf-167">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Exchange Active,Exchange Inactive,OneDrive Active,OneDrive Inactive,SharePoint Active,SharePoint Inactive,Skype For Business Active,Skype For Business Inactive,Yammer Active,Yammer Inactive,Teams Active,Teams Inactive,Office 365 Active,Office 365 Inactive,Report Period
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

