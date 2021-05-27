---
title: 'unifiedRoleEligibilityScheduleInstance: filterByCurrentUser'
description: Obter uma lista dos objetos unifiedRoleEligibilityScheduleInstance e suas propriedades filtradas por uma entidade de usuário específica
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 724933c90a7a404b360e19a76304ba1d99be25bb
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52679908"
---
# <a name="unifiedroleeligibilityscheduleinstance-filterbycurrentuser"></a><span data-ttu-id="b273a-103">unifiedRoleEligibilityScheduleInstance: filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="b273a-103">unifiedRoleEligibilityScheduleInstance: filterByCurrentUser</span></span>
<span data-ttu-id="b273a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b273a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b273a-105">Obter uma lista dos [objetos unifiedRoleEligibilityScheduleInstance](../resources/unifiedRoleEligibilityScheduleInstance.md) e suas propriedades associadas a um objeto principal específico.</span><span class="sxs-lookup"><span data-stu-id="b273a-105">Get a list of the [unifiedRoleEligibilityScheduleInstance](../resources/unifiedRoleEligibilityScheduleInstance.md) objects and their properties associated with a particular principal object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b273a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b273a-106">Permissions</span></span>
<span data-ttu-id="b273a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b273a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b273a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b273a-109">Permission type</span></span>|<span data-ttu-id="b273a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b273a-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b273a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b273a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b273a-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="b273a-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="b273a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b273a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b273a-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b273a-114">Not supported</span></span>|
|<span data-ttu-id="b273a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b273a-115">Application</span></span>|<span data-ttu-id="b273a-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="b273a-116">PrivilegedAccess.Read.AzureAD</span></span>|

## <a name="http-request"></a><span data-ttu-id="b273a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b273a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleEligibilityScheduleInstances/filterByCurrentUser
```

## <a name="query-parameters"></a><span data-ttu-id="b273a-118">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="b273a-118">Query parameters</span></span>
<span data-ttu-id="b273a-119">A tabela a seguir mostra os parâmetros de consulta que podem ser usados com esse método.</span><span class="sxs-lookup"><span data-stu-id="b273a-119">The following table shows the query parameters that can be used with this method.</span></span>

|<span data-ttu-id="b273a-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b273a-120">Parameter</span></span>|<span data-ttu-id="b273a-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="b273a-121">Type</span></span>|<span data-ttu-id="b273a-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="b273a-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b273a-123">on</span><span class="sxs-lookup"><span data-stu-id="b273a-123">on</span></span>|<span data-ttu-id="b273a-124">roleEligibilityScheduleInstanceFilterByCurrentUserOptions</span><span class="sxs-lookup"><span data-stu-id="b273a-124">roleEligibilityScheduleInstanceFilterByCurrentUserOptions</span></span>|<span data-ttu-id="b273a-125">ID do usuário atual.</span><span class="sxs-lookup"><span data-stu-id="b273a-125">Id of the current user.</span></span>|


## <a name="request-headers"></a><span data-ttu-id="b273a-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b273a-126">Request headers</span></span>
|<span data-ttu-id="b273a-127">Nome</span><span class="sxs-lookup"><span data-stu-id="b273a-127">Name</span></span>|<span data-ttu-id="b273a-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="b273a-128">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b273a-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="b273a-129">Authorization</span></span>|<span data-ttu-id="b273a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b273a-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b273a-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b273a-132">Request body</span></span>
<span data-ttu-id="b273a-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b273a-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b273a-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b273a-134">Response</span></span>

<span data-ttu-id="b273a-135">Se tiver êxito, este método retornará um código de resposta e uma coleção `200 OK` [unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b273a-135">If successful, this method returns a `200 OK` response code and a [unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b273a-136">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b273a-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b273a-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b273a-137">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "unifiedroleeligibilityscheduleinstance_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleEligibilityScheduleInstances/filterByCurrentUser(on='5cfd7709-7709-5cfd-0977-fd5c0977fd5c')
```


### <a name="response"></a><span data-ttu-id="b273a-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="b273a-138">Response</span></span>
<span data-ttu-id="b273a-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b273a-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleEligibilityScheduleInstance)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "5cfd7709-7709-5cfd-0977-fd5c0977fd5c",
      "principalId": "5cfd7709-7709-5cfd-0977-fd5c0977fd5c",
      "roleDefinitionId": "5cfd7709-7709-5cfd-0977-fd5c0977fd5c",
      "directoryScopeId": "5cfd7709-7709-5cfd-0977-fd5c0977fd5c",
      "appScopeId": "5cfd7709-7709-5cfd-0977-fd5c0977fd5c",
      "startDateTime": "2020-09-09T21:35:27.91Z",
      "endDateTime": "2020-09-09T21:35:27.91Z",
      "memberType": "direct",
      "roleEligibilityScheduleId": "5cfd7709-7709-5cfd-0977-fd5c0977fd5c"
    }
  ]
}
```

