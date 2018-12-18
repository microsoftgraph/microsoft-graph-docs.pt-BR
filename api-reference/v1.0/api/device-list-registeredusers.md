---
title: Listar registeredUsers
description: Recupera uma lista de usuários que são usuários registrados do dispositivo.
author: tfitzmac
ms.openlocfilehash: 7b6f861e275ea36eb864aee5958c94055e8e8168
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27336796"
---
# <a name="list-registeredusers"></a><span data-ttu-id="b6a73-103">Listar registeredUsers</span><span class="sxs-lookup"><span data-stu-id="b6a73-103">List registeredUsers</span></span>

<span data-ttu-id="b6a73-104">Recupera uma lista de usuários que são usuários registrados do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b6a73-104">Retrieve a list of users that are registered users of the device.</span></span>

<span data-ttu-id="b6a73-105">Para dispositivos associados em nuvem e dispositivos pessoais registrados, os usuários registrados são definidos para o mesmo valor que proprietários registrados no momento do registro.</span><span class="sxs-lookup"><span data-stu-id="b6a73-105">For cloud joined devices and registered personal devices, registered users are set to the same value as registered owners at the time of registration.</span></span>

## <a name="permissions"></a><span data-ttu-id="b6a73-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b6a73-106">Permissions</span></span>
<span data-ttu-id="b6a73-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6a73-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b6a73-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b6a73-109">Permission type</span></span>      | <span data-ttu-id="b6a73-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b6a73-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b6a73-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b6a73-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b6a73-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b6a73-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b6a73-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b6a73-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b6a73-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6a73-114">Not supported.</span></span>    |
|<span data-ttu-id="b6a73-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b6a73-115">Application</span></span> | <span data-ttu-id="b6a73-116">Directory.Read.All ou Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6a73-116">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b6a73-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b6a73-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredUsers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b6a73-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b6a73-118">Optional query parameters</span></span>
<span data-ttu-id="b6a73-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b6a73-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b6a73-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b6a73-120">Request headers</span></span>
| <span data-ttu-id="b6a73-121">Nome</span><span class="sxs-lookup"><span data-stu-id="b6a73-121">Name</span></span>       | <span data-ttu-id="b6a73-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="b6a73-122">Type</span></span> | <span data-ttu-id="b6a73-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6a73-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b6a73-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="b6a73-124">Authorization</span></span>  | <span data-ttu-id="b6a73-125">string</span><span class="sxs-lookup"><span data-stu-id="b6a73-125">string</span></span>  | <span data-ttu-id="b6a73-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b6a73-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b6a73-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b6a73-128">Request body</span></span>
<span data-ttu-id="b6a73-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b6a73-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b6a73-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6a73-130">Response</span></span>

<span data-ttu-id="b6a73-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b6a73-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b6a73-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b6a73-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b6a73-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b6a73-133">Request</span></span>
<span data-ttu-id="b6a73-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b6a73-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_registeredusers"
}-->
```http
GET https://graph.microsoft.com/v1.0/devices/{id}/registeredUsers
```
##### <a name="response"></a><span data-ttu-id="b6a73-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6a73-135">Response</span></span>
<span data-ttu-id="b6a73-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b6a73-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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