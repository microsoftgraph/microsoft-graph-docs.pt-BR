---
title: Listar memberOf
description: 'Obtenha todos os grupos e funções de diretório dos quais o usuário é um membro direto. '
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 36a99730128fca385394121b75437cd807a2b400
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32571307"
---
# <a name="list-memberof"></a><span data-ttu-id="0736f-103">Listar memberOf</span><span class="sxs-lookup"><span data-stu-id="0736f-103">List memberOf</span></span>

<span data-ttu-id="0736f-104">Obtenha [grupos](../resources/group.md) e [funções de diretório](../resources/directoryrole.md) dos quais o usuário é membro.</span><span class="sxs-lookup"><span data-stu-id="0736f-104">Get [groups](../resources/group.md) and [directory roles](../resources/directoryrole.md) that the user is a direct member of.</span></span> 

## <a name="permissions"></a><span data-ttu-id="0736f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0736f-105">Permissions</span></span>
<span data-ttu-id="0736f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0736f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0736f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0736f-108">Permission type</span></span>      | <span data-ttu-id="0736f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0736f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0736f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0736f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0736f-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0736f-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0736f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0736f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0736f-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0736f-113">Not supported.</span></span>    |
|<span data-ttu-id="0736f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0736f-114">Application</span></span> | <span data-ttu-id="0736f-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0736f-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0736f-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0736f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/memberOf
or
GET /users/{id | userPrincipalName}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0736f-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0736f-117">Optional query parameters</span></span>
<span data-ttu-id="0736f-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0736f-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> <span data-ttu-id="0736f-119">$filter não é suportado.</span><span class="sxs-lookup"><span data-stu-id="0736f-119">$filter is not supported.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="0736f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0736f-120">Request headers</span></span>
| <span data-ttu-id="0736f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0736f-121">Header</span></span>       | <span data-ttu-id="0736f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0736f-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0736f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0736f-123">Authorization</span></span>  | <span data-ttu-id="0736f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0736f-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0736f-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0736f-126">Accept</span></span>  | <span data-ttu-id="0736f-127">application/json</span><span class="sxs-lookup"><span data-stu-id="0736f-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0736f-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0736f-128">Request body</span></span>
<span data-ttu-id="0736f-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0736f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0736f-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="0736f-130">Response</span></span>

<span data-ttu-id="0736f-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0736f-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0736f-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0736f-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0736f-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0736f-133">Request</span></span>
<span data-ttu-id="0736f-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0736f-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_memberof"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/memberOf
```
##### <a name="response"></a><span data-ttu-id="0736f-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="0736f-135">Response</span></span>
<span data-ttu-id="0736f-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0736f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
