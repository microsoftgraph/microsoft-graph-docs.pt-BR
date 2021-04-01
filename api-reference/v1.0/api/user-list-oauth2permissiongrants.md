---
title: Lista oauth2PermissionGrants
description: Recuperar uma lista de objetos oAuth2PermissionGrant, representando concessões de permissão delegadas.
localization_priority: Priority
doc_type: apiPageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 2960a27b59fc6dc0af4267ceee9d87772102bbfa
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473952"
---
# <a name="list-oauth2permissiongrants"></a><span data-ttu-id="e96ac-103">Lista oauth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="e96ac-103">List oauth2PermissionGrants</span></span>

<span data-ttu-id="e96ac-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e96ac-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e96ac-105">Recuperar uma lista de entidades [oAuth2PermissionGrant](../resources/oAuth2PermissionGrant.md), que representam permissões delegadas concedidas para habilitar um aplicativo cliente para acessar uma API em nome do usuário.</span><span class="sxs-lookup"><span data-stu-id="e96ac-105">Retrieve a list of [oAuth2PermissionGrant](../resources/oAuth2PermissionGrant.md) entities, which represent delegated permissions granted to enable a client application to access an API on behalf of the user.</span></span>

> [!NOTE]
> <span data-ttu-id="e96ac-106">Consultar as concessões de permissão delegada para um usuário só retornará permissões delegadas para o usuário específico.</span><span class="sxs-lookup"><span data-stu-id="e96ac-106">Querying the delegated permission grants for a user will only return delegated permissions grants that are specifically for the given user.</span></span> <span data-ttu-id="e96ac-107">As permissões delegadas concedidas em nome de todos os usuários da organização _não_ são incluídas na resposta.</span><span class="sxs-lookup"><span data-stu-id="e96ac-107">Delegated permissions granted on behalf of all users in the organization are _not_ included in the response.</span></span>

## <a name="permissions"></a><span data-ttu-id="e96ac-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="e96ac-108">Permissions</span></span>

<span data-ttu-id="e96ac-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e96ac-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e96ac-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e96ac-111">Permission type</span></span>      | <span data-ttu-id="e96ac-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e96ac-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e96ac-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e96ac-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e96ac-114">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e96ac-114">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="e96ac-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e96ac-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e96ac-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e96ac-116">Not supported.</span></span>    |
|<span data-ttu-id="e96ac-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e96ac-117">Application</span></span> | <span data-ttu-id="e96ac-118">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e96ac-118">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e96ac-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e96ac-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/oauth2PermissionGrants
GET /users/{id | userPrincipalName}/oauth2PermissionGrants
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e96ac-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e96ac-120">Optional query parameters</span></span>

<span data-ttu-id="e96ac-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e96ac-121">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e96ac-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e96ac-122">Request headers</span></span>

| <span data-ttu-id="e96ac-123">Nome</span><span class="sxs-lookup"><span data-stu-id="e96ac-123">Name</span></span>           | <span data-ttu-id="e96ac-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="e96ac-124">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="e96ac-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="e96ac-125">Authorization</span></span>  | <span data-ttu-id="e96ac-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e96ac-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e96ac-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e96ac-128">Request body</span></span>

<span data-ttu-id="e96ac-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e96ac-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e96ac-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="e96ac-130">Response</span></span>

<span data-ttu-id="e96ac-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e96ac-131">If successful, this method returns a `200 OK` response code and a collection of [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e96ac-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e96ac-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e96ac-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e96ac-133">Request</span></span>

<span data-ttu-id="e96ac-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e96ac-134">Here is an example of the request.</span></span>


<!-- {
  "blockType": "request",
  "name": "get_user_oAuth2PermissionGrants"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/7d54cb02-aaa3-4016-9f9c-a4b49422dd9b/oauth2PermissionGrants
```

### <a name="response"></a><span data-ttu-id="e96ac-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e96ac-135">Response</span></span>

<span data-ttu-id="e96ac-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e96ac-136">Here is an example of the response.</span></span> 

> <span data-ttu-id="e96ac-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e96ac-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "clientId": "85477313-ea43-4c7d-b8a4-54fed35d0b60",
      "consentType": "Principal",
      "id": "E3NHhUPqfUy4pFT-010LYFo5-ycA-_5Fhl7nHbaJ7qACy1R9o6oWQJ-cpLSUIt2b",
      "principalId": "7d54cb02-aaa3-4016-9f9c-a4b49422dd9b",
      "resourceId": "27fb395a-fb00-45fe-865e-e71db689eea0",
      "scope": " Contacts.ReadWrite openid profile"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List oAuth2PermissionGrants",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

