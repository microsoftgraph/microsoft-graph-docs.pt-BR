---
title: Membro transitivo do usuário de lista
description: Obtenha os grupos, funções de diretório e unidades administrativas que o usuário é membro do. Essa solicitação API é transitiva e também retornará todos os grupos que o usuário é membro de aninhados.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b0681196b994e9a0c88a2b2d05e25e3166a5242f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528862"
---
# <a name="list-user-transitive-memberof"></a><span data-ttu-id="9b0a0-104">Membro transitivo do usuário de lista</span><span class="sxs-lookup"><span data-stu-id="9b0a0-104">List user transitive memberOf</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9b0a0-105">Obtenha os grupos, funções de diretório e unidades administrativas que o usuário é membro do.</span><span class="sxs-lookup"><span data-stu-id="9b0a0-105">Get groups, directory roles and administrative units that the user is a member of.</span></span> <span data-ttu-id="9b0a0-106">Essa solicitação API é transitiva e também retornará todos os grupos que o usuário é membro de aninhados.</span><span class="sxs-lookup"><span data-stu-id="9b0a0-106">This API request is transitive, and will also return all groups the user is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="9b0a0-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="9b0a0-107">Permissions</span></span>

<span data-ttu-id="9b0a0-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b0a0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b0a0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9b0a0-110">Permission type</span></span>      | <span data-ttu-id="9b0a0-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9b0a0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9b0a0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9b0a0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9b0a0-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9b0a0-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9b0a0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9b0a0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9b0a0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9b0a0-115">Not supported.</span></span>    |
|<span data-ttu-id="9b0a0-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9b0a0-116">Application</span></span> | <span data-ttu-id="9b0a0-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b0a0-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9b0a0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9b0a0-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{id | userPrincipalName}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9b0a0-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9b0a0-119">Optional query parameters</span></span>

<span data-ttu-id="9b0a0-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9b0a0-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9b0a0-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9b0a0-121">Request headers</span></span>

| <span data-ttu-id="9b0a0-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9b0a0-122">Header</span></span>       | <span data-ttu-id="9b0a0-123">Valor</span><span class="sxs-lookup"><span data-stu-id="9b0a0-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9b0a0-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="9b0a0-124">Authorization</span></span>  | <span data-ttu-id="9b0a0-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9b0a0-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9b0a0-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9b0a0-127">Accept</span></span>  | <span data-ttu-id="9b0a0-128">application/json</span><span class="sxs-lookup"><span data-stu-id="9b0a0-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b0a0-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9b0a0-129">Request body</span></span>

<span data-ttu-id="9b0a0-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9b0a0-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9b0a0-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b0a0-131">Response</span></span>

<span data-ttu-id="9b0a0-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9b0a0-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b0a0-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9b0a0-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="9b0a0-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9b0a0-134">Request</span></span>

<span data-ttu-id="9b0a0-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9b0a0-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_transitivememberof"
}-->

```http
GET https://graph.microsoft.com/beta/me/transitiveMemberOf
```

### <a name="response"></a><span data-ttu-id="9b0a0-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b0a0-136">Response</span></span>

<span data-ttu-id="9b0a0-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9b0a0-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "List transitiveMsemberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list-transitivememberof.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
