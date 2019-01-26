---
title: 'reportRoot: getOffice365ActivationsUserDetail'
description: Obtenha dados sobre usuários que ativaram o Office 365.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 3e5e6841e0c8f37cf9a054bcd5d7276e3b1fd04b
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571391"
---
# <a name="reportroot-getoffice365activationsuserdetail"></a><span data-ttu-id="796b3-103">reportRoot: getOffice365ActivationsUserDetail</span><span class="sxs-lookup"><span data-stu-id="796b3-103">reportRoot: getOffice365ActivationsUserDetail</span></span>

<span data-ttu-id="796b3-104">Obtenha dados sobre usuários que ativaram o Office 365.</span><span class="sxs-lookup"><span data-stu-id="796b3-104">Get details about users who have activated Office 365.</span></span>

> <span data-ttu-id="796b3-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Ativações do Microsoft Office](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="796b3-105">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="796b3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="796b3-106">Permissions</span></span>

<span data-ttu-id="796b3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="796b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="796b3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="796b3-109">Permission type</span></span>                        | <span data-ttu-id="796b3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="796b3-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="796b3-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="796b3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="796b3-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="796b3-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="796b3-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="796b3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="796b3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="796b3-114">Not supported.</span></span>                           |
| <span data-ttu-id="796b3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="796b3-115">Application</span></span>                            | <span data-ttu-id="796b3-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="796b3-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="796b3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="796b3-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserDetail
```

## <a name="request-headers"></a><span data-ttu-id="796b3-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="796b3-118">Request headers</span></span>

| <span data-ttu-id="796b3-119">Nome</span><span class="sxs-lookup"><span data-stu-id="796b3-119">Name</span></span>          | <span data-ttu-id="796b3-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="796b3-120">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="796b3-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="796b3-121">Authorization</span></span> | <span data-ttu-id="796b3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="796b3-p102">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="796b3-124">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="796b3-124">If-None-Match</span></span> | <span data-ttu-id="796b3-125">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="796b3-125">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="796b3-126">Opcional.</span><span class="sxs-lookup"><span data-stu-id="796b3-126">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="796b3-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="796b3-127">Response</span></span>

<span data-ttu-id="796b3-128">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="796b3-128">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="796b3-129">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="796b3-129">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="796b3-130">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="796b3-130">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="796b3-131">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="796b3-131">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="796b3-132">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="796b3-132">Report Refresh Date</span></span>
- <span data-ttu-id="796b3-133">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="796b3-133">User Principal Name</span></span>
- <span data-ttu-id="796b3-134">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="796b3-134">Display Name</span></span>
- <span data-ttu-id="796b3-135">Tipo de produto</span><span class="sxs-lookup"><span data-stu-id="796b3-135">Product Type</span></span>
- <span data-ttu-id="796b3-136">Data da última ativação</span><span class="sxs-lookup"><span data-stu-id="796b3-136">Last Activated Date</span></span>
- <span data-ttu-id="796b3-137">Windows</span><span class="sxs-lookup"><span data-stu-id="796b3-137">Windows</span></span>
- <span data-ttu-id="796b3-138">Mac</span><span class="sxs-lookup"><span data-stu-id="796b3-138">Mac</span></span>
- <span data-ttu-id="796b3-139">Windows 10 Mobile</span><span class="sxs-lookup"><span data-stu-id="796b3-139">Windows 10 Mobile</span></span>
- <span data-ttu-id="796b3-140">iOS</span><span class="sxs-lookup"><span data-stu-id="796b3-140">iOS</span></span>
- <span data-ttu-id="796b3-141">Android</span><span class="sxs-lookup"><span data-stu-id="796b3-141">Android</span></span>
- <span data-ttu-id="796b3-142">Ativado no computador compartilhado</span><span class="sxs-lookup"><span data-stu-id="796b3-142">Activated On Shared Computer</span></span>

## <a name="example"></a><span data-ttu-id="796b3-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="796b3-143">Example</span></span>

#### <a name="request"></a><span data-ttu-id="796b3-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="796b3-144">Request</span></span>

<span data-ttu-id="796b3-145">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="796b3-145">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activationsuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActivationsUserDetail
```

#### <a name="response"></a><span data-ttu-id="796b3-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="796b3-146">Response</span></span>

<span data-ttu-id="796b3-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="796b3-147">The following is an example of the response.</span></span>

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

<span data-ttu-id="796b3-148">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="796b3-148">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Product Type,Last Activated Date,Windows,Mac,Windows 10 Mobile,iOS,Android,Activated On Shared Computer
```
