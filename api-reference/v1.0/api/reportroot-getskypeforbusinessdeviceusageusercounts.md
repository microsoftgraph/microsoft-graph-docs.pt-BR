---
title: 'reportRoot: getSkypeForBusinessDeviceUsageUserCounts'
description: Obtenha as tendências de uso de quantos usuários de sua organização conectaram usando o aplicativo Skype for Business. Você também obterá um detalhamento pelo tipo de dispositivo (Windows, Windows Phone, telefone Android, iPhone ou iPad) em que o aplicativo cliente Skype for Business está instalado e usado em toda a sua organização.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 2e839553f9e84b07057d885727192261555b44b4
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981428"
---
# <a name="reportroot-getskypeforbusinessdeviceusageusercounts"></a><span data-ttu-id="dd60b-104">reportRoot: getSkypeForBusinessDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="dd60b-104">reportRoot: getSkypeForBusinessDeviceUsageUserCounts</span></span>

<span data-ttu-id="dd60b-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd60b-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dd60b-106">Obtenha as tendências de uso de quantos usuários de sua organização conectaram usando o aplicativo Skype for Business.</span><span class="sxs-lookup"><span data-stu-id="dd60b-106">Get the usage trends on how many users in your organization have connected using the Skype for Business app.</span></span> <span data-ttu-id="dd60b-107">Você também obterá um detalhamento pelo tipo de dispositivo (Windows, Windows Phone, telefone Android, iPhone ou iPad) em que o aplicativo cliente Skype for Business está instalado e usado em toda a sua organização.</span><span class="sxs-lookup"><span data-stu-id="dd60b-107">You will also get a breakdown by the type of device (Windows, Windows phone, Android phone, iPhone, or iPad) on which the Skype for Business client app is installed and used across your organization.</span></span>

> <span data-ttu-id="dd60b-108">**Observação:** Para obter detalhes sobre diferentes visualizações e nomes de relatórios, consulte relatórios do [Microsoft 365 - Clientes do Skype for Business usados.](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3)</span><span class="sxs-lookup"><span data-stu-id="dd60b-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="dd60b-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="dd60b-109">Permissions</span></span>

<span data-ttu-id="dd60b-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd60b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dd60b-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dd60b-112">Permission type</span></span>                        | <span data-ttu-id="dd60b-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dd60b-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="dd60b-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dd60b-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="dd60b-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="dd60b-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="dd60b-116">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dd60b-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd60b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dd60b-117">Not supported.</span></span>                           |
| <span data-ttu-id="dd60b-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dd60b-118">Application</span></span>                            | <span data-ttu-id="dd60b-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="dd60b-119">Reports.Read.All</span></span>                         |

<span data-ttu-id="dd60b-120">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="dd60b-120">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="dd60b-121">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="dd60b-121">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="dd60b-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dd60b-122">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="dd60b-123">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="dd60b-123">Function parameters</span></span>

<span data-ttu-id="dd60b-124">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="dd60b-124">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="dd60b-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="dd60b-125">Parameter</span></span> | <span data-ttu-id="dd60b-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="dd60b-126">Type</span></span>   | <span data-ttu-id="dd60b-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd60b-127">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="dd60b-128">ponto</span><span class="sxs-lookup"><span data-stu-id="dd60b-128">period</span></span>    | <span data-ttu-id="dd60b-129">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dd60b-129">string</span></span> | <span data-ttu-id="dd60b-130">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="dd60b-130">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="dd60b-131">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="dd60b-131">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="dd60b-132">Eles seguem o formato D *n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="dd60b-132">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="dd60b-133">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dd60b-133">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="dd60b-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dd60b-134">Request headers</span></span>

| <span data-ttu-id="dd60b-135">Nome</span><span class="sxs-lookup"><span data-stu-id="dd60b-135">Name</span></span>          | <span data-ttu-id="dd60b-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd60b-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="dd60b-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="dd60b-137">Authorization</span></span> | <span data-ttu-id="dd60b-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dd60b-p106">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="dd60b-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="dd60b-140">If-None-Match</span></span> | <span data-ttu-id="dd60b-141">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="dd60b-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="dd60b-142">Opcional.</span><span class="sxs-lookup"><span data-stu-id="dd60b-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="dd60b-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd60b-143">Response</span></span>

<span data-ttu-id="dd60b-144">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="dd60b-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="dd60b-145">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="dd60b-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="dd60b-146">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="dd60b-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="dd60b-147">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="dd60b-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="dd60b-148">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="dd60b-148">Report Refresh Date</span></span>
- <span data-ttu-id="dd60b-149">Windows</span><span class="sxs-lookup"><span data-stu-id="dd60b-149">Windows</span></span>
- <span data-ttu-id="dd60b-150">Windows Phone</span><span class="sxs-lookup"><span data-stu-id="dd60b-150">Windows Phone</span></span>
- <span data-ttu-id="dd60b-151">Telefone Android</span><span class="sxs-lookup"><span data-stu-id="dd60b-151">Android Phone</span></span>
- <span data-ttu-id="dd60b-152">iPhone</span><span class="sxs-lookup"><span data-stu-id="dd60b-152">iPhone</span></span>
- <span data-ttu-id="dd60b-153">iPad</span><span class="sxs-lookup"><span data-stu-id="dd60b-153">iPad</span></span>
- <span data-ttu-id="dd60b-154">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="dd60b-154">Report Date</span></span>
- <span data-ttu-id="dd60b-155">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="dd60b-155">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="dd60b-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dd60b-156">Example</span></span>

#### <a name="request"></a><span data-ttu-id="dd60b-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dd60b-157">Request</span></span>

<span data-ttu-id="dd60b-158">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="dd60b-158">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessdeviceusageusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessDeviceUsageUserCounts(period='D7')
```


#### <a name="response"></a><span data-ttu-id="dd60b-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd60b-159">Response</span></span>

<span data-ttu-id="dd60b-160">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="dd60b-160">The following is an example of the response.</span></span>

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

<span data-ttu-id="dd60b-161">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="dd60b-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Windows,Windows Phone,Android Phone,iPhone,iPad,Report Date,Report Period
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

