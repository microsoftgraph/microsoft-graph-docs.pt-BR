---
title: 'reportRoot: getOffice365ActivationsUserCounts'
description: Obter a contagem de usuários que estão habilitados e aqueles que ativaram a assinatura do Office em computadores desktop ou dispositivos ou computadores compartilhados.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 07f3583aacdd246b0514d60d866d177765e6bd21
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49982058"
---
# <a name="reportroot-getoffice365activationsusercounts"></a><span data-ttu-id="e4e5a-103">reportRoot: getOffice365ActivationsUserCounts</span><span class="sxs-lookup"><span data-stu-id="e4e5a-103">reportRoot: getOffice365ActivationsUserCounts</span></span>

<span data-ttu-id="e4e5a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4e5a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e4e5a-105">Obter a contagem de usuários que estão habilitados e aqueles que ativaram a assinatura do Office em computadores desktop ou dispositivos ou computadores compartilhados.</span><span class="sxs-lookup"><span data-stu-id="e4e5a-105">Get the count of users that are enabled and those that have activated the Office subscription on desktop or devices or shared computers.</span></span>

> <span data-ttu-id="e4e5a-106">**Observação:** Para obter detalhes sobre diferentes visualizações e nomes de relatórios, consulte [relatórios do Microsoft 365 - ativações do Microsoft Office.](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)</span><span class="sxs-lookup"><span data-stu-id="e4e5a-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="e4e5a-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="e4e5a-107">Permissions</span></span>

<span data-ttu-id="e4e5a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4e5a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e4e5a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e4e5a-110">Permission type</span></span>                        | <span data-ttu-id="e4e5a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e4e5a-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="e4e5a-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e4e5a-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="e4e5a-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4e5a-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="e4e5a-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e4e5a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e4e5a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e4e5a-115">Not supported.</span></span>                           |
| <span data-ttu-id="e4e5a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e4e5a-116">Application</span></span>                            | <span data-ttu-id="e4e5a-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4e5a-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="e4e5a-118">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="e4e5a-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="e4e5a-119">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="e4e5a-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="e4e5a-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e4e5a-120">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserCounts
```

## <a name="request-headers"></a><span data-ttu-id="e4e5a-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e4e5a-121">Request headers</span></span>

| <span data-ttu-id="e4e5a-122">Nome</span><span class="sxs-lookup"><span data-stu-id="e4e5a-122">Name</span></span>          | <span data-ttu-id="e4e5a-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4e5a-123">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="e4e5a-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="e4e5a-124">Authorization</span></span> | <span data-ttu-id="e4e5a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e4e5a-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="e4e5a-127">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="e4e5a-127">If-None-Match</span></span> | <span data-ttu-id="e4e5a-128">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="e4e5a-128">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="e4e5a-129">Opcional.</span><span class="sxs-lookup"><span data-stu-id="e4e5a-129">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="e4e5a-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4e5a-130">Response</span></span>

<span data-ttu-id="e4e5a-131">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="e4e5a-131">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="e4e5a-132">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="e4e5a-132">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="e4e5a-133">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="e4e5a-133">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="e4e5a-134">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="e4e5a-134">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="e4e5a-135">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="e4e5a-135">Report Refresh Date</span></span>
- <span data-ttu-id="e4e5a-136">Tipo de produto</span><span class="sxs-lookup"><span data-stu-id="e4e5a-136">Product Type</span></span>
- <span data-ttu-id="e4e5a-137">Atribuído</span><span class="sxs-lookup"><span data-stu-id="e4e5a-137">Assigned</span></span>
- <span data-ttu-id="e4e5a-138">Ativado</span><span class="sxs-lookup"><span data-stu-id="e4e5a-138">Activated</span></span>
- <span data-ttu-id="e4e5a-139">Ativação de computador compartilhado</span><span class="sxs-lookup"><span data-stu-id="e4e5a-139">Shared Computer Activation</span></span>

## <a name="example"></a><span data-ttu-id="e4e5a-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e4e5a-140">Example</span></span>

#### <a name="request"></a><span data-ttu-id="e4e5a-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e4e5a-141">Request</span></span>

<span data-ttu-id="e4e5a-142">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e4e5a-142">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getoffice365activationsusercounts"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActivationsUserCounts
```


#### <a name="response"></a><span data-ttu-id="e4e5a-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4e5a-143">Response</span></span>

<span data-ttu-id="e4e5a-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e4e5a-144">The following is an example of the response.</span></span>

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

<span data-ttu-id="e4e5a-145">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="e4e5a-145">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Product Type,Assigned,Activated,Shared Computer Activation
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

