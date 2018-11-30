---
title: Membro de usuário da lista
description: Obtenha os grupos, funções de diretório e unidades administrativas que o usuário é um membro direto. Esta operação não é transitiva.
ms.openlocfilehash: 0d22189f35e41798929c10d63219a5f5688c42c9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037227"
---
# <a name="list-user-memberof"></a><span data-ttu-id="5f49f-104">Membro de usuário da lista</span><span class="sxs-lookup"><span data-stu-id="5f49f-104">List user memberOf</span></span>

> <span data-ttu-id="5f49f-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5f49f-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5f49f-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5f49f-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5f49f-107">Obtenha os grupos, funções de diretório e unidades administrativas que o usuário é um membro direto.</span><span class="sxs-lookup"><span data-stu-id="5f49f-107">Get groups, directory roles and administrative units that the user is a direct member of.</span></span> <span data-ttu-id="5f49f-108">Esta operação não é transitiva.</span><span class="sxs-lookup"><span data-stu-id="5f49f-108">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="5f49f-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="5f49f-109">Permissions</span></span>

<span data-ttu-id="5f49f-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f49f-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f49f-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5f49f-112">Permission type</span></span>      | <span data-ttu-id="5f49f-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5f49f-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5f49f-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5f49f-114">Delegated (work or school account)</span></span> | <span data-ttu-id="5f49f-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5f49f-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5f49f-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5f49f-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5f49f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5f49f-117">Not supported.</span></span>    |
|<span data-ttu-id="5f49f-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5f49f-118">Application</span></span> | <span data-ttu-id="5f49f-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f49f-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5f49f-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5f49f-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5f49f-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5f49f-121">Optional query parameters</span></span>

<span data-ttu-id="5f49f-122">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5f49f-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="5f49f-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5f49f-123">Request headers</span></span>
| <span data-ttu-id="5f49f-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5f49f-124">Header</span></span>       | <span data-ttu-id="5f49f-125">Valor</span><span class="sxs-lookup"><span data-stu-id="5f49f-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5f49f-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="5f49f-126">Authorization</span></span>  | <span data-ttu-id="5f49f-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5f49f-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5f49f-129">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5f49f-129">Accept</span></span>  | <span data-ttu-id="5f49f-130">application/json</span><span class="sxs-lookup"><span data-stu-id="5f49f-130">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f49f-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5f49f-131">Request body</span></span>

<span data-ttu-id="5f49f-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5f49f-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5f49f-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f49f-133">Response</span></span>

<span data-ttu-id="5f49f-134">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5f49f-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5f49f-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5f49f-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="5f49f-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5f49f-136">Request</span></span>

<span data-ttu-id="5f49f-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5f49f-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_user_memberof"
}-->
```http
GET https://graph.microsoft.com/beta/me/memberOf
```

### <a name="response"></a><span data-ttu-id="5f49f-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f49f-138">Response</span></span>

<span data-ttu-id="5f49f-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5f49f-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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