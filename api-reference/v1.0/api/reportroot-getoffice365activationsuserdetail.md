---
title: 'reportRoot: getOffice365ActivationsUserDetail'
description: Obtenha dados sobre usuários que ativaram o Office 365.
ms.openlocfilehash: cab151992f2e8ba148ab82c64e967b2514bd2222
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006098"
---
# <a name="reportroot-getoffice365activationsuserdetail"></a><span data-ttu-id="b2e2b-103">reportRoot: getOffice365ActivationsUserDetail</span><span class="sxs-lookup"><span data-stu-id="b2e2b-103">reportRoot: getOffice365ActivationsUserDetail</span></span>

<span data-ttu-id="b2e2b-104">Obtenha dados sobre usuários que ativaram o Office 365.</span><span class="sxs-lookup"><span data-stu-id="b2e2b-104">Get details about users who have activated Office 365.</span></span>

> <span data-ttu-id="b2e2b-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Ativações do Microsoft Office](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="b2e2b-105">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="b2e2b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b2e2b-106">Permissions</span></span>

<span data-ttu-id="b2e2b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2e2b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b2e2b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b2e2b-109">Permission type</span></span>                        | <span data-ttu-id="b2e2b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b2e2b-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="b2e2b-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b2e2b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b2e2b-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b2e2b-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="b2e2b-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b2e2b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b2e2b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b2e2b-114">Not supported.</span></span>                           |
| <span data-ttu-id="b2e2b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b2e2b-115">Application</span></span>                            | <span data-ttu-id="b2e2b-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b2e2b-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="b2e2b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b2e2b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserDetail
```

## <a name="request-headers"></a><span data-ttu-id="b2e2b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b2e2b-118">Request headers</span></span>

| <span data-ttu-id="b2e2b-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b2e2b-119">Name</span></span>          | <span data-ttu-id="b2e2b-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2e2b-120">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="b2e2b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b2e2b-121">Authorization</span></span> | <span data-ttu-id="b2e2b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b2e2b-p102">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="b2e2b-124">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="b2e2b-124">If-None-Match</span></span> | <span data-ttu-id="b2e2b-125">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="b2e2b-125">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="b2e2b-126">Opcional.</span><span class="sxs-lookup"><span data-stu-id="b2e2b-126">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="b2e2b-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2e2b-127">Response</span></span>

<span data-ttu-id="b2e2b-128">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="b2e2b-128">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="b2e2b-129">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="b2e2b-129">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="b2e2b-130">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="b2e2b-130">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="b2e2b-131">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="b2e2b-131">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="b2e2b-132">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="b2e2b-132">Report Refresh Date</span></span>
- <span data-ttu-id="b2e2b-133">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="b2e2b-133">User Principal Name</span></span>
- <span data-ttu-id="b2e2b-134">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="b2e2b-134">Display Name</span></span>
- <span data-ttu-id="b2e2b-135">Tipo de produto</span><span class="sxs-lookup"><span data-stu-id="b2e2b-135">Product Type</span></span>
- <span data-ttu-id="b2e2b-136">Data da última ativação</span><span class="sxs-lookup"><span data-stu-id="b2e2b-136">Last Activated Date</span></span>
- <span data-ttu-id="b2e2b-137">Windows</span><span class="sxs-lookup"><span data-stu-id="b2e2b-137">Windows</span></span>
- <span data-ttu-id="b2e2b-138">Mac</span><span class="sxs-lookup"><span data-stu-id="b2e2b-138">Mac</span></span>
- <span data-ttu-id="b2e2b-139">Windows 10 Mobile</span><span class="sxs-lookup"><span data-stu-id="b2e2b-139">Windows 10 Mobile</span></span>
- <span data-ttu-id="b2e2b-140">iOS</span><span class="sxs-lookup"><span data-stu-id="b2e2b-140">iOS</span></span>
- <span data-ttu-id="b2e2b-141">Android</span><span class="sxs-lookup"><span data-stu-id="b2e2b-141">Android</span></span>
- <span data-ttu-id="b2e2b-142">Ativado no computador compartilhado</span><span class="sxs-lookup"><span data-stu-id="b2e2b-142">Activated On Shared Computer</span></span>

## <a name="example"></a><span data-ttu-id="b2e2b-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b2e2b-143">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b2e2b-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b2e2b-144">Request</span></span>

<span data-ttu-id="b2e2b-145">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b2e2b-145">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activationsuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActivationsUserDetail
```

#### <a name="response"></a><span data-ttu-id="b2e2b-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2e2b-146">Response</span></span>

<span data-ttu-id="b2e2b-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b2e2b-147">The following is an example of the response.</span></span>

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

<span data-ttu-id="b2e2b-148">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="b2e2b-148">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Product Type,Last Activated Date,Windows,Mac,Windows 10 Mobile,iOS,Android,Activated On Shared Computer
```
