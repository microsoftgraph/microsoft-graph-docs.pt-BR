---
title: Listar printServices
description: Recupere uma lista de objetos printService que representam os serviços disponíveis para seu locatário.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: c5226eadd4edfd3e8d2d15534eed3fcb5ffc9619
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516882"
---
# <a name="list-printservices"></a><span data-ttu-id="a27aa-103">Listar printServices</span><span class="sxs-lookup"><span data-stu-id="a27aa-103">List printServices</span></span>
<span data-ttu-id="a27aa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a27aa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="a27aa-105">Recupere uma lista de **objetos printService** que representam os serviços disponíveis para seu locatário.</span><span class="sxs-lookup"><span data-stu-id="a27aa-105">Retrieve a list of **printService** objects that represent the services available to your tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="a27aa-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a27aa-106">Permissions</span></span>
<span data-ttu-id="a27aa-107">Uma das permissões **de** Impressão Universal delegada [é](/graph/permissions-reference#universal-print-permissions) necessária para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="a27aa-107">One of the **delegated** Universal Print [permissions](/graph/permissions-reference#universal-print-permissions) is required to call this API.</span></span>

## <a name="http-request"></a><span data-ttu-id="a27aa-108">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a27aa-108">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/services
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a27aa-109">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a27aa-109">Optional query parameters</span></span>
<span data-ttu-id="a27aa-110">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a27aa-110">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="a27aa-111">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="a27aa-111">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a27aa-112">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a27aa-112">Request headers</span></span>
|<span data-ttu-id="a27aa-113">Nome</span><span class="sxs-lookup"><span data-stu-id="a27aa-113">Name</span></span>|<span data-ttu-id="a27aa-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="a27aa-114">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a27aa-115">Autorização</span><span class="sxs-lookup"><span data-stu-id="a27aa-115">Authorization</span></span>|<span data-ttu-id="a27aa-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a27aa-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a27aa-118">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a27aa-118">Request body</span></span>
<span data-ttu-id="a27aa-119">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a27aa-119">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a27aa-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="a27aa-120">Response</span></span>

<span data-ttu-id="a27aa-121">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos printService](../resources/printservice.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a27aa-121">If successful, this method returns a `200 OK` response code and a collection of [printService](../resources/printservice.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a27aa-122">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a27aa-122">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a27aa-123">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a27aa-123">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_printservice"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/services
```


### <a name="response"></a><span data-ttu-id="a27aa-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="a27aa-124">Response</span></span>
<span data-ttu-id="a27aa-125">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a27aa-125">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.printService)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/services",
  "value": [
    {
      "id": "f4cfee8b-4117-4773-a2f0-3807beb282b9",
      "endpoints": [
        {
          "id": "mpsdiscovery",
          "displayName": "Microsoft Universal Print Discovery Service",
          "uri": "https://discovery.print.microsoft.com"
        }
      ]
    }
  ]
}
```

