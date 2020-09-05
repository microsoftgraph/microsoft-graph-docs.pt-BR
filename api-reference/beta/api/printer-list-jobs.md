---
title: Listar trabalhos
description: Recupere uma lista de trabalhos de impressão associados à impressora.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: d442f39a0327c511a105b420fd57b775c6f06853
ms.sourcegitcommit: 0a979eb1f21ec7834d24c268c24383c3139577ef
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/05/2020
ms.locfileid: "47400403"
---
# <a name="list-printjobs"></a><span data-ttu-id="71f71-103">Listar trabalhos</span><span class="sxs-lookup"><span data-stu-id="71f71-103">List printJobs</span></span>

<span data-ttu-id="71f71-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71f71-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71f71-105">Recupere uma lista de trabalhos de impressão associados à [impressora](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="71f71-105">Retrieve a list of print jobs associated with the [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="71f71-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="71f71-106">Permissions</span></span>
<span data-ttu-id="71f71-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71f71-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="71f71-109">Para usar o serviço de impressão universal, o usuário ou o locatário do aplicativo deve ter uma assinatura universal de impressão ativa, uma permissão que conceda obter acesso à [impressora](printer-get.md) e uma das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="71f71-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, a permission that grants [Get printer](printer-get.md) access, and one of the permissions listed in the following table.</span></span> <span data-ttu-id="71f71-110">O usuário conectado deve ser um [administrador da impressora](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span><span class="sxs-lookup"><span data-stu-id="71f71-110">The signed in user must be a [Printer Administrator](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

<span data-ttu-id="71f71-111">Para ler os trabalhos de impressão de outro usuário, o usuário conectado precisa ser um administrador de impressão e ter a permissão PrintJob. ReadBasic. All, PrintJob. Read. All, PrintJob. ReadWriteBasic. All ou PrintJob. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="71f71-111">To read print jobs from another user, the signed in user needs to be a print administrator and have the PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All, or PrintJob.ReadWrite.All permission.</span></span>

|<span data-ttu-id="71f71-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="71f71-112">Permission type</span></span> | <span data-ttu-id="71f71-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="71f71-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="71f71-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="71f71-114">Delegated (work or school account)</span></span>| <span data-ttu-id="71f71-115">PrintJob. ReadBasic, PrintJob. Read, PrintJob. ReadBasic. All, PrintJob. Read. All, PrintJob. ReadWriteBasic, PrintJob. ReadWrite, PrintJob. ReadWriteBasic. All, PrintJob. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="71f71-115">PrintJob.ReadBasic, PrintJob.Read, PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="71f71-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="71f71-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71f71-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="71f71-117">Not Supported.</span></span>|
|<span data-ttu-id="71f71-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="71f71-118">Application</span></span>| <span data-ttu-id="71f71-119">PrintJob. ReadBasic. All, PrintJob. Read. All, PrintJob. ReadWriteBasic. All, PrintJob. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="71f71-119">PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="71f71-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="71f71-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}/jobs
```

## <a name="optional-query-parameters"></a><span data-ttu-id="71f71-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="71f71-121">Optional query parameters</span></span>
<span data-ttu-id="71f71-122">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="71f71-122">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="71f71-123">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="71f71-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

* <span data-ttu-id="71f71-124">A propriedade **Documents** é omitida da resposta por padrão.</span><span class="sxs-lookup"><span data-stu-id="71f71-124">The **documents** property is omitted from the response by default.</span></span> <span data-ttu-id="71f71-125">Para retornar também uma lista de [documentos](../resources/printdocument.md) impressos para cada trabalho de impressão, use `$expand=documents` .</span><span class="sxs-lookup"><span data-stu-id="71f71-125">To also return a list of [printDocuments](../resources/printdocument.md) for each print job, use `$expand=documents`.</span></span>
* <span data-ttu-id="71f71-126">Este método dá suporte à filtragem de trabalhos de impressão pelo usuário que os criou.</span><span class="sxs-lookup"><span data-stu-id="71f71-126">This method supports filtering print jobs by the user who created them.</span></span> <span data-ttu-id="71f71-127">Use `$filter=createdBy/userPrincipalName eq '{upn}'` , em que **{UPN}** é o [nome principal](https://docs.microsoft.com/azure/active-directory/hybrid/plan-connect-userprincipalname#what-is-userprincipalname) do usuário associado.</span><span class="sxs-lookup"><span data-stu-id="71f71-127">Use `$filter=createdBy/userPrincipalName eq '{upn}'`, where **{upn}** is the [user principal name](https://docs.microsoft.com/azure/active-directory/hybrid/plan-connect-userprincipalname#what-is-userprincipalname) of the associated user.</span></span>

### <a name="exceptions"></a><span data-ttu-id="71f71-128">Exceptions</span><span class="sxs-lookup"><span data-stu-id="71f71-128">Exceptions</span></span>
<span data-ttu-id="71f71-129">Não há suporte para alguns operadores: `$count` , `$search` , `$filter` .</span><span class="sxs-lookup"><span data-stu-id="71f71-129">Some operators are not supported: `$count`, `$search`, `$filter`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="71f71-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="71f71-130">Request headers</span></span>
| <span data-ttu-id="71f71-131">Nome</span><span class="sxs-lookup"><span data-stu-id="71f71-131">Name</span></span>      |<span data-ttu-id="71f71-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="71f71-132">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="71f71-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="71f71-133">Authorization</span></span> | <span data-ttu-id="71f71-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="71f71-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="71f71-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="71f71-136">Request body</span></span>
<span data-ttu-id="71f71-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="71f71-137">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="71f71-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="71f71-138">Response</span></span>
<span data-ttu-id="71f71-139">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [printJob](../resources/printjob.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="71f71-139">If successful, this method returns a `200 OK` response code and collection of [printJob](../resources/printjob.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="71f71-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="71f71-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="71f71-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="71f71-141">Request</span></span>
<span data-ttu-id="71f71-142">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="71f71-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="71f71-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="71f71-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_jobs"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/{id}/jobs
```
# <a name="c"></a>[<span data-ttu-id="71f71-144">C#</span><span class="sxs-lookup"><span data-stu-id="71f71-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-jobs-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="71f71-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="71f71-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-jobs-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="71f71-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="71f71-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-jobs-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="71f71-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="71f71-147">Response</span></span>
<span data-ttu-id="71f71-148">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="71f71-148">The following is an example of the response.</span></span>
><span data-ttu-id="71f71-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="71f71-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
