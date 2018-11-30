---
title: Membro do lista servicePrincipal transitivo
description: Obtenha os grupos e funções de diretório que esse serviço principal é um membro de. Essa operação é transitiva e incluirá todos os grupos que esse serviço principal é um membro aninhado do.
ms.openlocfilehash: e08185e15f583173e585bf392f628a8d9c0800eb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037833"
---
# <a name="list-serviceprincipal-transitive-memberof"></a><span data-ttu-id="6885c-104">Membro do lista servicePrincipal transitivo</span><span class="sxs-lookup"><span data-stu-id="6885c-104">List servicePrincipal transitive memberOf</span></span>

> <span data-ttu-id="6885c-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6885c-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6885c-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6885c-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6885c-107">Obtenha os grupos e funções de diretório que esse serviço principal é um membro de.</span><span class="sxs-lookup"><span data-stu-id="6885c-107">Get the groups and directory roles that this service principal is a member of.</span></span> <span data-ttu-id="6885c-108">Essa operação é transitiva e incluirá todos os grupos que esse serviço principal é um membro aninhado do.</span><span class="sxs-lookup"><span data-stu-id="6885c-108">This operation is transitive and will include all groups that this service principal is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="6885c-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="6885c-109">Permissions</span></span>
<span data-ttu-id="6885c-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6885c-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6885c-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6885c-112">Permission type</span></span>      | <span data-ttu-id="6885c-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6885c-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6885c-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6885c-114">Delegated (work or school account)</span></span> | <span data-ttu-id="6885c-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6885c-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6885c-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6885c-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6885c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6885c-117">Not supported.</span></span>    |
|<span data-ttu-id="6885c-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6885c-118">Application</span></span> | <span data-ttu-id="6885c-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6885c-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6885c-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6885c-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6885c-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6885c-121">Optional query parameters</span></span>
<span data-ttu-id="6885c-122">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6885c-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6885c-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6885c-123">Request headers</span></span>
| <span data-ttu-id="6885c-124">Nome</span><span class="sxs-lookup"><span data-stu-id="6885c-124">Name</span></span>       | <span data-ttu-id="6885c-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="6885c-125">Type</span></span> | <span data-ttu-id="6885c-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="6885c-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6885c-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="6885c-127">Authorization</span></span>  | <span data-ttu-id="6885c-128">string</span><span class="sxs-lookup"><span data-stu-id="6885c-128">string</span></span>  | <span data-ttu-id="6885c-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6885c-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6885c-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6885c-131">Request body</span></span>
<span data-ttu-id="6885c-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6885c-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6885c-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="6885c-133">Response</span></span>

<span data-ttu-id="6885c-134">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6885c-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6885c-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6885c-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="6885c-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6885c-136">Request</span></span>

<span data-ttu-id="6885c-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6885c-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal_memberof"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/memberOf
```

### <a name="response"></a><span data-ttu-id="6885c-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="6885c-138">Response</span></span>

<span data-ttu-id="6885c-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6885c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List servicePrincipal memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->