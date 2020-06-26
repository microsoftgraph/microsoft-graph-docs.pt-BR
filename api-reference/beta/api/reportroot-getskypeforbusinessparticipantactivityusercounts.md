---
title: 'reportRoot: getSkypeForBusinessParticipantActivityUserCounts'
description: Obtenha tendências de uso do número de usuários únicos e o tipo de sessões de conferência das quais os usuários de sua organização participaram. Tipos de sessões de conferência incluem mensagens instantâneas, áudio/vídeo, compartilhamento de aplicativos, web e dial-in/out por terceiros.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: a268cf551bcf89678e9489d7286bad196871993f
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896648"
---
# <a name="reportroot-getskypeforbusinessparticipantactivityusercounts"></a><span data-ttu-id="a9d76-104">reportRoot: getSkypeForBusinessParticipantActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="a9d76-104">reportRoot: getSkypeForBusinessParticipantActivityUserCounts</span></span>

<span data-ttu-id="a9d76-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9d76-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9d76-106">Obtenha tendências de uso do número de usuários únicos e o tipo de sessões de conferência das quais os usuários de sua organização participaram.</span><span class="sxs-lookup"><span data-stu-id="a9d76-106">Get usage trends on the number of unique users and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="a9d76-107">Tipos de sessões de conferência incluem mensagens instantâneas, áudio/vídeo, compartilhamento de aplicativos, web e dial-in/out por terceiros.</span><span class="sxs-lookup"><span data-stu-id="a9d76-107">Types of conference sessions include IM, audio/video, application sharing, web, and dial-in/out - 3rd party.</span></span>

