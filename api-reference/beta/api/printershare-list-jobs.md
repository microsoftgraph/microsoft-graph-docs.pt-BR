---
title: Listar printJobs para uma printerShare
description: Recupere uma lista de trabalhos de impressão associados ao compartilhamento de impressão.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 7a2c7969a5900410eeb195025391c4b3b413ce26
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50950668"
---
# <a name="list-printjobs-for-a-printershare"></a><span data-ttu-id="fe890-103">Listar printJobs para uma printerShare</span><span class="sxs-lookup"><span data-stu-id="fe890-103">List printJobs for a printerShare</span></span>

<span data-ttu-id="fe890-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe890-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe890-105">Recupere uma lista de trabalhos de impressão associados à [printerShare](../resources/printershare.md).</span><span class="sxs-lookup"><span data-stu-id="fe890-105">Retrieve a list of print jobs associated with the [printerShare](../resources/printershare.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="fe890-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="fe890-106">Permissions</span></span>
<span data-ttu-id="fe890-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe890-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="fe890-109">Para usar o serviço impressão universal, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa, uma permissão que concede acesso [Get printerShare](printershare-get.md) e uma das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="fe890-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, a permission that grants [Get printerShare](printershare-get.md) access, and one of the permissions listed in the following table.</span></span> <span data-ttu-id="fe890-110">O usuário inscreveu deve ser um [Administrador de Impressora.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="fe890-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

<span data-ttu-id="fe890-111">Para ler trabalhos de impressão de outro usuário, o usuário inscreveu precisa ser um administrador de impressão e ter a permissão PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All ou PrintJob.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="fe890-111">To read print jobs from another user, the signed in user needs to be a print administrator and have the PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All, or PrintJob.ReadWrite.All permission.</span></span>

|<span data-ttu-id="fe890-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fe890-112">Permission type</span></span> | <span data-ttu-id="fe890-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fe890-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="fe890-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fe890-114">Delegated (work or school account)</span></span>| <span data-ttu-id="fe890-115">PrintJob.ReadBasic, PrintJob.Read, PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe890-115">PrintJob.ReadBasic, PrintJob.Read, PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="fe890-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fe890-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fe890-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fe890-117">Not Supported.</span></span>|
|<span data-ttu-id="fe890-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fe890-118">Application</span></span>| <span data-ttu-id="fe890-119">PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe890-119">PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fe890-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fe890-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/shares/{id}/jobs
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fe890-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fe890-121">Optional query parameters</span></span>
<span data-ttu-id="fe890-122">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fe890-122">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="fe890-123">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="fe890-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

* <span data-ttu-id="fe890-124">A **propriedade documents** é omitida da resposta por padrão.</span><span class="sxs-lookup"><span data-stu-id="fe890-124">The **documents** property is omitted from the response by default.</span></span> <span data-ttu-id="fe890-125">Para também retornar uma lista de [printDocuments](../resources/printdocument.md) para cada trabalho de impressão, use `$expand=documents` .</span><span class="sxs-lookup"><span data-stu-id="fe890-125">To also return a list of [printDocuments](../resources/printdocument.md) for each print job, use `$expand=documents`.</span></span>
* <span data-ttu-id="fe890-126">Este método dá suporte à filtragem de trabalhos de impressão pelo usuário que os criou.</span><span class="sxs-lookup"><span data-stu-id="fe890-126">This method supports filtering print jobs by the user who created them.</span></span> <span data-ttu-id="fe890-127">Use `$filter=createdBy/userPrincipalName eq '{upn}'` , onde **{upn}** é [o nome principal do](/azure/active-directory/hybrid/plan-connect-userprincipalname#what-is-userprincipalname) usuário do usuário associado.</span><span class="sxs-lookup"><span data-stu-id="fe890-127">Use `$filter=createdBy/userPrincipalName eq '{upn}'`, where **{upn}** is the [user principal name](/azure/active-directory/hybrid/plan-connect-userprincipalname#what-is-userprincipalname) of the associated user.</span></span>

### <a name="exceptions"></a><span data-ttu-id="fe890-128">Exceptions</span><span class="sxs-lookup"><span data-stu-id="fe890-128">Exceptions</span></span>
<span data-ttu-id="fe890-129">Alguns operadores não têm suporte: `$count` , `$search` , `$filter` .</span><span class="sxs-lookup"><span data-stu-id="fe890-129">Some operators are not supported: `$count`, `$search`, `$filter`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fe890-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fe890-130">Request headers</span></span>
| <span data-ttu-id="fe890-131">Nome</span><span class="sxs-lookup"><span data-stu-id="fe890-131">Name</span></span>      |<span data-ttu-id="fe890-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe890-132">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fe890-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="fe890-133">Authorization</span></span> | <span data-ttu-id="fe890-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fe890-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fe890-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fe890-136">Request body</span></span>
<span data-ttu-id="fe890-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fe890-137">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="fe890-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe890-138">Response</span></span>
<span data-ttu-id="fe890-139">Se tiver êxito, este método retornará um código `200 OK` de resposta e uma coleção de objetos [printJob](../resources/printjob.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fe890-139">If successful, this method returns a `200 OK` response code and collection of [printJob](../resources/printjob.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fe890-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fe890-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="fe890-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fe890-141">Request</span></span>
<span data-ttu-id="fe890-142">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fe890-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fe890-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="fe890-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_jobs_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/shares/{id}/jobs
```
# <a name="c"></a>[<span data-ttu-id="fe890-144">C#</span><span class="sxs-lookup"><span data-stu-id="fe890-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-jobs-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fe890-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fe890-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-jobs-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fe890-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fe890-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-jobs-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fe890-147">Java</span><span class="sxs-lookup"><span data-stu-id="fe890-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-jobs-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---

### <a name="response"></a><span data-ttu-id="fe890-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe890-148">Response</span></span>
<span data-ttu-id="fe890-149">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fe890-149">The following is an example of the response.</span></span>
><span data-ttu-id="fe890-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fe890-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
