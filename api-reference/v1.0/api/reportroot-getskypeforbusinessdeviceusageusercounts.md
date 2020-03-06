---
title: 'reportRoot: getSkypeForBusinessDeviceUsageUserCounts'
description: Obtenha as tendências de uso de quantos usuários de sua organização conectaram usando o aplicativo Skype for Business. Você também obterá um detalhamento pelo tipo de dispositivo (Windows, Windows Phone, telefone Android, iPhone ou iPad) em que o aplicativo cliente Skype for Business está instalado e usado em toda a sua organização.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: e22d630e1634df2da2e3a95e54513af2f68160e8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42510155"
---
# <a name="reportroot-getskypeforbusinessdeviceusageusercounts"></a><span data-ttu-id="294bc-104">reportRoot: getSkypeForBusinessDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="294bc-104">reportRoot: getSkypeForBusinessDeviceUsageUserCounts</span></span>

<span data-ttu-id="294bc-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="294bc-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="294bc-106">Obtenha as tendências de uso de quantos usuários de sua organização conectaram usando o aplicativo Skype for Business.</span><span class="sxs-lookup"><span data-stu-id="294bc-106">Get the usage trends on how many users in your organization have connected using the Skype for Business app.</span></span> <span data-ttu-id="294bc-107">Você também obterá um detalhamento pelo tipo de dispositivo (Windows, Windows Phone, telefone Android, iPhone ou iPad) em que o aplicativo cliente Skype for Business está instalado e usado em toda a sua organização.</span><span class="sxs-lookup"><span data-stu-id="294bc-107">You will also get a breakdown by the type of device (Windows, Windows phone, Android phone, iPhone, or iPad) on which the Skype for Business client app is installed and used across your organization.</span></span>

> <span data-ttu-id="294bc-108">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Skype for Business usado pelos clientes](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span><span class="sxs-lookup"><span data-stu-id="294bc-108">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="294bc-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="294bc-109">Permissions</span></span>

<span data-ttu-id="294bc-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="294bc-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="294bc-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="294bc-112">Permission type</span></span>                        | <span data-ttu-id="294bc-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="294bc-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="294bc-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="294bc-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="294bc-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="294bc-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="294bc-116">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="294bc-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="294bc-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="294bc-117">Not supported.</span></span>                           |
| <span data-ttu-id="294bc-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="294bc-118">Application</span></span>                            | <span data-ttu-id="294bc-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="294bc-119">Reports.Read.All</span></span>                         |

<span data-ttu-id="294bc-120">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="294bc-120">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="294bc-121">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="294bc-121">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="294bc-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="294bc-122">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="294bc-123">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="294bc-123">Function parameters</span></span>

<span data-ttu-id="294bc-124">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="294bc-124">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="294bc-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="294bc-125">Parameter</span></span> | <span data-ttu-id="294bc-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="294bc-126">Type</span></span>   | <span data-ttu-id="294bc-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="294bc-127">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="294bc-128">ponto</span><span class="sxs-lookup"><span data-stu-id="294bc-128">period</span></span>    | <span data-ttu-id="294bc-129">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="294bc-129">string</span></span> | <span data-ttu-id="294bc-130">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="294bc-130">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="294bc-131">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="294bc-131">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="294bc-132">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="294bc-132">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="294bc-133">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="294bc-133">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="294bc-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="294bc-134">Request headers</span></span>

| <span data-ttu-id="294bc-135">Nome</span><span class="sxs-lookup"><span data-stu-id="294bc-135">Name</span></span>          | <span data-ttu-id="294bc-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="294bc-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="294bc-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="294bc-137">Authorization</span></span> | <span data-ttu-id="294bc-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="294bc-p106">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="294bc-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="294bc-140">If-None-Match</span></span> | <span data-ttu-id="294bc-141">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="294bc-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="294bc-142">Opcional.</span><span class="sxs-lookup"><span data-stu-id="294bc-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="294bc-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="294bc-143">Response</span></span>

<span data-ttu-id="294bc-144">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="294bc-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="294bc-145">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="294bc-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="294bc-146">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="294bc-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="294bc-147">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="294bc-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="294bc-148">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="294bc-148">Report Refresh Date</span></span>
- <span data-ttu-id="294bc-149">Windows</span><span class="sxs-lookup"><span data-stu-id="294bc-149">Windows</span></span>
- <span data-ttu-id="294bc-150">Windows Phone</span><span class="sxs-lookup"><span data-stu-id="294bc-150">Windows Phone</span></span>
- <span data-ttu-id="294bc-151">Telefone Android</span><span class="sxs-lookup"><span data-stu-id="294bc-151">Android Phone</span></span>
- <span data-ttu-id="294bc-152">iPhone</span><span class="sxs-lookup"><span data-stu-id="294bc-152">iPhone</span></span>
- <span data-ttu-id="294bc-153">iPad</span><span class="sxs-lookup"><span data-stu-id="294bc-153">iPad</span></span>
- <span data-ttu-id="294bc-154">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="294bc-154">Report Date</span></span>
- <span data-ttu-id="294bc-155">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="294bc-155">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="294bc-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="294bc-156">Example</span></span>

#### <a name="request"></a><span data-ttu-id="294bc-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="294bc-157">Request</span></span>

<span data-ttu-id="294bc-158">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="294bc-158">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="294bc-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="294bc-159">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessdeviceusageusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessDeviceUsageUserCounts(period='D7')
```
# <a name="c"></a>[<span data-ttu-id="294bc-160">C#</span><span class="sxs-lookup"><span data-stu-id="294bc-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessdeviceusageusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="294bc-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="294bc-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessdeviceusageusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="294bc-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="294bc-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessdeviceusageusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="294bc-163">Java</span><span class="sxs-lookup"><span data-stu-id="294bc-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinessdeviceusageusercounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="294bc-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="294bc-164">Response</span></span>

<span data-ttu-id="294bc-165">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="294bc-165">The following is an example of the response.</span></span>

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

<span data-ttu-id="294bc-166">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="294bc-166">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
