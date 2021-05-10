---
title: Listar unifiedRoleAssignmentScheduleRequests
description: Obter uma lista dos objetos unifiedRoleAssignmentScheduleRequest e suas propriedades.
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 29e3c448dc96cfc1dfacad1a3eece2dbe5220688
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299084"
---
# <a name="list-unifiedroleassignmentschedulerequests"></a><span data-ttu-id="cb1b2-103">Listar unifiedRoleAssignmentScheduleRequests</span><span class="sxs-lookup"><span data-stu-id="cb1b2-103">List unifiedRoleAssignmentScheduleRequests</span></span>

<span data-ttu-id="cb1b2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb1b2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb1b2-105">Obter uma lista dos [objetos unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="cb1b2-105">Get a list of the [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="cb1b2-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="cb1b2-106">Permissions</span></span>

<span data-ttu-id="cb1b2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb1b2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cb1b2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cb1b2-109">Permission type</span></span>                        | <span data-ttu-id="cb1b2-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cb1b2-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="cb1b2-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cb1b2-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="cb1b2-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="cb1b2-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>          |
| <span data-ttu-id="cb1b2-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cb1b2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cb1b2-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="cb1b2-114">Not supported</span></span>                               |
| <span data-ttu-id="cb1b2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cb1b2-115">Application</span></span>                            | <span data-ttu-id="cb1b2-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="cb1b2-116">PrivilegedAccess.Read.AzureAD</span></span>               |

## <a name="http-request"></a><span data-ttu-id="cb1b2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cb1b2-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
GET /roleManagement/directory/roleAssignmentScheduleRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cb1b2-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="cb1b2-118">Optional query parameters</span></span>

<span data-ttu-id="cb1b2-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="cb1b2-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="cb1b2-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="cb1b2-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="cb1b2-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cb1b2-121">Request headers</span></span>

| <span data-ttu-id="cb1b2-122">Nome</span><span class="sxs-lookup"><span data-stu-id="cb1b2-122">Name</span></span>          | <span data-ttu-id="cb1b2-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb1b2-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="cb1b2-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="cb1b2-124">Authorization</span></span> | <span data-ttu-id="cb1b2-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cb1b2-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cb1b2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cb1b2-127">Request body</span></span>

<span data-ttu-id="cb1b2-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cb1b2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cb1b2-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb1b2-129">Response</span></span>

<span data-ttu-id="cb1b2-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cb1b2-130">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cb1b2-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="cb1b2-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cb1b2-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cb1b2-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_unifiedroleassignmentschedulerequest"
}
-->

```http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignmentScheduleRequests
```

### <a name="response"></a><span data-ttu-id="cb1b2-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb1b2-133">Response</span></span>

<span data-ttu-id="cb1b2-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="cb1b2-134">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleAssignmentScheduleRequest)"
}
-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "c13ee236-e236-c13e-36e2-3ec136e23ec1",
      "action": "String",
      "principalId": "String",
      "roleDefinitionId": "String",
      "directoryScopeId": "String",
      "appScopeId": "String",
      "isValidationOnly": "Boolean",
      "targetScheduleId": "String",
      "justification": "String",
      "scheduleInfo": {
        "@odata.type": "microsoft.graph.requestSchedule"
      },
      "ticketInfo": {
        "@odata.type": "microsoft.graph.ticketInfo"
      }
    }
  ]
}
```
