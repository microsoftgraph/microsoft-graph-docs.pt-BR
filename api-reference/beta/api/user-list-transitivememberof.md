---
title: Membro transitivo do usuário de lista
description: Obtenha os grupos, funções de diretório e unidades administrativas que o usuário é membro do. Essa solicitação API é transitiva e também retornará todos os grupos que o usuário é membro de aninhados.
localization_priority: Normal
ms.openlocfilehash: eadb9722bc323ea056d015ac15c8aed975306eee
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27887910"
---
# <a name="list-user-transitive-memberof"></a><span data-ttu-id="3bb6b-104">Membro transitivo do usuário de lista</span><span class="sxs-lookup"><span data-stu-id="3bb6b-104">List user transitive memberOf</span></span>

> <span data-ttu-id="3bb6b-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3bb6b-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3bb6b-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3bb6b-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3bb6b-107">Obtenha os grupos, funções de diretório e unidades administrativas que o usuário é membro do.</span><span class="sxs-lookup"><span data-stu-id="3bb6b-107">Get groups, directory roles and administrative units that the user is a member of.</span></span> <span data-ttu-id="3bb6b-108">Essa solicitação API é transitiva e também retornará todos os grupos que o usuário é membro de aninhados.</span><span class="sxs-lookup"><span data-stu-id="3bb6b-108">This API request is transitive, and will also return all groups the user is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="3bb6b-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="3bb6b-109">Permissions</span></span>

<span data-ttu-id="3bb6b-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3bb6b-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3bb6b-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3bb6b-112">Permission type</span></span>      | <span data-ttu-id="3bb6b-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3bb6b-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3bb6b-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3bb6b-114">Delegated (work or school account)</span></span> | <span data-ttu-id="3bb6b-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3bb6b-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3bb6b-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3bb6b-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3bb6b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3bb6b-117">Not supported.</span></span>    |
|<span data-ttu-id="3bb6b-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3bb6b-118">Application</span></span> | <span data-ttu-id="3bb6b-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3bb6b-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3bb6b-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3bb6b-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{id | userPrincipalName}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3bb6b-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3bb6b-121">Optional query parameters</span></span>

<span data-ttu-id="3bb6b-122">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3bb6b-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3bb6b-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3bb6b-123">Request headers</span></span>

| <span data-ttu-id="3bb6b-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3bb6b-124">Header</span></span>       | <span data-ttu-id="3bb6b-125">Valor</span><span class="sxs-lookup"><span data-stu-id="3bb6b-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3bb6b-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="3bb6b-126">Authorization</span></span>  | <span data-ttu-id="3bb6b-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3bb6b-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3bb6b-129">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3bb6b-129">Accept</span></span>  | <span data-ttu-id="3bb6b-130">application/json</span><span class="sxs-lookup"><span data-stu-id="3bb6b-130">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3bb6b-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3bb6b-131">Request body</span></span>

<span data-ttu-id="3bb6b-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3bb6b-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3bb6b-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="3bb6b-133">Response</span></span>

<span data-ttu-id="3bb6b-134">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3bb6b-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3bb6b-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3bb6b-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="3bb6b-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3bb6b-136">Request</span></span>

<span data-ttu-id="3bb6b-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3bb6b-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_transitivememberof"
}-->

```http
GET https://graph.microsoft.com/beta/me/transitiveMemberOf
```

### <a name="response"></a><span data-ttu-id="3bb6b-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="3bb6b-138">Response</span></span>

<span data-ttu-id="3bb6b-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3bb6b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
  "description": "List transitiveMsemberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
