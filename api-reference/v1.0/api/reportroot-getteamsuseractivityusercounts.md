---
title: 'reportRoot: getTeamsUserActivityUserCounts'
description: Obtém o número de atividades do Microsoft Teams por tipo de atividade. Os tipos de atividade são o número de mensagens de chat de equipes, mensagens de chat privadas, chamadas ou reuniões.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: f3c57a19224ca2a04f435526c1ec846b3eed90a2
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44892440"
---
# <a name="reportroot-getteamsuseractivityusercounts"></a><span data-ttu-id="dc2e3-104">reportRoot: getTeamsUserActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="dc2e3-104">reportRoot: getTeamsUserActivityUserCounts</span></span>

<span data-ttu-id="dc2e3-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc2e3-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dc2e3-106">Obtém o número de atividades do Microsoft Teams por tipo de atividade.</span><span class="sxs-lookup"><span data-stu-id="dc2e3-106">Get the number of Microsoft Teams users by activity type.</span></span> <span data-ttu-id="dc2e3-107">Os tipos de atividade são o número de mensagens de chat de equipes, mensagens de chat privadas, chamadas ou reuniões.</span><span class="sxs-lookup"><span data-stu-id="dc2e3-107">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span>

## <a name="permissions"></a><span data-ttu-id="dc2e3-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="dc2e3-108">Permissions</span></span>

<span data-ttu-id="dc2e3-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="dc2e3-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="dc2e3-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc2e3-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dc2e3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dc2e3-111">Permission type</span></span>                        | <span data-ttu-id="dc2e3-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dc2e3-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="dc2e3-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dc2e3-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="dc2e3-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="dc2e3-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="dc2e3-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dc2e3-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dc2e3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dc2e3-116">Not supported.</span></span>                           |
| <span data-ttu-id="dc2e3-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dc2e3-117">Application</span></span>                            | <span data-ttu-id="dc2e3-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="dc2e3-118">Reports.Read.All</span></span>                         |

<span data-ttu-id="dc2e3-119">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="dc2e3-119">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="dc2e3-120">Para obter mais detalhes, consulte [Authorization for APIs to read Microsoft 365 Usage Reports](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="dc2e3-120">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="dc2e3-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dc2e3-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="dc2e3-122">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="dc2e3-122">Function parameters</span></span>

<span data-ttu-id="dc2e3-123">Na URL da solicitação, forneça um valor válido ao seguinte parâmetro.</span><span class="sxs-lookup"><span data-stu-id="dc2e3-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="dc2e3-124">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="dc2e3-124">Parameter</span></span> | <span data-ttu-id="dc2e3-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="dc2e3-125">Type</span></span>   | <span data-ttu-id="dc2e3-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc2e3-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="dc2e3-127">ponto</span><span class="sxs-lookup"><span data-stu-id="dc2e3-127">period</span></span>    | <span data-ttu-id="dc2e3-128">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dc2e3-128">string</span></span> | <span data-ttu-id="dc2e3-129">Especifica o período de tempo durante o qual o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="dc2e3-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="dc2e3-130">Os valores com suporte para {period_value} são: D7, D30, D90 e D180.</span><span class="sxs-lookup"><span data-stu-id="dc2e3-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="dc2e3-131">Eles seguem o formato D*n*, em que *n* representa o número de dias em que o relatório é agregado.</span><span class="sxs-lookup"><span data-stu-id="dc2e3-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="dc2e3-132">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dc2e3-132">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="dc2e3-133">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dc2e3-133">Request headers</span></span>

| <span data-ttu-id="dc2e3-134">Nome</span><span class="sxs-lookup"><span data-stu-id="dc2e3-134">Name</span></span>          | <span data-ttu-id="dc2e3-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc2e3-135">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="dc2e3-136">Autorização</span><span class="sxs-lookup"><span data-stu-id="dc2e3-136">Authorization</span></span> | <span data-ttu-id="dc2e3-137">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="dc2e3-137">Bearer {token}.</span></span> <span data-ttu-id="dc2e3-138">Required.</span><span class="sxs-lookup"><span data-stu-id="dc2e3-138">Required.</span></span> |

## <a name="response"></a><span data-ttu-id="dc2e3-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc2e3-139">Response</span></span>

<span data-ttu-id="dc2e3-140">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="dc2e3-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="dc2e3-141">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="dc2e3-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="dc2e3-142">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="dc2e3-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="dc2e3-143">O arquivo CSV possui os seguintes cabeçalhos para colunas:</span><span class="sxs-lookup"><span data-stu-id="dc2e3-143">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="dc2e3-144">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="dc2e3-144">Report Refresh Date</span></span>
- <span data-ttu-id="dc2e3-145">Data do relatório</span><span class="sxs-lookup"><span data-stu-id="dc2e3-145">Report Date</span></span>
- <span data-ttu-id="dc2e3-146">Mensagens de chat de equipes</span><span class="sxs-lookup"><span data-stu-id="dc2e3-146">Team Chat Messages</span></span>
- <span data-ttu-id="dc2e3-147">Mensagens de chat privadas</span><span class="sxs-lookup"><span data-stu-id="dc2e3-147">Private Chat Messages</span></span>
- <span data-ttu-id="dc2e3-148">Chamadas</span><span class="sxs-lookup"><span data-stu-id="dc2e3-148">Calls</span></span>
- <span data-ttu-id="dc2e3-149">Reuniões</span><span class="sxs-lookup"><span data-stu-id="dc2e3-149">Meetings</span></span>
- <span data-ttu-id="dc2e3-150">Outras Ações</span><span class="sxs-lookup"><span data-stu-id="dc2e3-150">Other Actions</span></span>
- <span data-ttu-id="dc2e3-151">Período de Relatório</span><span class="sxs-lookup"><span data-stu-id="dc2e3-151">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="dc2e3-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dc2e3-152">Example</span></span>

#### <a name="request"></a><span data-ttu-id="dc2e3-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dc2e3-153">Request</span></span>

<span data-ttu-id="dc2e3-154">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="dc2e3-154">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivityusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getTeamsUserActivityUserCounts(period='D7')
```


#### <a name="response"></a><span data-ttu-id="dc2e3-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc2e3-155">Response</span></span>

<span data-ttu-id="dc2e3-156">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="dc2e3-156">The following is an example of the response.</span></span>

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

<span data-ttu-id="dc2e3-157">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="dc2e3-157">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Team Chat Messages,Private Chat Messages,Calls,Meetings,Other Actions,Report Period
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
