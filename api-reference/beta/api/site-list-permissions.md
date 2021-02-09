---
title: Listar permissões
description: Obter os recursos de permissão da propriedade de navegação de permissões em um site.
author: BarrySh
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: bcaa0cd18268bbfbc079883eb91cc74a88d87d96
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160151"
---
# <a name="list-permissions"></a><span data-ttu-id="62060-103">Listar permissões</span><span class="sxs-lookup"><span data-stu-id="62060-103">List permissions</span></span>
<span data-ttu-id="62060-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62060-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="62060-105">Obter os [recursos de](../resources/permission.md) permissão da propriedade de navegação de permissões em um site.</span><span class="sxs-lookup"><span data-stu-id="62060-105">Get the [permission](../resources/permission.md) resources from the permissions navigation property on a site.</span></span>

## <a name="permissions"></a><span data-ttu-id="62060-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="62060-106">Permissions</span></span>
<span data-ttu-id="62060-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62060-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62060-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="62060-109">Permission type</span></span>                        | <span data-ttu-id="62060-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="62060-110">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="62060-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="62060-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="62060-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="62060-112">Not supported.</span></span>
|<span data-ttu-id="62060-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="62060-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="62060-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="62060-114">Not supported.</span></span>
|<span data-ttu-id="62060-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="62060-115">Application</span></span>                            | <span data-ttu-id="62060-116">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="62060-116">Sites.FullControl.All</span></span>

## <a name="http-request"></a><span data-ttu-id="62060-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="62060-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /sites/{sitesId}/permissions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="62060-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="62060-118">Optional query parameters</span></span>
<span data-ttu-id="62060-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="62060-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="62060-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="62060-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="62060-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="62060-121">Request headers</span></span>
|<span data-ttu-id="62060-122">Nome</span><span class="sxs-lookup"><span data-stu-id="62060-122">Name</span></span>|<span data-ttu-id="62060-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="62060-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="62060-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="62060-124">Authorization</span></span>|<span data-ttu-id="62060-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="62060-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="62060-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="62060-127">Request body</span></span>
<span data-ttu-id="62060-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="62060-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="62060-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="62060-129">Response</span></span>

<span data-ttu-id="62060-130">Se bem-sucedido, este método retorna um código de resposta e uma `200 OK` coleção de objetos [permission](../resources/permission.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="62060-130">If successful, this method returns a `200 OK` response code and a collection of [permission](../resources/permission.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="62060-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="62060-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="62060-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="62060-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_permission"
}
-->
``` http
GET https://graph.microsoft.com/beta/sites/{sitesId}/permissions
```


### <a name="response"></a><span data-ttu-id="62060-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="62060-133">Response</span></span>
<span data-ttu-id="62060-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="62060-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.permission)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "1",
      "roles": ["read"],
      "grantedToIdentities": [{
        "application": {
          "id": "89ea5c94-7736-4e25-95ad-3fa95f62b66e",
          "displayName": "Foo App"
        }
      }]
    },
    {
      "id": "2",
      "roles": ["write"],
      "grantedToIdentities": [{
        "application": {
          "id": "22f09bb7-dd29-403e-bec2-ab5cde52c2b3",
          "displayName": "Bar App"
        }
      }]
    }
  ]
}
```

<!-- {
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Sites/Permissions/List site permissions"
} -->