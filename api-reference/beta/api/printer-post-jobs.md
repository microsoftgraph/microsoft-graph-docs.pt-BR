---
title: Criar printJob
description: Criar um novo printJob para uma impressora.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 615058e5aded858c40dc51f274ec40a1f3b64dec
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/30/2020
ms.locfileid: "48314402"
---
# <a name="create-printjob"></a><span data-ttu-id="96b2e-103">Criar printJob</span><span class="sxs-lookup"><span data-stu-id="96b2e-103">Create printJob</span></span>

<span data-ttu-id="96b2e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96b2e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96b2e-105">Criar um novo [printJob](../resources/printJob.md) para uma [impressora](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="96b2e-105">Create a new [printJob](../resources/printJob.md) for a [printer](../resources/printer.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="96b2e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="96b2e-106">Permissions</span></span>
<span data-ttu-id="96b2e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96b2e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="96b2e-109">Além das permissões a seguir, o locatário do usuário ou do aplicativo deve ter uma assinatura universal de impressão ativa e ter uma permissão que conceda obter acesso à [impressora](printer-get.md) .</span><span class="sxs-lookup"><span data-stu-id="96b2e-109">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printer](printer-get.md) access.</span></span> <span data-ttu-id="96b2e-110">O usuário conectado deve ser um [administrador da impressora](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span><span class="sxs-lookup"><span data-stu-id="96b2e-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="96b2e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="96b2e-111">Permission type</span></span> | <span data-ttu-id="96b2e-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="96b2e-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="96b2e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="96b2e-113">Delegated (work or school account)</span></span>| <span data-ttu-id="96b2e-114">PrintJob. ReadWriteBasic, PrintJob. ReadWrite, PrintJob. ReadWriteBasic. All, PrintJob. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="96b2e-114">PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="96b2e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="96b2e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="96b2e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="96b2e-116">Not Supported.</span></span>|
|<span data-ttu-id="96b2e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="96b2e-117">Application</span></span>| <span data-ttu-id="96b2e-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="96b2e-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="96b2e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="96b2e-119">HTTP request</span></span>

```http
POST print/printers/{id}/jobs
```

## <a name="request-headers"></a><span data-ttu-id="96b2e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="96b2e-120">Request headers</span></span>
| <span data-ttu-id="96b2e-121">Nome</span><span class="sxs-lookup"><span data-stu-id="96b2e-121">Name</span></span>      |<span data-ttu-id="96b2e-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="96b2e-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="96b2e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="96b2e-123">Authorization</span></span> | <span data-ttu-id="96b2e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="96b2e-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="96b2e-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="96b2e-126">Content-type</span></span>  | <span data-ttu-id="96b2e-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="96b2e-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="96b2e-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="96b2e-129">Request body</span></span>
<span data-ttu-id="96b2e-130">No corpo da solicitação, forneça uma representação JSON de um objeto [printJob](../resources/printjob.md) , incluindo um objeto [Document](../resources/printDocument.md) .</span><span class="sxs-lookup"><span data-stu-id="96b2e-130">In the request body, supply a JSON representation of a [printJob](../resources/printjob.md) object, including one [printDocument](../resources/printDocument.md) object.</span></span> <span data-ttu-id="96b2e-131">As IDs de trabalho e de documento são definidas automaticamente durante a criação do recurso.</span><span class="sxs-lookup"><span data-stu-id="96b2e-131">The job and document IDs are set automatically during resource creation.</span></span>

<span data-ttu-id="96b2e-132">No momento, a impressão universal suporta apenas um **documento** impresso por objeto **printJob** .</span><span class="sxs-lookup"><span data-stu-id="96b2e-132">Right now, Universal Print supports only one **printDocument** per **printJob** object.</span></span>

## <a name="response"></a><span data-ttu-id="96b2e-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="96b2e-133">Response</span></span>
<span data-ttu-id="96b2e-134">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto printJob e o [documento](../resources/printDocument.md) de [impressão](../resources/printjob.md) associado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="96b2e-134">If successful, this method returns a `201 Created` response code and a [printJob](../resources/printjob.md) object and associated [printDocument](../resources/printDocument.md) in the response body.</span></span> 
## <a name="example"></a><span data-ttu-id="96b2e-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="96b2e-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="96b2e-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="96b2e-136">Request</span></span>
<span data-ttu-id="96b2e-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="96b2e-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="96b2e-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="96b2e-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_printjob"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/{id}/jobs
```
# <a name="javascript"></a>[<span data-ttu-id="96b2e-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="96b2e-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-printjob-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="96b2e-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="96b2e-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-printjob-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="96b2e-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="96b2e-141">Response</span></span>
<span data-ttu-id="96b2e-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="96b2e-142">The following is an example of the response.</span></span>
><span data-ttu-id="96b2e-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="96b2e-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printJob"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 425

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printJobs/$entity",
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