> <span data-ttu-id="a9d76-108">**Observação:** Para obter detalhes sobre diferentes modos de exibição e nomes de relatórios, consulte [Microsoft 365 Reports-Skype for Business Conference participante Activity](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span><span class="sxs-lookup"><span data-stu-id="a9d76-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Skype for Business conference participant activity](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span></span>

## <a name="permissions"></a><span data-ttu-id="a9d76-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="a9d76-109">Permissions</span></span>

<span data-ttu-id="a9d76-110">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="a9d76-110">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="a9d76-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9d76-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a9d76-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a9d76-112">Permission type</span></span>                        | <span data-ttu-id="a9d76-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a9d76-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="a9d76-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a9d76-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="a9d76-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a9d76-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="a9d76-116">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a9d76-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a9d76-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a9d76-117">Not supported.</span></span>                           |
| <span data-ttu-id="a9d76-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a9d76-118">Application</span></span>                            | <span data-ttu-id="a9d76-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a9d76-119">Reports.Read.All</span></span>                         |

<span data-ttu-id="a9d76-120">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="a9d76-120">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="a9d76-121">Para obter mais detalhes, consulte [Authorization for APIs to read Microsoft 365 Usage Reports](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="a9d76-121">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="a9d76-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a9d76-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessParticipantActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="a9d76-123">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="a9d76-123">Function parameters</span></span>

<span data-ttu-id="a9d76-124">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="a9d76-124">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="a9d76-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="a9d76-125">Parameter</span></span> | <span data-ttu-id="a9d76-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="a9d76-126">Type</span></span>   | <span data-ttu-id="a9d76-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9d76-127">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="a9d76-128">ponto</span><span class="sxs-lookup"><span data-stu-id="a9d76-128">period</span></span>    | <span data-ttu-id="a9d76-129">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a9d76-129">string</span></span> | <span data-ttu-id="a9d76-130">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="a9d76-130">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="a9d76-131">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="a9d76-131">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="a9d76-132">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="a9d76-132">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="a9d76-133">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a9d76-133">Required.</span></span> |

<span data-ttu-id="a9d76-134">Esse método dá suporte ao`$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a9d76-134">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="a9d76-135">O tipo de saída padrão é text/csv.</span><span class="sxs-lookup"><span data-stu-id="a9d76-135">The default output type is text/csv.</span></span> <span data-ttu-id="a9d76-136">No entanto, se você quiser especificar o tipo de saída, poderá usar o parâmetro de consulta OData $format definido como text/csv ou Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="a9d76-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a9d76-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a9d76-137">Request headers</span></span>

| <span data-ttu-id="a9d76-138">Nome</span><span class="sxs-lookup"><span data-stu-id="a9d76-138">Name</span></span>          | <span data-ttu-id="a9d76-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9d76-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="a9d76-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="a9d76-140">Authorization</span></span> | <span data-ttu-id="a9d76-141">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="a9d76-141">Bearer {token}.</span></span> <span data-ttu-id="a9d76-142">Required.</span><span class="sxs-lookup"><span data-stu-id="a9d76-142">Required.</span></span> |

## <a name="response"></a><span data-ttu-id="a9d76-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9d76-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="a9d76-144">CSV</span><span class="sxs-lookup"><span data-stu-id="a9d76-144">CSV</span></span>

<span data-ttu-id="a9d76-145">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="a9d76-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="a9d76-146">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="a9d76-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="a9d76-147">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="a9d76-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="a9d76-148">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="a9d76-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="a9d76-149">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="a9d76-149">Report Refresh Date</span></span>
- <span data-ttu-id="a9d76-150">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="a9d76-150">Report Date</span></span>
- <span data-ttu-id="a9d76-151">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="a9d76-151">Report Period</span></span>
- <span data-ttu-id="a9d76-152">Mensagens instantâneas</span><span class="sxs-lookup"><span data-stu-id="a9d76-152">IM</span></span>
- <span data-ttu-id="a9d76-153">Áudio/vídeo</span><span class="sxs-lookup"><span data-stu-id="a9d76-153">Audio/Video</span></span>
- <span data-ttu-id="a9d76-154">Compartilhamento de aplicativos</span><span class="sxs-lookup"><span data-stu-id="a9d76-154">App Sharing</span></span>
- <span data-ttu-id="a9d76-155">Web</span><span class="sxs-lookup"><span data-stu-id="a9d76-155">Web</span></span>
- <span data-ttu-id="a9d76-156">Dial-in/out por terceiros</span><span class="sxs-lookup"><span data-stu-id="a9d76-156">Dial-in/out 3rd Party</span></span>

### <a name="json"></a><span data-ttu-id="a9d76-157">JSON</span><span class="sxs-lookup"><span data-stu-id="a9d76-157">JSON</span></span>

<span data-ttu-id="a9d76-158">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **[skypeForBusinessParticipantActivityUserCounts](../resources/skypeforbusinessparticipantactivityusercounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a9d76-158">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessParticipantActivityUserCounts](../resources/skypeforbusinessparticipantactivityusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9d76-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a9d76-159">Example</span></span>

### <a name="csv"></a><span data-ttu-id="a9d76-160">CSV</span><span class="sxs-lookup"><span data-stu-id="a9d76-160">CSV</span></span>

<span data-ttu-id="a9d76-161">Veja a seguir um exemplo que gera CSV.</span><span class="sxs-lookup"><span data-stu-id="a9d76-161">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="a9d76-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a9d76-162">Request</span></span>

<span data-ttu-id="a9d76-163">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a9d76-163">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getskypeforbusinessparticipantactivityusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessParticipantActivityUserCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="a9d76-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9d76-164">Response</span></span>

<span data-ttu-id="a9d76-165">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a9d76-165">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="a9d76-166">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="a9d76-166">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,IM,Audio/Video,App Sharing,Web,Dial-in/out 3rd Party
```

### <a name="json"></a><span data-ttu-id="a9d76-167">JSON</span><span class="sxs-lookup"><span data-stu-id="a9d76-167">JSON</span></span>

<span data-ttu-id="a9d76-168">Veja a seguir um exemplo que retorna JSON.</span><span class="sxs-lookup"><span data-stu-id="a9d76-168">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="a9d76-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a9d76-169">Request</span></span>

<span data-ttu-id="a9d76-170">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a9d76-170">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getskypeforbusinessparticipantactivityusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessParticipantActivityUserCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="a9d76-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9d76-171">Response</span></span>

<span data-ttu-id="a9d76-172">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a9d76-172">The following is an example of the response.</span></span>

> <span data-ttu-id="a9d76-173">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="a9d76-173">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a9d76-174">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="a9d76-174">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessParticipantActivityUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 301

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessParticipantActivityUserCounts)", 
  "value": [
    {
      "im": 137, 
      "audioVideo": 196, 
      "appSharing": 214, 
      "web": 30, 
      "dialInOut3rdParty": 2, 
      "reportRefreshDate": "2017-09-01", 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
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
