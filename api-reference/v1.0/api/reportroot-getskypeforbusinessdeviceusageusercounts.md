---
title: 'reportRoot: getSkypeForBusinessDeviceUsageUserCounts'
description: Obtenha as tendências de uso de quantos usuários de sua organização conectaram usando o aplicativo Skype for Business. Você também obterá um detalhamento pelo tipo de dispositivo (Windows, Windows Phone, telefone Android, iPhone ou iPad) em que o aplicativo cliente Skype for Business está instalado e usado em toda a sua organização.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: eab4bccf576b5a6a7b69f32e8f3ca777b7c63575
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865304"
---
# <a name="reportroot-getskypeforbusinessdeviceusageusercounts"></a><span data-ttu-id="1d40b-104">reportRoot: getSkypeForBusinessDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="1d40b-104">reportRoot: getSkypeForBusinessDeviceUsageUserCounts</span></span>

<span data-ttu-id="1d40b-105">Obtenha as tendências de uso de quantos usuários de sua organização conectaram usando o aplicativo Skype for Business.</span><span class="sxs-lookup"><span data-stu-id="1d40b-105">Get the usage trends on how many users in your organization have connected using the Skype for Business app.</span></span> <span data-ttu-id="1d40b-106">Você também obterá um detalhamento pelo tipo de dispositivo (Windows, Windows Phone, telefone Android, iPhone ou iPad) em que o aplicativo cliente Skype for Business está instalado e usado em toda a sua organização.</span><span class="sxs-lookup"><span data-stu-id="1d40b-106">You will also get a breakdown by the type of device (Windows, Windows phone, Android phone, iPhone, or iPad) on which the Skype for Business client app is installed and used across your organization.</span></span>

> <span data-ttu-id="1d40b-107">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Skype for Business usado pelos clientes](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span><span class="sxs-lookup"><span data-stu-id="1d40b-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="1d40b-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="1d40b-108">Permissions</span></span>

<span data-ttu-id="1d40b-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d40b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1d40b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1d40b-111">Permission type</span></span>                        | <span data-ttu-id="1d40b-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1d40b-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="1d40b-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1d40b-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="1d40b-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1d40b-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="1d40b-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1d40b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d40b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1d40b-116">Not supported.</span></span>                           |
| <span data-ttu-id="1d40b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1d40b-117">Application</span></span>                            | <span data-ttu-id="1d40b-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1d40b-118">Reports.Read.All</span></span>                         |

<span data-ttu-id="1d40b-119">**Observação**: para permissões delegadas para permitir que os aplicativos leiam relatórios de uso do serviço em nome de um usuário, o administrador do locatário deve ter atribuído ao usuário a função de administrador limitada do Azure ad apropriada.</span><span class="sxs-lookup"><span data-stu-id="1d40b-119">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="1d40b-120">Para obter mais detalhes, consulte [Authorization for APIs to read Office 365 Usage Reports](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="1d40b-120">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="1d40b-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1d40b-121">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="1d40b-122">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="1d40b-122">Function parameters</span></span>

<span data-ttu-id="1d40b-123">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="1d40b-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="1d40b-124">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="1d40b-124">Parameter</span></span> | <span data-ttu-id="1d40b-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="1d40b-125">Type</span></span>   | <span data-ttu-id="1d40b-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d40b-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="1d40b-127">ponto</span><span class="sxs-lookup"><span data-stu-id="1d40b-127">period</span></span>    | <span data-ttu-id="1d40b-128">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1d40b-128">string</span></span> | <span data-ttu-id="1d40b-129">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="1d40b-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="1d40b-130">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="1d40b-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="1d40b-131">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="1d40b-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="1d40b-132">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1d40b-132">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="1d40b-133">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1d40b-133">Request headers</span></span>

| <span data-ttu-id="1d40b-134">Nome</span><span class="sxs-lookup"><span data-stu-id="1d40b-134">Name</span></span>          | <span data-ttu-id="1d40b-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d40b-135">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="1d40b-136">Autorização</span><span class="sxs-lookup"><span data-stu-id="1d40b-136">Authorization</span></span> | <span data-ttu-id="1d40b-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1d40b-p106">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="1d40b-139">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="1d40b-139">If-None-Match</span></span> | <span data-ttu-id="1d40b-140">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="1d40b-140">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="1d40b-141">Opcional.</span><span class="sxs-lookup"><span data-stu-id="1d40b-141">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="1d40b-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d40b-142">Response</span></span>

<span data-ttu-id="1d40b-143">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="1d40b-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="1d40b-144">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="1d40b-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="1d40b-145">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="1d40b-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="1d40b-146">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="1d40b-146">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="1d40b-147">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="1d40b-147">Report Refresh Date</span></span>
- <span data-ttu-id="1d40b-148">Windows</span><span class="sxs-lookup"><span data-stu-id="1d40b-148">Windows</span></span>
- <span data-ttu-id="1d40b-149">Windows Phone</span><span class="sxs-lookup"><span data-stu-id="1d40b-149">Windows Phone</span></span>
- <span data-ttu-id="1d40b-150">Telefone Android</span><span class="sxs-lookup"><span data-stu-id="1d40b-150">Android Phone</span></span>
- <span data-ttu-id="1d40b-151">iPhone</span><span class="sxs-lookup"><span data-stu-id="1d40b-151">iPhone</span></span>
- <span data-ttu-id="1d40b-152">iPad</span><span class="sxs-lookup"><span data-stu-id="1d40b-152">iPad</span></span>
- <span data-ttu-id="1d40b-153">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="1d40b-153">Report Date</span></span>
- <span data-ttu-id="1d40b-154">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="1d40b-154">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="1d40b-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1d40b-155">Example</span></span>

#### <a name="request"></a><span data-ttu-id="1d40b-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1d40b-156">Request</span></span>

<span data-ttu-id="1d40b-157">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1d40b-157">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="1d40b-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="1d40b-158">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessdeviceusageusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessDeviceUsageUserCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1d40b-159">C#</span><span class="sxs-lookup"><span data-stu-id="1d40b-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessdeviceusageusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1d40b-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1d40b-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessdeviceusageusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1d40b-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1d40b-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessdeviceusageusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1d40b-162">Java</span><span class="sxs-lookup"><span data-stu-id="1d40b-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinessdeviceusageusercounts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1d40b-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d40b-163">Response</span></span>

<span data-ttu-id="1d40b-164">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1d40b-164">The following is an example of the response.</span></span>

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

<span data-ttu-id="1d40b-165">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="1d40b-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
