---
title: Listar printJobs para uma impressora
description: Recupere uma lista de trabalhos de impressão associados à impressora.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: a1368cd07dd32f2c04e9a8bb41b04b5ce8d092cb
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049895"
---
# <a name="list-printjobs-for-a-printer"></a><span data-ttu-id="1bde7-103">Listar printJobs para uma impressora</span><span class="sxs-lookup"><span data-stu-id="1bde7-103">List printJobs for a printer</span></span>

<span data-ttu-id="1bde7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1bde7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1bde7-105">Recupere uma lista de trabalhos de impressão associados à [impressora](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="1bde7-105">Retrieve a list of print jobs associated with the [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1bde7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1bde7-106">Permissions</span></span>
<span data-ttu-id="1bde7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1bde7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="1bde7-109">Para usar o serviço Impressão Universal, o usuário ou locatário do aplicativo deve [](printer-get.md) ter uma assinatura de Impressão Universal ativa, uma permissão que concede acesso a Obter impressora e uma das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="1bde7-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, a permission that grants [Get printer](printer-get.md) access, and one of the permissions listed in the following table.</span></span> <span data-ttu-id="1bde7-110">O usuário inscreveu deve ser um [Administrador de Impressora.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="1bde7-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

<span data-ttu-id="1bde7-111">Para ler trabalhos de impressão de outro usuário, o usuário inscreveu precisa ser um administrador de impressão e ter a permissão PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All ou PrintJob.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="1bde7-111">To read print jobs from another user, the signed in user needs to be a print administrator and have the PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All, or PrintJob.ReadWrite.All permission.</span></span>

|<span data-ttu-id="1bde7-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1bde7-112">Permission type</span></span> | <span data-ttu-id="1bde7-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1bde7-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="1bde7-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1bde7-114">Delegated (work or school account)</span></span>| <span data-ttu-id="1bde7-115">PrintJob.ReadBasic, PrintJob.Read, PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1bde7-115">PrintJob.ReadBasic, PrintJob.Read, PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="1bde7-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1bde7-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1bde7-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1bde7-117">Not Supported.</span></span>|
|<span data-ttu-id="1bde7-118">Application</span><span class="sxs-lookup"><span data-stu-id="1bde7-118">Application</span></span>| <span data-ttu-id="1bde7-119">PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1bde7-119">PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1bde7-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1bde7-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}/jobs
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1bde7-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1bde7-121">Optional query parameters</span></span>
<span data-ttu-id="1bde7-122">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1bde7-122">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="1bde7-123">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="1bde7-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

* <span data-ttu-id="1bde7-124">A **propriedade documents** é omitida da resposta por padrão.</span><span class="sxs-lookup"><span data-stu-id="1bde7-124">The **documents** property is omitted from the response by default.</span></span> <span data-ttu-id="1bde7-125">Para também retornar uma lista de [printDocuments](../resources/printdocument.md) para cada trabalho de impressão, use `$expand=documents` .</span><span class="sxs-lookup"><span data-stu-id="1bde7-125">To also return a list of [printDocuments](../resources/printdocument.md) for each print job, use `$expand=documents`.</span></span>
* <span data-ttu-id="1bde7-126">Este método dá suporte à filtragem de trabalhos de impressão pelo usuário que os criou.</span><span class="sxs-lookup"><span data-stu-id="1bde7-126">This method supports filtering print jobs by the user who created them.</span></span> <span data-ttu-id="1bde7-127">Use `$filter=createdBy/userPrincipalName eq '{upn}'` , onde **{upn}** é [o nome principal do](/azure/active-directory/hybrid/plan-connect-userprincipalname#what-is-userprincipalname) usuário do usuário associado.</span><span class="sxs-lookup"><span data-stu-id="1bde7-127">Use `$filter=createdBy/userPrincipalName eq '{upn}'`, where **{upn}** is the [user principal name](/azure/active-directory/hybrid/plan-connect-userprincipalname#what-is-userprincipalname) of the associated user.</span></span>

### <a name="exceptions"></a><span data-ttu-id="1bde7-128">Exceções</span><span class="sxs-lookup"><span data-stu-id="1bde7-128">Exceptions</span></span>
<span data-ttu-id="1bde7-129">Alguns operadores não têm suporte: `$count` , `$search` .</span><span class="sxs-lookup"><span data-stu-id="1bde7-129">Some operators are not supported: `$count`, `$search`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1bde7-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1bde7-130">Request headers</span></span>
| <span data-ttu-id="1bde7-131">Nome</span><span class="sxs-lookup"><span data-stu-id="1bde7-131">Name</span></span>      |<span data-ttu-id="1bde7-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1bde7-132">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1bde7-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="1bde7-133">Authorization</span></span> | <span data-ttu-id="1bde7-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1bde7-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1bde7-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1bde7-136">Request body</span></span>
<span data-ttu-id="1bde7-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1bde7-137">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="1bde7-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="1bde7-138">Response</span></span>
<span data-ttu-id="1bde7-139">Se tiver êxito, este método retornará um código `200 OK` de resposta e uma coleção de objetos [printJob](../resources/printjob.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1bde7-139">If successful, this method returns a `200 OK` response code and collection of [printJob](../resources/printjob.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1bde7-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1bde7-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="1bde7-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1bde7-141">Request</span></span>
<span data-ttu-id="1bde7-142">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1bde7-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1bde7-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="1bde7-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_jobs_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/{id}/jobs
```
# <a name="c"></a>[<span data-ttu-id="1bde7-144">C#</span><span class="sxs-lookup"><span data-stu-id="1bde7-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-jobs-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1bde7-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1bde7-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-jobs-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1bde7-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1bde7-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-jobs-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1bde7-147">Java</span><span class="sxs-lookup"><span data-stu-id="1bde7-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-jobs-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="1bde7-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="1bde7-148">Response</span></span>
<span data-ttu-id="1bde7-149">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1bde7-149">The following is an example of the response.</span></span>
><span data-ttu-id="1bde7-150">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1bde7-150">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printers('c05f3726-0d4b-4aa1-8fe9-2eb981bb26fb')/jobs",
  "value": [
    {
      "id": "5182",
      "createdDateTime": "2020-02-04T00:00:00.0000000Z",
      "createdBy": {},
      "status": {
        "processingState": "completed",
        "processingStateDescription": "The print job has completed successfully and no further processing will take place."
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
