---
title: Listar ownedObjects
description: Obtenha a lista de objetos de diretório de propriedade do usuário.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2fade3519bb0435c54b185816fb2e6d919d2234a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27913363"
---
# <a name="list-ownedobjects"></a><span data-ttu-id="a4e0c-103">Listar ownedObjects</span><span class="sxs-lookup"><span data-stu-id="a4e0c-103">List ownedObjects</span></span>

> <span data-ttu-id="a4e0c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a4e0c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a4e0c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a4e0c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a4e0c-106">Obtenha a lista de objetos de diretório de propriedade do usuário.</span><span class="sxs-lookup"><span data-stu-id="a4e0c-106">Get the list of directory objects that are owned by the user.</span></span>
## <a name="permissions"></a><span data-ttu-id="a4e0c-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="a4e0c-107">Permissions</span></span>
<span data-ttu-id="a4e0c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4e0c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4e0c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a4e0c-110">Permission type</span></span>      | <span data-ttu-id="a4e0c-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a4e0c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a4e0c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a4e0c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a4e0c-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a4e0c-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a4e0c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a4e0c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a4e0c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a4e0c-115">Not supported.</span></span>    |
|<span data-ttu-id="a4e0c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a4e0c-116">Application</span></span> | <span data-ttu-id="a4e0c-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4e0c-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a4e0c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a4e0c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/ownedObjects
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a4e0c-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a4e0c-119">Optional query parameters</span></span>
<span data-ttu-id="a4e0c-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a4e0c-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a4e0c-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a4e0c-121">Request headers</span></span>
| <span data-ttu-id="a4e0c-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a4e0c-122">Header</span></span>       | <span data-ttu-id="a4e0c-123">Valor</span><span class="sxs-lookup"><span data-stu-id="a4e0c-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a4e0c-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="a4e0c-124">Authorization</span></span>  | <span data-ttu-id="a4e0c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a4e0c-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a4e0c-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a4e0c-127">Accept</span></span>  | <span data-ttu-id="a4e0c-128">application/json</span><span class="sxs-lookup"><span data-stu-id="a4e0c-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4e0c-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a4e0c-129">Request body</span></span>
<span data-ttu-id="a4e0c-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a4e0c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a4e0c-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="a4e0c-131">Response</span></span>

<span data-ttu-id="a4e0c-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a4e0c-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a4e0c-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a4e0c-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a4e0c-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a4e0c-134">Request</span></span>
<span data-ttu-id="a4e0c-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a4e0c-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_ownedobjects"
}-->
```http
GET https://graph.microsoft.com/beta/me/ownedObjects
```
##### <a name="response"></a><span data-ttu-id="a4e0c-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="a4e0c-136">Response</span></span>
<span data-ttu-id="a4e0c-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a4e0c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List ownedObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
