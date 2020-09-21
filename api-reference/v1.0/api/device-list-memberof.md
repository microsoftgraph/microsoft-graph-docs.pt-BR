---
title: Listar grupos de dispositivos
description: Obter grupos dos quais este dispositivo é membro direto. Essa operação não é transitiva.
author: spunukol
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b3e06502e05a883630e6fe1f211a5715dd01aac5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013339"
---
# <a name="list-device-groups"></a><span data-ttu-id="ac311-104">Listar grupos de dispositivos</span><span class="sxs-lookup"><span data-stu-id="ac311-104">List device groups</span></span>

<span data-ttu-id="ac311-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac311-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ac311-106">Obter grupos dos quais este dispositivo é membro direto.</span><span class="sxs-lookup"><span data-stu-id="ac311-106">Get groups that this device is a direct member of.</span></span> <span data-ttu-id="ac311-107">Essa operação não é transitiva.</span><span class="sxs-lookup"><span data-stu-id="ac311-107">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="ac311-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="ac311-108">Permissions</span></span>

<span data-ttu-id="ac311-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ac311-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ac311-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ac311-111">Permission type</span></span>      | <span data-ttu-id="ac311-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ac311-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ac311-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ac311-113">Delegated (work or school account)</span></span> | <span data-ttu-id="ac311-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ac311-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ac311-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ac311-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ac311-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ac311-116">Not supported.</span></span>    |
|<span data-ttu-id="ac311-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ac311-117">Application</span></span> | <span data-ttu-id="ac311-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac311-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="ac311-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ac311-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ac311-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ac311-120">Optional query parameters</span></span>
<span data-ttu-id="ac311-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ac311-121">This method supports the [OData Query Parameters](/graph/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ac311-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ac311-122">Request headers</span></span>
| <span data-ttu-id="ac311-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ac311-123">Header</span></span>       | <span data-ttu-id="ac311-124">Valor</span><span class="sxs-lookup"><span data-stu-id="ac311-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ac311-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="ac311-125">Authorization</span></span>  | <span data-ttu-id="ac311-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ac311-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ac311-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ac311-128">Accept</span></span>  | <span data-ttu-id="ac311-129">application/json</span><span class="sxs-lookup"><span data-stu-id="ac311-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ac311-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ac311-130">Request body</span></span>
<span data-ttu-id="ac311-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ac311-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ac311-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac311-132">Response</span></span>

<span data-ttu-id="ac311-133">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ac311-133">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac311-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ac311-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="ac311-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ac311-135">Request</span></span>

<span data-ttu-id="ac311-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ac311-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ac311-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="ac311-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_device_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="ac311-138">C#</span><span class="sxs-lookup"><span data-stu-id="ac311-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-device-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ac311-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ac311-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-device-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ac311-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ac311-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-device-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ac311-141">Java</span><span class="sxs-lookup"><span data-stu-id="ac311-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-device-memberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ac311-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac311-142">Response</span></span>
<span data-ttu-id="ac311-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ac311-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All users at the company",
      "displayName": "All Users",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true,
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

