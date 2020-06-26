---
title: 'reportRoot: getOffice365ActivationsUserDetail'
description: Obtenha detalhes sobre os usuários que ativaram o Microsoft 365.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: c009511c7001cb33321e25f853c11741c37fd6da
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897397"
---
# <a name="reportroot-getoffice365activationsuserdetail"></a><span data-ttu-id="3ca04-103">reportRoot: getOffice365ActivationsUserDetail</span><span class="sxs-lookup"><span data-stu-id="3ca04-103">reportRoot: getOffice365ActivationsUserDetail</span></span>

<span data-ttu-id="3ca04-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ca04-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3ca04-105">Obtenha detalhes sobre os usuários que ativaram o Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="3ca04-105">Get details about users who have activated Microsoft 365.</span></span>

> <span data-ttu-id="3ca04-106">**Observação:** Para obter detalhes sobre diferentes modos de exibição e nomes de relatórios, consulte [microsoft 365 Reports-Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="3ca04-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="3ca04-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="3ca04-107">Permissions</span></span>

<span data-ttu-id="3ca04-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="3ca04-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="3ca04-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ca04-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3ca04-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3ca04-110">Permission type</span></span>                        | <span data-ttu-id="3ca04-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3ca04-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="3ca04-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3ca04-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="3ca04-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ca04-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="3ca04-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3ca04-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ca04-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3ca04-115">Not supported.</span></span>                           |
| <span data-ttu-id="3ca04-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3ca04-116">Application</span></span>                            | <span data-ttu-id="3ca04-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ca04-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="3ca04-118">**Observação**: para permissões delegadas para permitir que os aplicativos leiam os relatórios de uso de serviço em nome de um usuário, o administrador de locatários deve atribuir a função apropriada de administrador limitada do Azure AD ao usuário.</span><span class="sxs-lookup"><span data-stu-id="3ca04-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="3ca04-119">Para obter mais detalhes, consulte [Authorization for APIs to read Microsoft 365 Usage Reports](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="3ca04-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="3ca04-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3ca04-120">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserDetail
```

## <a name="request-headers"></a><span data-ttu-id="3ca04-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3ca04-121">Request headers</span></span>

| <span data-ttu-id="3ca04-122">Nome</span><span class="sxs-lookup"><span data-stu-id="3ca04-122">Name</span></span>          | <span data-ttu-id="3ca04-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="3ca04-123">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="3ca04-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="3ca04-124">Authorization</span></span> | <span data-ttu-id="3ca04-125">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="3ca04-125">Bearer {token}.</span></span> <span data-ttu-id="3ca04-126">Required.</span><span class="sxs-lookup"><span data-stu-id="3ca04-126">Required.</span></span>                |
| <span data-ttu-id="3ca04-127">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="3ca04-127">If-None-Match</span></span> | <span data-ttu-id="3ca04-128">Se este cabeçalho de solicitação estiver incluso e a eTag fornecida corresponder à marca atual do arquivo, um código de resposta `304 Not Modified` será exibido.</span><span class="sxs-lookup"><span data-stu-id="3ca04-128">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="3ca04-129">Opcional.</span><span class="sxs-lookup"><span data-stu-id="3ca04-129">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="3ca04-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ca04-130">Response</span></span>

<span data-ttu-id="3ca04-131">Se for bem-sucedido, este método retorna uma resposta `302 Found` que redireciona para uma URL de download pré-autenticada para o relatório.</span><span class="sxs-lookup"><span data-stu-id="3ca04-131">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="3ca04-132">Essa URL pode ser encontrada no cabeçalho `Location` na resposta.</span><span class="sxs-lookup"><span data-stu-id="3ca04-132">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="3ca04-133">As URLs de download previamente autenticadas são válidas apenas por um curto período de tempo (alguns minutos) e não exigem um cabeçalho `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="3ca04-133">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="3ca04-134">O arquivo CSV possui os seguintes cabeçalhos para colunas.</span><span class="sxs-lookup"><span data-stu-id="3ca04-134">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="3ca04-135">Data de atualização do relatório</span><span class="sxs-lookup"><span data-stu-id="3ca04-135">Report Refresh Date</span></span>
- <span data-ttu-id="3ca04-136">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="3ca04-136">User Principal Name</span></span>
- <span data-ttu-id="3ca04-137">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="3ca04-137">Display Name</span></span>
- <span data-ttu-id="3ca04-138">Tipo de produto</span><span class="sxs-lookup"><span data-stu-id="3ca04-138">Product Type</span></span>
- <span data-ttu-id="3ca04-139">Data da última ativação</span><span class="sxs-lookup"><span data-stu-id="3ca04-139">Last Activated Date</span></span>
- <span data-ttu-id="3ca04-140">Windows</span><span class="sxs-lookup"><span data-stu-id="3ca04-140">Windows</span></span>
- <span data-ttu-id="3ca04-141">Mac</span><span class="sxs-lookup"><span data-stu-id="3ca04-141">Mac</span></span>
- <span data-ttu-id="3ca04-142">Windows 10 Mobile</span><span class="sxs-lookup"><span data-stu-id="3ca04-142">Windows 10 Mobile</span></span>
- <span data-ttu-id="3ca04-143">iOS</span><span class="sxs-lookup"><span data-stu-id="3ca04-143">iOS</span></span>
- <span data-ttu-id="3ca04-144">Android</span><span class="sxs-lookup"><span data-stu-id="3ca04-144">Android</span></span>
- <span data-ttu-id="3ca04-145">Ativado no computador compartilhado</span><span class="sxs-lookup"><span data-stu-id="3ca04-145">Activated On Shared Computer</span></span>

## <a name="example"></a><span data-ttu-id="3ca04-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3ca04-146">Example</span></span>

#### <a name="request"></a><span data-ttu-id="3ca04-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3ca04-147">Request</span></span>

<span data-ttu-id="3ca04-148">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3ca04-148">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getoffice365activationsuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActivationsUserDetail
```


#### <a name="response"></a><span data-ttu-id="3ca04-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ca04-149">Response</span></span>

<span data-ttu-id="3ca04-150">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3ca04-150">The following is an example of the response.</span></span>

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

<span data-ttu-id="3ca04-151">Siga o redirecionamento 302 e o arquivo CSV baixado terá o seguinte esquema.</span><span class="sxs-lookup"><span data-stu-id="3ca04-151">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
