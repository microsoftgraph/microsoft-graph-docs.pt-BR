---
title: Obter printOperation
description: Recupere um printOperation.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: cfae83587eb4dcd0cf02f8367632df3b04a0c206
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516896"
---
# <a name="get-printoperation"></a><span data-ttu-id="a1fa9-103">Obter printOperation</span><span class="sxs-lookup"><span data-stu-id="a1fa9-103">Get printOperation</span></span>
<span data-ttu-id="a1fa9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a1fa9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="a1fa9-105">Recupere as propriedades e as relações de um [objeto printOperation.](../resources/printoperation.md)</span><span class="sxs-lookup"><span data-stu-id="a1fa9-105">Retrieve the properties and relationships of a [printOperation](../resources/printoperation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a1fa9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a1fa9-106">Permissions</span></span>
<span data-ttu-id="a1fa9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1fa9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="a1fa9-109">O usuário inscreveu deve ser um [Administrador de Impressora.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="a1fa9-109">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="a1fa9-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a1fa9-110">Permission type</span></span> | <span data-ttu-id="a1fa9-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a1fa9-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="a1fa9-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a1fa9-112">Delegated (work or school account)</span></span>| <span data-ttu-id="a1fa9-113">Printer.Create, Printer.ReadWrite.All, Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="a1fa9-113">Printer.Create, Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="a1fa9-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a1fa9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1fa9-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1fa9-115">Not Supported.</span></span>|
|<span data-ttu-id="a1fa9-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a1fa9-116">Application</span></span>| <span data-ttu-id="a1fa9-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1fa9-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a1fa9-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a1fa9-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/operations/{printOperationId}
```

## <a name="request-headers"></a><span data-ttu-id="a1fa9-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a1fa9-119">Request headers</span></span>
|<span data-ttu-id="a1fa9-120">Nome</span><span class="sxs-lookup"><span data-stu-id="a1fa9-120">Name</span></span>|<span data-ttu-id="a1fa9-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1fa9-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a1fa9-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a1fa9-122">Authorization</span></span>|<span data-ttu-id="a1fa9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a1fa9-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1fa9-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a1fa9-125">Request body</span></span>
<span data-ttu-id="a1fa9-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a1fa9-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a1fa9-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1fa9-127">Response</span></span>
<span data-ttu-id="a1fa9-128">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto printOperation](../resources/printOperation.md) (ou uma derivada de **printOperation**) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a1fa9-128">If successful, this method returns a `200 OK` response code and a [printOperation](../resources/printOperation.md) object (or a derivative of **printOperation**) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a1fa9-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a1fa9-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a1fa9-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a1fa9-130">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_printoperation"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/operations/{printOperationId}
```


### <a name="response"></a><span data-ttu-id="a1fa9-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1fa9-131">Response</span></span>
<span data-ttu-id="a1fa9-132">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a1fa9-132">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printOperation"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/operations/$entity",
    "@odata.type": "#microsoft.graph.printerCreateOperation",
    "id": "81f4cca3-b3b7-47ea-9f88-7ddbf7208ef4",
    "createdDateTime": "2020-06-15T22:27:03.031849Z",
    "certificate": "{ceritificate}",
    "status": {
        "state": "succeeded",
        "description": "The operation has completed successfully."
    },
    "printer": {
        "registeredDateTime": "2020-06-15T22:27:12.0920077Z",
        "isShared": false,
        "id": "e56f9cdd-acec-486f-a05e-b622ff0bcc7d",
        "displayName": "Test Printer",
        "manufacturer": "Test Printer Manufacturer",
        "model": "Test Printer Model",
        "isAcceptingJobs": null,
        "status": {
            "state": "unknown",
            "details": [],
            "description": ""
        },
        "location": {
            "latitude": null,
            "longitude": null
        }
    }
}
```

