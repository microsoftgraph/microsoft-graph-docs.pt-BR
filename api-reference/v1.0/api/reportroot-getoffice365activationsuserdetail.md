---
title: 'reportRoot: getOffice365ActivationsUserDetail'
description: Obter detalhes sobre os usuários que ativaram o Microsoft 365.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 83a59693898f85dd910e4f87765427fda4c10f90
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981778"
---
# <a name="reportroot-getoffice365activationsuserdetail"></a><span data-ttu-id="8b78b-103">reportRoot: getOffice365ActivationsUserDetail</span><span class="sxs-lookup"><span data-stu-id="8b78b-103">reportRoot: getOffice365ActivationsUserDetail</span></span>

<span data-ttu-id="8b78b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b78b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8b78b-105">Obter detalhes sobre os usuários que ativaram o Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="8b78b-105">Get details about users who have activated Microsoft 365.</span></span>

> <span data-ttu-id="8b78b-106">**Observação:** Para obter detalhes sobre diferentes visualizações e nomes de relatórios, consulte [relatórios do Microsoft 365 - ativações do Microsoft Office.](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)</span><span class="sxs-lookup"><span data-stu-id="8b78b-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="8b78b-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="8b78b-107">Permissions</span></span>

<span data-ttu-id="8b78b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b78b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8b78b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8b78b-110">Permission type</span></span>                        | <span data-ttu-id="8b78b-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8b78b-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="8b78b-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8b78b-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="8b78b-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b78b-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="8b78b-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8b78b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b78b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8b78b-115">Not supported.</span></span>                           |
| <span data-ttu-id="8b78b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8b78b-116">Application</span></span>                            | <span data-ttu-id="8b78b-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b78b-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="8b78b-118">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="8b78b-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="8b78b-119">Para saber mais, confira [Autorização para APIs lerem os relatórios de uso do Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="8b78b-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="8b78b-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8b78b-120">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserDetail
```

## <a name="request-headers"></a><span data-ttu-id="8b78b-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8b78b-121">Request headers</span></span>

| <span data-ttu-id="8b78b-122">Nome</span><span class="sxs-lookup"><span data-stu-id="8b78b-122">Name</span></span>          | <span data-ttu-id="8b78b-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="8b78b-123">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="8b78b-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="8b78b-124">Authorization</span></span> | <span data-ttu-id="8b78b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8b78b-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="8b78b-127">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="8b78b-127">If-None-Match</span></span> | <span data-ttu-id="8b78b-128">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="8b78b-128">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="8b78b-129">Opcional.</span><span class="sxs-lookup"><span data-stu-id="8b78b-129">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="8b78b-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="8b78b-130">Response</span></span>

<span data-ttu-id="8b78b-131">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="8b78b-131">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="8b78b-132">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="8b78b-132">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="8b78b-133">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="8b78b-133">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="8b78b-134">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="8b78b-134">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="8b78b-135">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="8b78b-135">Report Refresh Date</span></span>
- <span data-ttu-id="8b78b-136">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="8b78b-136">User Principal Name</span></span>
- <span data-ttu-id="8b78b-137">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="8b78b-137">Display Name</span></span>
- <span data-ttu-id="8b78b-138">Tipo de produto</span><span class="sxs-lookup"><span data-stu-id="8b78b-138">Product Type</span></span>
- <span data-ttu-id="8b78b-139">Data da última ativação</span><span class="sxs-lookup"><span data-stu-id="8b78b-139">Last Activated Date</span></span>
- <span data-ttu-id="8b78b-140">Windows</span><span class="sxs-lookup"><span data-stu-id="8b78b-140">Windows</span></span>
- <span data-ttu-id="8b78b-141">Mac</span><span class="sxs-lookup"><span data-stu-id="8b78b-141">Mac</span></span>
- <span data-ttu-id="8b78b-142">Windows 10 Mobile</span><span class="sxs-lookup"><span data-stu-id="8b78b-142">Windows 10 Mobile</span></span>
- <span data-ttu-id="8b78b-143">iOS</span><span class="sxs-lookup"><span data-stu-id="8b78b-143">iOS</span></span>
- <span data-ttu-id="8b78b-144">Android</span><span class="sxs-lookup"><span data-stu-id="8b78b-144">Android</span></span>
- <span data-ttu-id="8b78b-145">Ativado em um computador compartilhado</span><span class="sxs-lookup"><span data-stu-id="8b78b-145">Activated On Shared Computer</span></span>

## <a name="example"></a><span data-ttu-id="8b78b-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8b78b-146">Example</span></span>

#### <a name="request"></a><span data-ttu-id="8b78b-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8b78b-147">Request</span></span>

<span data-ttu-id="8b78b-148">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8b78b-148">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getoffice365activationsuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActivationsUserDetail
```


#### <a name="response"></a><span data-ttu-id="8b78b-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="8b78b-149">Response</span></span>

<span data-ttu-id="8b78b-150">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8b78b-150">The following is an example of the response.</span></span>

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

<span data-ttu-id="8b78b-151">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="8b78b-151">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Product Type,Last Activated Date,Windows,Mac,Windows 10 Mobile,iOS,Android,Activated On Shared Computer
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

