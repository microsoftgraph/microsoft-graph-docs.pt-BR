---
title: A lista exclui coleção de permissionGrantPolicy
description: Recupere uma lista de conjuntos de condição que descrevem condições sob as quais um evento de concessão de permissão é excluído em uma política de concessão de permissão.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: bc9b6d655f9040cd34228f5d34155ad7b9bef33b
ms.sourcegitcommit: 6201b3a5646f640f25a68ab033eca9eb60ccd05e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377166"
---
# <a name="list-excludes-collection-of-permissiongrantpolicy"></a><span data-ttu-id="918e6-103">A lista exclui coleção de permissionGrantPolicy</span><span class="sxs-lookup"><span data-stu-id="918e6-103">List excludes collection of permissionGrantPolicy</span></span>

<span data-ttu-id="918e6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="918e6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="918e6-105">Recupere os conjuntos de condição que são *excluídos* em um [permissionGrantPolicy](../resources/permissiongrantpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="918e6-105">Retrieve the condition sets which are *excluded* in a [permissionGrantPolicy](../resources/permissiongrantpolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="918e6-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="918e6-106">Permissions</span></span>

<span data-ttu-id="918e6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="918e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="918e6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="918e6-109">Permission type</span></span>      | <span data-ttu-id="918e6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="918e6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="918e6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="918e6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="918e6-112">Policy. Read. PermissionGrant, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="918e6-112">Policy.Read.PermissionGrant, Directory.Read.All</span></span> |
|<span data-ttu-id="918e6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="918e6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="918e6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="918e6-114">Not supported.</span></span>    |
|<span data-ttu-id="918e6-115">Application</span><span class="sxs-lookup"><span data-stu-id="918e6-115">Application</span></span> | <span data-ttu-id="918e6-116">Policy. Read. PermissionGrant, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="918e6-116">Policy.Read.PermissionGrant, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="918e6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="918e6-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /policies/permissionGrantPolicies/{id}/excludes
```

## <a name="optional-query-parameters"></a><span data-ttu-id="918e6-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="918e6-118">Optional query parameters</span></span>

<span data-ttu-id="918e6-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="918e6-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="918e6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="918e6-120">Request headers</span></span>

| <span data-ttu-id="918e6-121">Nome</span><span class="sxs-lookup"><span data-stu-id="918e6-121">Name</span></span>           | <span data-ttu-id="918e6-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="918e6-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="918e6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="918e6-123">Authorization</span></span>  | <span data-ttu-id="918e6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="918e6-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="918e6-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="918e6-126">Request body</span></span>

<span data-ttu-id="918e6-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="918e6-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="918e6-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="918e6-128">Response</span></span>

<span data-ttu-id="918e6-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="918e6-129">If successful, this method returns a `200 OK` response code and a collection of [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="918e6-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="918e6-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="918e6-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="918e6-131">Request</span></span>

<span data-ttu-id="918e6-132">Veja a seguir um exemplo da solicitação para recuperar os conjuntos de condições de **exclusão** da política de concessão de permissão interna `microsoft-application-admin` .</span><span class="sxs-lookup"><span data-stu-id="918e6-132">The following is an example of the request to retrieve the **excludes** condition sets of the built-on permission grant policy `microsoft-application-admin`.</span></span> <span data-ttu-id="918e6-133">Essa política de concessão de permissão inclui todas as permissões delegadas e todas as permissões de aplicativo, excluindo permissões de aplicativo para o Microsoft Graph e permissões de aplicativo do Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="918e6-133">This permission grant policy includes all delegated permissions, and all application permissions excluding application permissions for Microsoft Graph and application permissions for Azure AD Graph.</span></span>


<!-- {
  "blockType": "request",
  "name": "permissiongrantpolicy_get_excludes"
}-->

```http
GET https://graph.microsoft.com/v1.0/policies/permissionGrantPolicies/microsoft-application-admin/excludes
```

### <a name="response"></a><span data-ttu-id="918e6-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="918e6-134">Response</span></span>

<span data-ttu-id="918e6-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="918e6-135">The following is an example of the response.</span></span>

> <span data-ttu-id="918e6-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="918e6-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permissionGrantConditionSet",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "c85b029f-4abf-47d8-ae61-d2a38299033a",
      "permissionClassification": "all",
      "permissionType": "application",
      "resourceApplication": "00000003-0000-0000-c000-000000000000",
      "permissions": [ "all" ],
      "clientApplicationIds": [ "all" ],
      "clientApplicationTenantIds": [ "all" ],
      "clientApplicationPublisherIds": [ "all" ],
      "clientApplicationsFromVerifiedPublisherOnly": false
    },
    {
      "id": "2a1fbb36-9d9a-42d8-8804-de2aa45aca80",
      "permissionClassification": "all",
      "permissionType": "application",
      "resourceApplication": "00000002-0000-0000-c000-000000000000",
      "permissions": [ "all" ],
      "clientApplicationIds": [ "all" ],
      "clientApplicationTenantIds": [ "all" ],
      "clientApplicationPublisherIds": [ "all" ],
      "clientApplicationsFromVerifiedPublisherOnly": false
    }
  ]
}
```
