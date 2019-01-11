---
title: 'reportRoot: getSkypeForBusinessParticipantActivityUserCounts'
description: Obtenha tendências de uso do número de usuários únicos e o tipo de sessões de conferência das quais os usuários de sua organização participaram. Tipos de sessões de conferência incluem mensagens instantâneas, áudio/vídeo, compartilhamento de aplicativos, web e dial-in/out por terceiros.
localization_priority: Normal
ms.openlocfilehash: 5bc447e6cd4ea6845f60a01645d28b2745bb6fb5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867568"
---
# <a name="reportroot-getskypeforbusinessparticipantactivityusercounts"></a><span data-ttu-id="8baa1-104">reportRoot: getSkypeForBusinessParticipantActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="8baa1-104">reportRoot: getSkypeForBusinessParticipantActivityUserCounts</span></span>

> <span data-ttu-id="8baa1-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8baa1-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8baa1-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8baa1-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8baa1-107">Obtenha tendências de uso do número de usuários únicos e o tipo de sessões de conferência das quais os usuários de sua organização participaram.</span><span class="sxs-lookup"><span data-stu-id="8baa1-107">Get usage trends on the number of unique users and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="8baa1-108">Tipos de sessões de conferência incluem mensagens instantâneas, áudio/vídeo, compartilhamento de aplicativos, web e dial-in/out por terceiros.</span><span class="sxs-lookup"><span data-stu-id="8baa1-108">Types of conference sessions include IM, audio/video, application sharing, web, and dial-in/out - 3rd party.</span></span>

> <span data-ttu-id="8baa1-109">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Atividade do participante da conferência do Skype for Business](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span><span class="sxs-lookup"><span data-stu-id="8baa1-109">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference participant activity](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span></span>

## <a name="permissions"></a><span data-ttu-id="8baa1-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="8baa1-110">Permissions</span></span>

<span data-ttu-id="8baa1-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8baa1-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8baa1-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8baa1-113">Permission type</span></span>                        | <span data-ttu-id="8baa1-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8baa1-114">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="8baa1-115">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8baa1-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="8baa1-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8baa1-116">Reports.Read.All</span></span>                         |
| <span data-ttu-id="8baa1-117">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8baa1-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8baa1-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8baa1-118">Not supported.</span></span>                           |
| <span data-ttu-id="8baa1-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8baa1-119">Application</span></span>                            | <span data-ttu-id="8baa1-120">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8baa1-120">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="8baa1-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8baa1-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessParticipantActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="8baa1-122">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="8baa1-122">Function parameters</span></span>

<span data-ttu-id="8baa1-123">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="8baa1-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="8baa1-124">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="8baa1-124">Parameter</span></span> | <span data-ttu-id="8baa1-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="8baa1-125">Type</span></span>   | <span data-ttu-id="8baa1-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="8baa1-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="8baa1-127">ponto</span><span class="sxs-lookup"><span data-stu-id="8baa1-127">period</span></span>    | <span data-ttu-id="8baa1-128">string</span><span class="sxs-lookup"><span data-stu-id="8baa1-128">string</span></span> | <span data-ttu-id="8baa1-129">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="8baa1-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="8baa1-130">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="8baa1-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="8baa1-131">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="8baa1-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="8baa1-132">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8baa1-132">Required.</span></span> |

<span data-ttu-id="8baa1-133">Este método oferece suporte a `$format` [parâmetro de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8baa1-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="8baa1-134">O tipo de saída padrão é texto/csv.</span><span class="sxs-lookup"><span data-stu-id="8baa1-134">The default output type is text/csv.</span></span> <span data-ttu-id="8baa1-135">No entanto, se você deseja especificar o tipo de saída, você pode usar o parâmetro de consulta OData $format definido como texto/csv ou aplicativo/json.</span><span class="sxs-lookup"><span data-stu-id="8baa1-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8baa1-136">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8baa1-136">Request headers</span></span>

| <span data-ttu-id="8baa1-137">Nome</span><span class="sxs-lookup"><span data-stu-id="8baa1-137">Name</span></span>          | <span data-ttu-id="8baa1-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="8baa1-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="8baa1-139">Autorização</span><span class="sxs-lookup"><span data-stu-id="8baa1-139">Authorization</span></span> | <span data-ttu-id="8baa1-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8baa1-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="8baa1-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="8baa1-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="8baa1-143">CSV</span><span class="sxs-lookup"><span data-stu-id="8baa1-143">CSV</span></span>

<span data-ttu-id="8baa1-144">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="8baa1-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="8baa1-145">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="8baa1-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="8baa1-146">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="8baa1-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="8baa1-147">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="8baa1-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="8baa1-148">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="8baa1-148">Report Refresh Date</span></span>
- <span data-ttu-id="8baa1-149">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="8baa1-149">Report Date</span></span>
- <span data-ttu-id="8baa1-150">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="8baa1-150">Report Period</span></span>
- <span data-ttu-id="8baa1-151">Mensagens instantâneas</span><span class="sxs-lookup"><span data-stu-id="8baa1-151">IM</span></span>
- <span data-ttu-id="8baa1-152">Áudio/vídeo</span><span class="sxs-lookup"><span data-stu-id="8baa1-152">Audio/Video</span></span>
- <span data-ttu-id="8baa1-153">Compartilhamento de aplicativos</span><span class="sxs-lookup"><span data-stu-id="8baa1-153">App Sharing</span></span>
- <span data-ttu-id="8baa1-154">Web</span><span class="sxs-lookup"><span data-stu-id="8baa1-154">Web</span></span>
- <span data-ttu-id="8baa1-155">Dial-in/out por terceiros</span><span class="sxs-lookup"><span data-stu-id="8baa1-155">Dial-in/out 3rd Party</span></span>

### <a name="json"></a><span data-ttu-id="8baa1-156">JSON</span><span class="sxs-lookup"><span data-stu-id="8baa1-156">JSON</span></span>

<span data-ttu-id="8baa1-157">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto **[skypeForBusinessParticipantActivityUserCounts](../resources/skypeforbusinessparticipantactivityusercounts.md)** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8baa1-157">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessParticipantActivityUserCounts](../resources/skypeforbusinessparticipantactivityusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8baa1-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8baa1-158">Example</span></span>

### <a name="csv"></a><span data-ttu-id="8baa1-159">CSV</span><span class="sxs-lookup"><span data-stu-id="8baa1-159">CSV</span></span>

<span data-ttu-id="8baa1-160">O exemplo a seguir é um exemplo que emite CSV.</span><span class="sxs-lookup"><span data-stu-id="8baa1-160">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="8baa1-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8baa1-161">Request</span></span>

<span data-ttu-id="8baa1-162">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8baa1-162">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessparticipantactivityusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessParticipantActivityUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="8baa1-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="8baa1-163">Response</span></span>

<span data-ttu-id="8baa1-164">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8baa1-164">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="8baa1-165">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="8baa1-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="8baa1-166">JSON</span><span class="sxs-lookup"><span data-stu-id="8baa1-166">JSON</span></span>

<span data-ttu-id="8baa1-167">O exemplo a seguir é um exemplo que retorne JSON.</span><span class="sxs-lookup"><span data-stu-id="8baa1-167">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="8baa1-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8baa1-168">Request</span></span>

<span data-ttu-id="8baa1-169">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8baa1-169">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessparticipantactivityusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessParticipantActivityUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="8baa1-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="8baa1-170">Response</span></span>

<span data-ttu-id="8baa1-171">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8baa1-171">The following is an example of the response.</span></span>

> <span data-ttu-id="8baa1-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8baa1-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
