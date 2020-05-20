---
title: Listar oAuth2PermissionGrants
description: Recupere uma lista de objetos oauth2PermissionGrant, representando as autorizações de permissão delegadas.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 49c15d70947d991b6bb9b326d148836557ef8f93
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44288643"
---
# <a name="list-oauth2permissiongrants"></a><span data-ttu-id="bfbe4-103">List oauth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="bfbe4-103">List oauth2PermissionGrants</span></span>

<span data-ttu-id="bfbe4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bfbe4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bfbe4-105">Recupere uma lista de objetos [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) , representando as permissões delegadas que foram concedidas para que os aplicativos clientes acessem APIs em nome de usuários conectados.</span><span class="sxs-lookup"><span data-stu-id="bfbe4-105">Retrieve a list of [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) objects, representing delegated permissions which have been granted for client applications to access APIs on behalf of signed-in users.</span></span>

## <a name="permissions"></a><span data-ttu-id="bfbe4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="bfbe4-106">Permissions</span></span>

<span data-ttu-id="bfbe4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bfbe4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bfbe4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bfbe4-109">Permission type</span></span>      | <span data-ttu-id="bfbe4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bfbe4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bfbe4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bfbe4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bfbe4-112">Directory. Read. All, DelegatedPermissionGrant. ReadWrite. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="bfbe4-112">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="bfbe4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bfbe4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bfbe4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bfbe4-114">Not supported.</span></span>    |
|<span data-ttu-id="bfbe4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bfbe4-115">Application</span></span> | <span data-ttu-id="bfbe4-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bfbe4-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bfbe4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bfbe4-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /oauth2PermissionGrants
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bfbe4-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="bfbe4-118">Optional query parameters</span></span>

<span data-ttu-id="bfbe4-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="bfbe4-119">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bfbe4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bfbe4-120">Request headers</span></span>

| <span data-ttu-id="bfbe4-121">Nome</span><span class="sxs-lookup"><span data-stu-id="bfbe4-121">Name</span></span> | <span data-ttu-id="bfbe4-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="bfbe4-122">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="bfbe4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="bfbe4-123">Authorization</span></span>  | <span data-ttu-id="bfbe4-124">string</span><span class="sxs-lookup"><span data-stu-id="bfbe4-124">string</span></span>  | <span data-ttu-id="bfbe4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bfbe4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bfbe4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bfbe4-127">Request body</span></span>

<span data-ttu-id="bfbe4-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bfbe4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bfbe4-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="bfbe4-129">Response</span></span>

<span data-ttu-id="bfbe4-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bfbe4-130">If successful, this method returns a `200 OK` response code and collection of [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bfbe4-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bfbe4-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="bfbe4-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bfbe4-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_oauth2permissiongrants"
}-->

```http
GET https://graph.microsoft.com/v1.0/oauth2PermissionGrants
```

### <a name="response"></a><span data-ttu-id="bfbe4-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="bfbe4-133">Response</span></span>

> <span data-ttu-id="bfbe4-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bfbe4-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 259

{
  "value": [
    {
      "id": "id-value",
      "clientId": "clientId-value",
      "consentType": "consentType-value",
      "principalId": "principalId-value",
      "resourceId": "resourceId-value",
      "scope": "scope-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List oauth2PermissionGrants",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
