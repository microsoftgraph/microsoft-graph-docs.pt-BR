---
title: 'reportRoot: getOffice365ActivationsUserCounts'
description: Obtenha a contagem de usuários habilitados e aqueles que ativaram a assinatura do Office em desktops ou dispositivos ou computadores compartilhados.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 9a150911e9234cde7258acbeed7f825fb9db4c66
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582154"
---
# <a name="reportroot-getoffice365activationsusercounts"></a><span data-ttu-id="29fcb-103">reportRoot: getOffice365ActivationsUserCounts</span><span class="sxs-lookup"><span data-stu-id="29fcb-103">reportRoot: getOffice365ActivationsUserCounts</span></span>

<span data-ttu-id="29fcb-104">Obtenha a contagem de usuários habilitados e aqueles que ativaram a assinatura do Office em desktops ou dispositivos ou computadores compartilhados.</span><span class="sxs-lookup"><span data-stu-id="29fcb-104">Get the count of users that are enabled and those that have activated the Office subscription on desktop or devices or shared computers.</span></span>

> <span data-ttu-id="29fcb-105">**Observação:** para saber mais sobre diferentes visualizações e nomes de relatórios, confira [Relatórios do Office 365 Reports - Ativações do Microsoft Office](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="29fcb-105">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="29fcb-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="29fcb-106">Permissions</span></span>

<span data-ttu-id="29fcb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29fcb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="29fcb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="29fcb-109">Permission type</span></span>                        | <span data-ttu-id="29fcb-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="29fcb-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="29fcb-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="29fcb-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="29fcb-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="29fcb-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="29fcb-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="29fcb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29fcb-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="29fcb-114">Not supported.</span></span>                           |
| <span data-ttu-id="29fcb-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="29fcb-115">Application</span></span>                            | <span data-ttu-id="29fcb-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="29fcb-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="29fcb-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="29fcb-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserCounts
```

## <a name="request-headers"></a><span data-ttu-id="29fcb-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="29fcb-118">Request headers</span></span>

| <span data-ttu-id="29fcb-119">Nome</span><span class="sxs-lookup"><span data-stu-id="29fcb-119">Name</span></span>          | <span data-ttu-id="29fcb-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="29fcb-120">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="29fcb-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="29fcb-121">Authorization</span></span> | <span data-ttu-id="29fcb-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="29fcb-p102">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="29fcb-124">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="29fcb-124">If-None-Match</span></span> | <span data-ttu-id="29fcb-125">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="29fcb-125">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="29fcb-126">Opcional.</span><span class="sxs-lookup"><span data-stu-id="29fcb-126">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="29fcb-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="29fcb-127">Response</span></span>

<span data-ttu-id="29fcb-128">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="29fcb-128">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="29fcb-129">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="29fcb-129">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="29fcb-130">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="29fcb-130">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="29fcb-131">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="29fcb-131">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="29fcb-132">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="29fcb-132">Report Refresh Date</span></span>
- <span data-ttu-id="29fcb-133">Tipo de produto</span><span class="sxs-lookup"><span data-stu-id="29fcb-133">Product Type</span></span>
- <span data-ttu-id="29fcb-134">Atribuído</span><span class="sxs-lookup"><span data-stu-id="29fcb-134">Assigned</span></span>
- <span data-ttu-id="29fcb-135">Ativado</span><span class="sxs-lookup"><span data-stu-id="29fcb-135">Activated</span></span>
- <span data-ttu-id="29fcb-136">Ativação de computador compartilhado</span><span class="sxs-lookup"><span data-stu-id="29fcb-136">Shared Computer Activation</span></span>

## <a name="example"></a><span data-ttu-id="29fcb-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="29fcb-137">Example</span></span>

#### <a name="request"></a><span data-ttu-id="29fcb-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="29fcb-138">Request</span></span>

<span data-ttu-id="29fcb-139">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="29fcb-139">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activationsusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActivationsUserCounts
```

#### <a name="response"></a><span data-ttu-id="29fcb-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="29fcb-140">Response</span></span>

<span data-ttu-id="29fcb-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="29fcb-141">The following is an example of the response.</span></span>

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

<span data-ttu-id="29fcb-142">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="29fcb-142">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Product Type,Assigned,Activated,Shared Computer Activation
```
