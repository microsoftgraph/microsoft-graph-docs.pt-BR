---
title: Listar printJobs para uma printerShare
description: Recupere uma lista de trabalhos de impressão associados ao compartilhamento de impressão.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 7899640922cd5f8ba38d11bba03c485dbb6099bd
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053913"
---
# <a name="list-printjobs-for-a-printershare"></a><span data-ttu-id="735dd-103">Listar printJobs para uma printerShare</span><span class="sxs-lookup"><span data-stu-id="735dd-103">List printJobs for a printerShare</span></span>
<span data-ttu-id="735dd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="735dd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="735dd-105">Recupere uma lista de trabalhos de impressão associados à [printerShare](../resources/printershare.md).</span><span class="sxs-lookup"><span data-stu-id="735dd-105">Retrieve a list of print jobs associated with the [printerShare](../resources/printershare.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="735dd-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="735dd-106">Permissions</span></span>
<span data-ttu-id="735dd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="735dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="735dd-109">Para usar o serviço impressão universal, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa, uma permissão que concede acesso [Get printerShare](printershare-get.md) e uma das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="735dd-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, a permission that grants [Get printerShare](printershare-get.md) access, and one of the permissions listed in the following table.</span></span>

<span data-ttu-id="735dd-110">Para ler trabalhos de impressão de outro usuário, o usuário inscreveu precisa ser um administrador de impressão e ter a permissão PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All ou PrintJob.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="735dd-110">To read print jobs from another user, the signed in user needs to be a print administrator and have the PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All, or PrintJob.ReadWrite.All permission.</span></span>

|<span data-ttu-id="735dd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="735dd-111">Permission type</span></span> | <span data-ttu-id="735dd-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="735dd-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="735dd-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="735dd-113">Delegated (work or school account)</span></span>| <span data-ttu-id="735dd-114">PrintJob.ReadBasic, PrintJob.Read, PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="735dd-114">PrintJob.ReadBasic, PrintJob.Read, PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="735dd-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="735dd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="735dd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="735dd-116">Not Supported.</span></span>|
|<span data-ttu-id="735dd-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="735dd-117">Application</span></span>| <span data-ttu-id="735dd-118">PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="735dd-118">PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="735dd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="735dd-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/shares/{printerShareId}/jobs
```

## <a name="optional-query-parameters"></a><span data-ttu-id="735dd-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="735dd-120">Optional query parameters</span></span>
<span data-ttu-id="735dd-121">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="735dd-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="735dd-122">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="735dd-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

* <span data-ttu-id="735dd-123">A **propriedade documents** é omitida da resposta por padrão.</span><span class="sxs-lookup"><span data-stu-id="735dd-123">The **documents** property is omitted from the response by default.</span></span> <span data-ttu-id="735dd-124">Para também retornar uma lista de [printDocuments](../resources/printdocument.md) para cada trabalho de impressão, use `$expand=documents` .</span><span class="sxs-lookup"><span data-stu-id="735dd-124">To also return a list of [printDocuments](../resources/printdocument.md) for each print job, use `$expand=documents`.</span></span>
* <span data-ttu-id="735dd-125">Este método dá suporte à filtragem de trabalhos de impressão pelo usuário que os criou.</span><span class="sxs-lookup"><span data-stu-id="735dd-125">This method supports filtering print jobs by the user who created them.</span></span> <span data-ttu-id="735dd-126">Use `$filter=createdBy/userPrincipalName eq '{upn}'` , onde **{upn}** é [o nome principal do](/azure/active-directory/hybrid/plan-connect-userprincipalname#what-is-userprincipalname) usuário do usuário associado.</span><span class="sxs-lookup"><span data-stu-id="735dd-126">Use `$filter=createdBy/userPrincipalName eq '{upn}'`, where **{upn}** is the [user principal name](/azure/active-directory/hybrid/plan-connect-userprincipalname#what-is-userprincipalname) of the associated user.</span></span>

### <a name="exceptions"></a><span data-ttu-id="735dd-127">Exceções</span><span class="sxs-lookup"><span data-stu-id="735dd-127">Exceptions</span></span>
<span data-ttu-id="735dd-128">Alguns operadores não têm suporte: `$count` , `$search` .</span><span class="sxs-lookup"><span data-stu-id="735dd-128">Some operators are not supported: `$count`, `$search`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="735dd-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="735dd-129">Request headers</span></span>
|<span data-ttu-id="735dd-130">Nome</span><span class="sxs-lookup"><span data-stu-id="735dd-130">Name</span></span>|<span data-ttu-id="735dd-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="735dd-131">Description</span></span>|
|:---|:---|
|<span data-ttu-id="735dd-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="735dd-132">Authorization</span></span>|<span data-ttu-id="735dd-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="735dd-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="735dd-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="735dd-135">Request body</span></span>
<span data-ttu-id="735dd-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="735dd-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="735dd-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="735dd-137">Response</span></span>

<span data-ttu-id="735dd-138">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos printJob](../resources/printjob.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="735dd-138">If successful, this method returns a `200 OK` response code and a collection of [printJob](../resources/printjob.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="735dd-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="735dd-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="735dd-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="735dd-140">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="735dd-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="735dd-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_printjob_2"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/shares/{printerShareId}/jobs
```
# <a name="c"></a>[<span data-ttu-id="735dd-142">C#</span><span class="sxs-lookup"><span data-stu-id="735dd-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-printjob-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="735dd-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="735dd-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-printjob-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="735dd-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="735dd-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-printjob-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="735dd-145">Java</span><span class="sxs-lookup"><span data-stu-id="735dd-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-printjob-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="735dd-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="735dd-146">Response</span></span>
<span data-ttu-id="735dd-147">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="735dd-147">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.printJob)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/shares('f37141d9-0afb-484f-96d3-0ef0a679e6c1')/jobs",
  "value": [
    {
      "id": "103",
      "createdDateTime": "2020-02-04T00:00:00.0000000Z",
      "createdBy": {        
      },
      "status": {
        "state": "completed",
        "description": "The print job has completed successfully and no further processing will take place.",
        "details": [          
        ],
        "isAcquiredByPrinter": true
      },
      "configuration": {        
      },
      "redirectedTo": null,
      "redirectedFrom": null,
      "isFetchable": false
    }
  ]
}
```

