---
title: Listar trabalhos para um printerShare
description: Recupere uma lista de trabalhos de impressão associados ao compartilhamento de impressão.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: e573dda53c127e7b1b697b56dbadcfdfeca038d8
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48704874"
---
# <a name="list-printjobs-for-a-printershare"></a><span data-ttu-id="3c39d-103">Listar trabalhos para um printerShare</span><span class="sxs-lookup"><span data-stu-id="3c39d-103">List printJobs for a printerShare</span></span>

<span data-ttu-id="3c39d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c39d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c39d-105">Recupere uma lista de trabalhos de impressão associados ao [printerShare](../resources/printershare.md).</span><span class="sxs-lookup"><span data-stu-id="3c39d-105">Retrieve a list of print jobs associated with the [printerShare](../resources/printershare.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3c39d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3c39d-106">Permissions</span></span>
<span data-ttu-id="3c39d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c39d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="3c39d-109">Para usar o serviço de impressão universal, o usuário ou o locatário do aplicativo deve ter uma assinatura de impressão universal ativa, uma permissão que conceda [Get printerShare](printershare-get.md) Access e uma das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="3c39d-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, a permission that grants [Get printerShare](printershare-get.md) access, and one of the permissions listed in the following table.</span></span> <span data-ttu-id="3c39d-110">O usuário conectado deve ser um [administrador da impressora](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span><span class="sxs-lookup"><span data-stu-id="3c39d-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

<span data-ttu-id="3c39d-111">Para ler os trabalhos de impressão de outro usuário, o usuário conectado precisa ser um administrador de impressão e ter a permissão PrintJob. ReadBasic. All, PrintJob. Read. All, PrintJob. ReadWriteBasic. All ou PrintJob. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="3c39d-111">To read print jobs from another user, the signed in user needs to be a print administrator and have the PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All, or PrintJob.ReadWrite.All permission.</span></span>

|<span data-ttu-id="3c39d-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3c39d-112">Permission type</span></span> | <span data-ttu-id="3c39d-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3c39d-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="3c39d-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3c39d-114">Delegated (work or school account)</span></span>| <span data-ttu-id="3c39d-115">PrintJob. ReadBasic, PrintJob. Read, PrintJob. ReadBasic. All, PrintJob. Read. All, PrintJob. ReadWriteBasic, PrintJob. ReadWrite, PrintJob. ReadWriteBasic. All, PrintJob. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="3c39d-115">PrintJob.ReadBasic, PrintJob.Read, PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="3c39d-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3c39d-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c39d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3c39d-117">Not Supported.</span></span>|
|<span data-ttu-id="3c39d-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3c39d-118">Application</span></span>| <span data-ttu-id="3c39d-119">PrintJob. ReadBasic. All, PrintJob. Read. All, PrintJob. ReadWriteBasic. All, PrintJob. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="3c39d-119">PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3c39d-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3c39d-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/shares/{id}/jobs
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3c39d-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3c39d-121">Optional query parameters</span></span>
<span data-ttu-id="3c39d-122">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3c39d-122">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="3c39d-123">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="3c39d-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

* <span data-ttu-id="3c39d-124">A propriedade **Documents** é omitida da resposta por padrão.</span><span class="sxs-lookup"><span data-stu-id="3c39d-124">The **documents** property is omitted from the response by default.</span></span> <span data-ttu-id="3c39d-125">Para retornar também uma lista de [documentos](../resources/printdocument.md) impressos para cada trabalho de impressão, use `$expand=documents` .</span><span class="sxs-lookup"><span data-stu-id="3c39d-125">To also return a list of [printDocuments](../resources/printdocument.md) for each print job, use `$expand=documents`.</span></span>
* <span data-ttu-id="3c39d-126">Este método dá suporte à filtragem de trabalhos de impressão pelo usuário que os criou.</span><span class="sxs-lookup"><span data-stu-id="3c39d-126">This method supports filtering print jobs by the user who created them.</span></span> <span data-ttu-id="3c39d-127">Use `$filter=createdBy/userPrincipalName eq '{upn}'` , em que **{UPN}** é o [nome principal](/azure/active-directory/hybrid/plan-connect-userprincipalname#what-is-userprincipalname) do usuário associado.</span><span class="sxs-lookup"><span data-stu-id="3c39d-127">Use `$filter=createdBy/userPrincipalName eq '{upn}'`, where **{upn}** is the [user principal name](/azure/active-directory/hybrid/plan-connect-userprincipalname#what-is-userprincipalname) of the associated user.</span></span>

### <a name="exceptions"></a><span data-ttu-id="3c39d-128">Exceptions</span><span class="sxs-lookup"><span data-stu-id="3c39d-128">Exceptions</span></span>
<span data-ttu-id="3c39d-129">Não há suporte para alguns operadores: `$count` , `$search` , `$filter` .</span><span class="sxs-lookup"><span data-stu-id="3c39d-129">Some operators are not supported: `$count`, `$search`, `$filter`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3c39d-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3c39d-130">Request headers</span></span>
| <span data-ttu-id="3c39d-131">Nome</span><span class="sxs-lookup"><span data-stu-id="3c39d-131">Name</span></span>      |<span data-ttu-id="3c39d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c39d-132">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3c39d-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="3c39d-133">Authorization</span></span> | <span data-ttu-id="3c39d-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3c39d-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3c39d-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3c39d-136">Request body</span></span>
<span data-ttu-id="3c39d-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3c39d-137">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="3c39d-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c39d-138">Response</span></span>
<span data-ttu-id="3c39d-139">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [printJob](../resources/printjob.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3c39d-139">If successful, this method returns a `200 OK` response code and collection of [printJob](../resources/printjob.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3c39d-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3c39d-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="3c39d-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3c39d-141">Request</span></span>
<span data-ttu-id="3c39d-142">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3c39d-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3c39d-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="3c39d-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_jobs"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/shares/{id}/jobs
```
---

### <a name="response"></a><span data-ttu-id="3c39d-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c39d-144">Response</span></span>
<span data-ttu-id="3c39d-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3c39d-145">The following is an example of the response.</span></span>
><span data-ttu-id="3c39d-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3c39d-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
