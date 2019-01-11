---
title: Listar registeredOwners
description: Recupera uma lista de usuários que são proprietários registrados do dispositivo. Um proprietário registrado é o usuário que se associou ao dispositivo na nuvem ou que registrou o dispositivo pessoal. O proprietário registrado é definido no momento do registro. Atualmente, só pode haver um proprietário.
localization_priority: Normal
ms.openlocfilehash: f2b39217485ef248cb7da203152f8e87c483096d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845679"
---
# <a name="list-registeredowners"></a><span data-ttu-id="da368-106">Listar registeredOwners</span><span class="sxs-lookup"><span data-stu-id="da368-106">List registeredOwners</span></span>

<span data-ttu-id="da368-107">Recupera uma lista de usuários que são proprietários registrados do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="da368-107">Retrieve a list of users that are registered owners of the device.</span></span> <span data-ttu-id="da368-108">Um proprietário registrado é o usuário que se associou ao dispositivo na nuvem ou que registrou o dispositivo pessoal.</span><span class="sxs-lookup"><span data-stu-id="da368-108">A registered owner is the user that cloud joined the device or registered their personal device.</span></span> <span data-ttu-id="da368-109">O proprietário registrado é definido no momento do registro.</span><span class="sxs-lookup"><span data-stu-id="da368-109">The registered owner is set at the time of registration.</span></span> <span data-ttu-id="da368-110">Atualmente, só pode haver um proprietário.</span><span class="sxs-lookup"><span data-stu-id="da368-110">Currently, there can be only one owner.</span></span>

## <a name="permissions"></a><span data-ttu-id="da368-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="da368-111">Permissions</span></span>
<span data-ttu-id="da368-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da368-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="da368-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="da368-114">Permission type</span></span>      | <span data-ttu-id="da368-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="da368-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="da368-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="da368-116">Delegated (work or school account)</span></span> | <span data-ttu-id="da368-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="da368-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="da368-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="da368-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da368-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="da368-119">Not supported.</span></span>    |
|<span data-ttu-id="da368-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="da368-120">Application</span></span> | <span data-ttu-id="da368-121">Directory.Read.All ou Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da368-121">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="da368-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="da368-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredOwners
```
## <a name="optional-query-parameters"></a><span data-ttu-id="da368-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="da368-123">Optional query parameters</span></span>
<span data-ttu-id="da368-124">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="da368-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="da368-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="da368-125">Request headers</span></span>
| <span data-ttu-id="da368-126">Nome</span><span class="sxs-lookup"><span data-stu-id="da368-126">Name</span></span>       | <span data-ttu-id="da368-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="da368-127">Type</span></span> | <span data-ttu-id="da368-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="da368-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="da368-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="da368-129">Authorization</span></span>  | <span data-ttu-id="da368-130">string</span><span class="sxs-lookup"><span data-stu-id="da368-130">string</span></span>  | <span data-ttu-id="da368-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="da368-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="da368-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="da368-133">Request body</span></span>
<span data-ttu-id="da368-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="da368-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="da368-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="da368-135">Response</span></span>

<span data-ttu-id="da368-136">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="da368-136">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="da368-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="da368-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="da368-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="da368-138">Request</span></span>
<span data-ttu-id="da368-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="da368-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_registeredowners"
}-->
```http
GET https://graph.microsoft.com/v1.0/devices/{id}/registeredOwners
```
##### <a name="response"></a><span data-ttu-id="da368-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="da368-140">Response</span></span>
<span data-ttu-id="da368-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="da368-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
