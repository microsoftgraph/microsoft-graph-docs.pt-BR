---
title: Listar printJobs para uma printerShare
description: Recupere uma lista de trabalhos de impressão associados ao compartilhamento de impressão.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: a7453677550e974536de20b6ad2b054d2040990e
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52037454"
---
# <a name="list-printjobs-for-a-printershare"></a><span data-ttu-id="8a624-103">Listar printJobs para uma printerShare</span><span class="sxs-lookup"><span data-stu-id="8a624-103">List printJobs for a printerShare</span></span>

<span data-ttu-id="8a624-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a624-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8a624-105">Recupere uma lista de trabalhos de impressão associados à [printerShare](../resources/printershare.md).</span><span class="sxs-lookup"><span data-stu-id="8a624-105">Retrieve a list of print jobs associated with the [printerShare](../resources/printershare.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8a624-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8a624-106">Permissions</span></span>
<span data-ttu-id="8a624-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a624-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="8a624-109">Para usar o serviço impressão universal, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa, uma permissão que concede acesso [Get printerShare](printershare-get.md) e uma das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="8a624-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, a permission that grants [Get printerShare](printershare-get.md) access, and one of the permissions listed in the following table.</span></span> 

<span data-ttu-id="8a624-110">Para ler trabalhos de impressão de outro usuário, o usuário inscreveu precisa ser um administrador de impressão e ter a permissão PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All ou PrintJob.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="8a624-110">To read print jobs from another user, the signed in user needs to be a print administrator and have the PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All, or PrintJob.ReadWrite.All permission.</span></span>

|<span data-ttu-id="8a624-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8a624-111">Permission type</span></span> | <span data-ttu-id="8a624-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8a624-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="8a624-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8a624-113">Delegated (work or school account)</span></span>| <span data-ttu-id="8a624-114">PrintJob.ReadBasic, PrintJob.Read, PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a624-114">PrintJob.ReadBasic, PrintJob.Read, PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="8a624-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8a624-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8a624-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8a624-116">Not Supported.</span></span>|
|<span data-ttu-id="8a624-117">Application</span><span class="sxs-lookup"><span data-stu-id="8a624-117">Application</span></span>| <span data-ttu-id="8a624-118">PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a624-118">PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8a624-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8a624-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/shares/{id}/jobs
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8a624-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8a624-120">Optional query parameters</span></span>
<span data-ttu-id="8a624-121">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8a624-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="8a624-122">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="8a624-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

* <span data-ttu-id="8a624-123">A **propriedade documents** é omitida da resposta por padrão.</span><span class="sxs-lookup"><span data-stu-id="8a624-123">The **documents** property is omitted from the response by default.</span></span> <span data-ttu-id="8a624-124">Para também retornar uma lista de [printDocuments](../resources/printdocument.md) para cada trabalho de impressão, use `$expand=documents` .</span><span class="sxs-lookup"><span data-stu-id="8a624-124">To also return a list of [printDocuments](../resources/printdocument.md) for each print job, use `$expand=documents`.</span></span>
* <span data-ttu-id="8a624-125">Este método dá suporte à filtragem de trabalhos de impressão pelo usuário que os criou.</span><span class="sxs-lookup"><span data-stu-id="8a624-125">This method supports filtering print jobs by the user who created them.</span></span> <span data-ttu-id="8a624-126">Use `$filter=createdBy/userPrincipalName eq '{upn}'` , onde **{upn}** é [o nome principal do](/azure/active-directory/hybrid/plan-connect-userprincipalname#what-is-userprincipalname) usuário do usuário associado.</span><span class="sxs-lookup"><span data-stu-id="8a624-126">Use `$filter=createdBy/userPrincipalName eq '{upn}'`, where **{upn}** is the [user principal name](/azure/active-directory/hybrid/plan-connect-userprincipalname#what-is-userprincipalname) of the associated user.</span></span>

### <a name="exceptions"></a><span data-ttu-id="8a624-127">Exceções</span><span class="sxs-lookup"><span data-stu-id="8a624-127">Exceptions</span></span>
<span data-ttu-id="8a624-128">Alguns operadores não têm suporte: `$count` , `$search` .</span><span class="sxs-lookup"><span data-stu-id="8a624-128">Some operators are not supported: `$count`, `$search`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8a624-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8a624-129">Request headers</span></span>
| <span data-ttu-id="8a624-130">Nome</span><span class="sxs-lookup"><span data-stu-id="8a624-130">Name</span></span>      |<span data-ttu-id="8a624-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="8a624-131">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8a624-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="8a624-132">Authorization</span></span> | <span data-ttu-id="8a624-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8a624-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8a624-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8a624-135">Request body</span></span>
<span data-ttu-id="8a624-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8a624-136">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="8a624-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a624-137">Response</span></span>
<span data-ttu-id="8a624-138">Se tiver êxito, este método retornará um código `200 OK` de resposta e uma coleção de objetos [printJob](../resources/printjob.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8a624-138">If successful, this method returns a `200 OK` response code and collection of [printJob](../resources/printjob.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8a624-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8a624-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="8a624-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8a624-140">Request</span></span>
<span data-ttu-id="8a624-141">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8a624-141">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8a624-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="8a624-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_jobs_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/shares/{id}/jobs
```
# <a name="c"></a>[<span data-ttu-id="8a624-143">C#</span><span class="sxs-lookup"><span data-stu-id="8a624-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-jobs-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8a624-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8a624-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-jobs-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8a624-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8a624-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-jobs-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8a624-146">Java</span><span class="sxs-lookup"><span data-stu-id="8a624-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-jobs-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---

### <a name="response"></a><span data-ttu-id="8a624-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a624-147">Response</span></span>
<span data-ttu-id="8a624-148">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8a624-148">The following is an example of the response.</span></span>
><span data-ttu-id="8a624-149">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8a624-149">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printJob",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 461

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/shares('f37141d9-0afb-484f-96d3-0ef0a679e6c1')/jobs",
  "value": [
    {
      "id": "103",
      "createdDateTime": "2020-02-04T00:00:00.0000000Z",
      "createdBy": {},
      "status": {
        "state": "completed",
        "description": "The print job has completed successfully and no further processing will take place.",
        "details" : [],
        "isAcquiredByPrinter": true
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List jobs",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
