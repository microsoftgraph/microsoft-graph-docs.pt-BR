---
title: 'reportRoot: getYammerDeviceUsageUserCounts'
description: Obtenha o número de usuários diários por tipo de dispositivo.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 3ebb94df6d4474868917afeaee5a5ab92b236d10
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896011"
---
# <a name="reportroot-getyammerdeviceusageusercounts"></a><span data-ttu-id="59578-103">reportRoot: getYammerDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="59578-103">reportRoot: getYammerDeviceUsageUserCounts</span></span>

<span data-ttu-id="59578-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59578-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="59578-105">Obtenha o número de usuários diários por tipo de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="59578-105">Get the number of daily users by device type.</span></span>

> <span data-ttu-id="59578-106">**Observação:** Para obter detalhes sobre diferentes modos de exibição e nomes de relatórios, consulte [Microsoft 365 Reports-uso do dispositivo do Yammer](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span><span class="sxs-lookup"><span data-stu-id="59578-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="59578-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="59578-107">Permissions</span></span>

<span data-ttu-id="59578-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59578-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="59578-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="59578-110">Permission type</span></span>                        | <span data-ttu-id="59578-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="59578-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="59578-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="59578-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="59578-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="59578-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="59578-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="59578-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59578-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="59578-115">Not supported.</span></span>                           |
| <span data-ttu-id="59578-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="59578-116">Application</span></span>                            | <span data-ttu-id="59578-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="59578-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="59578-118">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="59578-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="59578-119">Para obter mais detalhes, consulte [Authorization for APIs to read Microsoft 365 Usage Reports](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="59578-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="59578-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="59578-120">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="59578-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="59578-121">Function parameters</span></span>

<span data-ttu-id="59578-122">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="59578-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="59578-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="59578-123">Parameter</span></span> | <span data-ttu-id="59578-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="59578-124">Type</span></span>   | <span data-ttu-id="59578-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="59578-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="59578-126">ponto</span><span class="sxs-lookup"><span data-stu-id="59578-126">period</span></span>    | <span data-ttu-id="59578-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59578-127">string</span></span> | <span data-ttu-id="59578-128">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="59578-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="59578-129">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="59578-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="59578-130">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="59578-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="59578-131">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59578-131">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="59578-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="59578-132">Request headers</span></span>

| <span data-ttu-id="59578-133">Nome</span><span class="sxs-lookup"><span data-stu-id="59578-133">Name</span></span>          | <span data-ttu-id="59578-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="59578-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="59578-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="59578-135">Authorization</span></span> | <span data-ttu-id="59578-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59578-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="59578-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="59578-138">If-None-Match</span></span> | <span data-ttu-id="59578-139">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="59578-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="59578-140">Opcional.</span><span class="sxs-lookup"><span data-stu-id="59578-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="59578-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="59578-141">Response</span></span>

<span data-ttu-id="59578-142">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="59578-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="59578-143">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="59578-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="59578-144">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="59578-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="59578-145">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="59578-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="59578-146">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="59578-146">Report Refresh Date</span></span>
- <span data-ttu-id="59578-147">Web</span><span class="sxs-lookup"><span data-stu-id="59578-147">Web</span></span>
- <span data-ttu-id="59578-148">Windows Phone</span><span class="sxs-lookup"><span data-stu-id="59578-148">Windows Phone</span></span>
- <span data-ttu-id="59578-149">Telefone Android</span><span class="sxs-lookup"><span data-stu-id="59578-149">Android Phone</span></span>
- <span data-ttu-id="59578-150">iPhone</span><span class="sxs-lookup"><span data-stu-id="59578-150">iPhone</span></span>
- <span data-ttu-id="59578-151">iPad</span><span class="sxs-lookup"><span data-stu-id="59578-151">iPad</span></span>
- <span data-ttu-id="59578-152">Outro</span><span class="sxs-lookup"><span data-stu-id="59578-152">Other</span></span>
- <span data-ttu-id="59578-153">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="59578-153">Report Date</span></span>
- <span data-ttu-id="59578-154">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="59578-154">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="59578-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="59578-155">Example</span></span>

#### <a name="request"></a><span data-ttu-id="59578-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="59578-156">Request</span></span>

<span data-ttu-id="59578-157">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="59578-157">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getyammerdeviceusageusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getYammerDeviceUsageUserCounts(period='D7')
```


#### <a name="response"></a><span data-ttu-id="59578-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="59578-158">Response</span></span>

<span data-ttu-id="59578-159">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="59578-159">The following is an example of the response.</span></span>

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

<span data-ttu-id="59578-160">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="59578-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iPhone,iPad,Other,Report Date,Report Period
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
