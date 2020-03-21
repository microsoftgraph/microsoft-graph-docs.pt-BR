---
title: Criar printJob
description: Criar um novo printJob para uma impressora.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: e1cae1610877ae9354729d31c0999185612c3b86
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895556"
---
# <a name="create-printjob"></a><span data-ttu-id="0ab2d-103">Criar printJob</span><span class="sxs-lookup"><span data-stu-id="0ab2d-103">Create printJob</span></span>

<span data-ttu-id="0ab2d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0ab2d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ab2d-105">Criar um novo [printJob](../resources/printJob.md) para uma [impressora](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="0ab2d-105">Create a new [printJob](../resources/printJob.md) for a [printer](../resources/printer.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="0ab2d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0ab2d-106">Permissions</span></span>
<span data-ttu-id="0ab2d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ab2d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="0ab2d-109">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="0ab2d-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="0ab2d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0ab2d-110">Permission type</span></span> | <span data-ttu-id="0ab2d-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0ab2d-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="0ab2d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0ab2d-112">Delegated (work or school account)</span></span>| <span data-ttu-id="0ab2d-113">Users. Read. All</span><span class="sxs-lookup"><span data-stu-id="0ab2d-113">Users.Read.All</span></span> |
|<span data-ttu-id="0ab2d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0ab2d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ab2d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0ab2d-115">Not Supported.</span></span>|
|<span data-ttu-id="0ab2d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0ab2d-116">Application</span></span>|<span data-ttu-id="0ab2d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0ab2d-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ab2d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0ab2d-118">HTTP request</span></span>

```http
POST print/printers/{id}/jobs
```

## <a name="request-headers"></a><span data-ttu-id="0ab2d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0ab2d-119">Request headers</span></span>
| <span data-ttu-id="0ab2d-120">Nome</span><span class="sxs-lookup"><span data-stu-id="0ab2d-120">Name</span></span>      |<span data-ttu-id="0ab2d-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ab2d-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0ab2d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0ab2d-122">Authorization</span></span> | <span data-ttu-id="0ab2d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0ab2d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0ab2d-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="0ab2d-125">Content-type</span></span>  | <span data-ttu-id="0ab2d-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0ab2d-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ab2d-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0ab2d-128">Request body</span></span>
<span data-ttu-id="0ab2d-129">No corpo da solicitação, forneça uma representação JSON de um objeto [printJob](../resources/printjob.md) , incluindo um objeto [Document](../resources/printDocument.md) .</span><span class="sxs-lookup"><span data-stu-id="0ab2d-129">In the request body, supply a JSON representation of a [printJob](../resources/printjob.md) object, including one [printDocument](../resources/printDocument.md) object.</span></span> <span data-ttu-id="0ab2d-130">As IDs de trabalho e de documento são definidas automaticamente durante a criação do recurso.</span><span class="sxs-lookup"><span data-stu-id="0ab2d-130">The job and document IDs are set automatically during resource creation.</span></span>

<span data-ttu-id="0ab2d-131">No momento, a impressão universal suporta apenas um **documento** impresso por objeto **printJob** .</span><span class="sxs-lookup"><span data-stu-id="0ab2d-131">Right now, Universal Print supports only one **printDocument** per **printJob** object.</span></span>

## <a name="response"></a><span data-ttu-id="0ab2d-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ab2d-132">Response</span></span>
<span data-ttu-id="0ab2d-133">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto printJob e o [documento](../resources/printDocument.md) de [impressão](../resources/printjob.md) associado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0ab2d-133">If successful, this method returns a `201 Created` response code and a [printJob](../resources/printjob.md) object and associated [printDocument](../resources/printDocument.md) in the response body.</span></span> 
## <a name="example"></a><span data-ttu-id="0ab2d-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0ab2d-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0ab2d-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0ab2d-135">Request</span></span>
<span data-ttu-id="0ab2d-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0ab2d-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_printjob"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/{id}/jobs
```
##### <a name="response"></a><span data-ttu-id="0ab2d-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ab2d-137">Response</span></span>
<span data-ttu-id="0ab2d-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0ab2d-138">The following is an example of the response.</span></span>
><span data-ttu-id="0ab2d-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0ab2d-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
