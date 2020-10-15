---
title: Listar registeredOwners
description: Recupera uma lista de usuários que são proprietários registrados do dispositivo.
localization_priority: Normal
author: spunukol
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c7f86a1c2038cd9d6ff477d3c18cbf00b829624a
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/14/2020
ms.locfileid: "48457860"
---
# <a name="list-registeredowners"></a><span data-ttu-id="fecdc-103">Listar registeredOwners</span><span class="sxs-lookup"><span data-stu-id="fecdc-103">List registeredOwners</span></span>

<span data-ttu-id="fecdc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fecdc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fecdc-105">Recupera uma lista de usuários que são proprietários registrados do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fecdc-105">Retrieve a list of users that are registered owners of the device.</span></span> <span data-ttu-id="fecdc-106">Um proprietário registrado é o usuário que se associou ao dispositivo na nuvem ou que registrou o dispositivo pessoal.</span><span class="sxs-lookup"><span data-stu-id="fecdc-106">A registered owner is the user that cloud joined the device or registered their personal device.</span></span> <span data-ttu-id="fecdc-107">O proprietário registrado é definido no momento do registro.</span><span class="sxs-lookup"><span data-stu-id="fecdc-107">The registered owner is set at the time of registration.</span></span> <span data-ttu-id="fecdc-108">Atualmente, só pode haver um proprietário.</span><span class="sxs-lookup"><span data-stu-id="fecdc-108">Currently, there can be only one owner.</span></span>

## <a name="permissions"></a><span data-ttu-id="fecdc-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="fecdc-109">Permissions</span></span>
<span data-ttu-id="fecdc-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fecdc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="fecdc-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fecdc-112">Permission type</span></span>      | <span data-ttu-id="fecdc-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fecdc-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fecdc-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fecdc-114">Delegated (work or school account)</span></span> | <span data-ttu-id="fecdc-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fecdc-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fecdc-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fecdc-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fecdc-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fecdc-117">Not supported.</span></span>    |
|<span data-ttu-id="fecdc-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fecdc-118">Application</span></span> | <span data-ttu-id="fecdc-119">Directory.Read.All ou Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fecdc-119">Directory.Read.All or Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="fecdc-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fecdc-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredOwners
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fecdc-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fecdc-121">Optional query parameters</span></span>
<span data-ttu-id="fecdc-122">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fecdc-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="fecdc-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fecdc-123">Request headers</span></span>
| <span data-ttu-id="fecdc-124">Nome</span><span class="sxs-lookup"><span data-stu-id="fecdc-124">Name</span></span>       | <span data-ttu-id="fecdc-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="fecdc-125">Type</span></span> | <span data-ttu-id="fecdc-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="fecdc-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="fecdc-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="fecdc-127">Authorization</span></span>  | <span data-ttu-id="fecdc-128">string</span><span class="sxs-lookup"><span data-stu-id="fecdc-128">string</span></span>  | <span data-ttu-id="fecdc-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fecdc-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fecdc-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fecdc-131">Request body</span></span>
<span data-ttu-id="fecdc-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fecdc-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fecdc-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="fecdc-133">Response</span></span>

<span data-ttu-id="fecdc-134">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fecdc-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fecdc-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fecdc-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fecdc-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fecdc-136">Request</span></span>
<span data-ttu-id="fecdc-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fecdc-137">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fecdc-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="fecdc-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_registeredowners"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices/{id}/registeredOwners
```
# <a name="c"></a>[<span data-ttu-id="fecdc-139">C#</span><span class="sxs-lookup"><span data-stu-id="fecdc-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-registeredowners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fecdc-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fecdc-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-registeredowners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fecdc-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fecdc-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-registeredowners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fecdc-142">Java</span><span class="sxs-lookup"><span data-stu-id="fecdc-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-registeredowners-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="fecdc-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="fecdc-143">Response</span></span>
<span data-ttu-id="fecdc-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fecdc-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List registeredOwners",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
