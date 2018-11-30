---
title: Listar registeredUsers
description: Recupera uma lista de usuários que são usuários registrados do dispositivo.
ms.openlocfilehash: 370990b5b9c61b071620fe0df04fd38e98892bd1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006668"
---
# <a name="list-registeredusers"></a><span data-ttu-id="d5c8b-103">Listar registeredUsers</span><span class="sxs-lookup"><span data-stu-id="d5c8b-103">List registeredUsers</span></span>

<span data-ttu-id="d5c8b-104">Recupera uma lista de usuários que são usuários registrados do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d5c8b-104">Retrieve a list of users that are registered users of the device.</span></span>

<span data-ttu-id="d5c8b-105">Para dispositivos associados em nuvem e dispositivos pessoais registrados, os usuários registrados são definidos para o mesmo valor que proprietários registrados no momento do registro.</span><span class="sxs-lookup"><span data-stu-id="d5c8b-105">For cloud joined devices and registered personal devices, registered users are set to the same value as registered owners at the time of registration.</span></span>

## <a name="permissions"></a><span data-ttu-id="d5c8b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d5c8b-106">Permissions</span></span>
<span data-ttu-id="d5c8b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5c8b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d5c8b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d5c8b-109">Permission type</span></span>      | <span data-ttu-id="d5c8b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d5c8b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d5c8b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d5c8b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d5c8b-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d5c8b-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d5c8b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d5c8b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d5c8b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d5c8b-114">Not supported.</span></span>    |
|<span data-ttu-id="d5c8b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d5c8b-115">Application</span></span> | <span data-ttu-id="d5c8b-116">Directory.Read.All ou Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5c8b-116">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d5c8b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d5c8b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredUsers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d5c8b-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d5c8b-118">Optional query parameters</span></span>
<span data-ttu-id="d5c8b-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d5c8b-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d5c8b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d5c8b-120">Request headers</span></span>
| <span data-ttu-id="d5c8b-121">Nome</span><span class="sxs-lookup"><span data-stu-id="d5c8b-121">Name</span></span>       | <span data-ttu-id="d5c8b-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="d5c8b-122">Type</span></span> | <span data-ttu-id="d5c8b-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5c8b-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d5c8b-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="d5c8b-124">Authorization</span></span>  | <span data-ttu-id="d5c8b-125">string</span><span class="sxs-lookup"><span data-stu-id="d5c8b-125">string</span></span>  | <span data-ttu-id="d5c8b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d5c8b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d5c8b-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d5c8b-128">Request body</span></span>
<span data-ttu-id="d5c8b-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d5c8b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d5c8b-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5c8b-130">Response</span></span>

<span data-ttu-id="d5c8b-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d5c8b-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d5c8b-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d5c8b-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d5c8b-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d5c8b-133">Request</span></span>
<span data-ttu-id="d5c8b-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d5c8b-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_registeredusers"
}-->
```http
GET https://graph.microsoft.com/v1.0/devices/{id}/registeredUsers
```
##### <a name="response"></a><span data-ttu-id="d5c8b-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5c8b-135">Response</span></span>
<span data-ttu-id="d5c8b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d5c8b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List registeredUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->