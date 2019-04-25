---
title: Listar registeredDevices
description: Obtenha a lista de dispositivos registrado do usuário.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: fa2a0e8d9209a652c751bd30f0b950182c6525f8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32547785"
---
# <a name="list-registereddevices"></a><span data-ttu-id="b37f0-103">Listar registeredDevices</span><span class="sxs-lookup"><span data-stu-id="b37f0-103">List registeredDevices</span></span>

<span data-ttu-id="b37f0-104">Obtenha a lista de dispositivos registrado do usuário.</span><span class="sxs-lookup"><span data-stu-id="b37f0-104">Get the list of user's registered devices.</span></span>
## <a name="permissions"></a><span data-ttu-id="b37f0-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b37f0-105">Permissions</span></span>
<span data-ttu-id="b37f0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b37f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b37f0-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b37f0-108">Permission type</span></span>      | <span data-ttu-id="b37f0-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b37f0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b37f0-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b37f0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b37f0-111">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b37f0-111">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b37f0-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b37f0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b37f0-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b37f0-113">Not supported.</span></span>    |
|<span data-ttu-id="b37f0-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b37f0-114">Application</span></span> | <span data-ttu-id="b37f0-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b37f0-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b37f0-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b37f0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/registeredDevices
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b37f0-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b37f0-117">Optional query parameters</span></span>
<span data-ttu-id="b37f0-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b37f0-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b37f0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b37f0-119">Request headers</span></span>
| <span data-ttu-id="b37f0-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b37f0-120">Header</span></span>       | <span data-ttu-id="b37f0-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b37f0-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b37f0-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b37f0-122">Authorization</span></span>  | <span data-ttu-id="b37f0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b37f0-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b37f0-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b37f0-125">Accept</span></span>  | <span data-ttu-id="b37f0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b37f0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b37f0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b37f0-127">Request body</span></span>
<span data-ttu-id="b37f0-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b37f0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b37f0-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b37f0-129">Response</span></span>

<span data-ttu-id="b37f0-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b37f0-130">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b37f0-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b37f0-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b37f0-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b37f0-132">Request</span></span>
<span data-ttu-id="b37f0-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b37f0-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_registereddevices"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/registeredDevices
```
##### <a name="response"></a><span data-ttu-id="b37f0-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b37f0-134">Response</span></span>
<span data-ttu-id="b37f0-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b37f0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List registeredDevices",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
