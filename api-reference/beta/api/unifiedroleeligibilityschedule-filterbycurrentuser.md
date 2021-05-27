---
title: 'unifiedRoleEligibilitySchedule: filterByCurrentUser'
description: Obter uma lista dos objetos unifiedRoleEligibilitySchedule e suas propriedades filtradas por uma entidade de usuário específica
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 30221a7766703a4e16efca7b590512ca48bf1720
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52679929"
---
# <a name="unifiedroleeligibilityschedule-filterbycurrentuser"></a><span data-ttu-id="17643-103">unifiedRoleEligibilitySchedule: filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="17643-103">unifiedRoleEligibilitySchedule: filterByCurrentUser</span></span>
<span data-ttu-id="17643-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="17643-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="17643-105">Obter uma lista dos [objetos unifiedRoleEligibilitySchedule](../resources/unifiedRoleEligibilitySchedule.md) e suas propriedades associadas a um objeto principal específico.</span><span class="sxs-lookup"><span data-stu-id="17643-105">Get a list of the [unifiedRoleEligibilitySchedule](../resources/unifiedRoleEligibilitySchedule.md) objects and their properties associated with a particular principal object.</span></span>

## <a name="permissions"></a><span data-ttu-id="17643-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="17643-106">Permissions</span></span>
<span data-ttu-id="17643-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17643-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17643-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="17643-109">Permission type</span></span>|<span data-ttu-id="17643-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="17643-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="17643-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="17643-111">Delegated (work or school account)</span></span>|<span data-ttu-id="17643-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="17643-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="17643-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="17643-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="17643-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="17643-114">Not supported</span></span>|
|<span data-ttu-id="17643-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="17643-115">Application</span></span>|<span data-ttu-id="17643-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="17643-116">PrivilegedAccess.Read.AzureAD</span></span>|

## <a name="http-request"></a><span data-ttu-id="17643-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="17643-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET roleManagement/directory/roleEligibilitySchedules/filterByCurrentUser
```

## <a name="query-parameters"></a><span data-ttu-id="17643-118">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="17643-118">Query parameters</span></span>
<span data-ttu-id="17643-119">A tabela a seguir mostra os parâmetros que podem ser usados com esse método.</span><span class="sxs-lookup"><span data-stu-id="17643-119">The following table shows the parameters that can be used with this method.</span></span>

|<span data-ttu-id="17643-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="17643-120">Parameter</span></span>|<span data-ttu-id="17643-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="17643-121">Type</span></span>|<span data-ttu-id="17643-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="17643-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17643-123">on</span><span class="sxs-lookup"><span data-stu-id="17643-123">on</span></span>|<span data-ttu-id="17643-124">roleEligibilityScheduleFilterByCurrentUserOptions</span><span class="sxs-lookup"><span data-stu-id="17643-124">roleEligibilityScheduleFilterByCurrentUserOptions</span></span>|<span data-ttu-id="17643-125">ID do usuário atual.</span><span class="sxs-lookup"><span data-stu-id="17643-125">Id of the current user.</span></span>|


## <a name="request-headers"></a><span data-ttu-id="17643-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="17643-126">Request headers</span></span>
|<span data-ttu-id="17643-127">Nome</span><span class="sxs-lookup"><span data-stu-id="17643-127">Name</span></span>|<span data-ttu-id="17643-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="17643-128">Description</span></span>|
|:---|:---|
|<span data-ttu-id="17643-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="17643-129">Authorization</span></span>|<span data-ttu-id="17643-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="17643-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="17643-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="17643-132">Request body</span></span>
<span data-ttu-id="17643-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="17643-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="17643-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="17643-134">Response</span></span>

<span data-ttu-id="17643-135">Se tiver êxito, este método retornará um código de resposta e uma coleção `200 OK` [unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="17643-135">If successful, this method returns a `200 OK` response code and a [unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="17643-136">Exemplos</span><span class="sxs-lookup"><span data-stu-id="17643-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="17643-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="17643-137">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "unifiedroleeligibilityschedule_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleEligibilitySchedules/filterByCurrentUser(on='eb18c026-c026-eb18-26c0-18eb26c018eb')
```


### <a name="response"></a><span data-ttu-id="17643-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="17643-138">Response</span></span>
<span data-ttu-id="17643-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="17643-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleEligibilitySchedule)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "eb18c026-c026-eb18-26c0-18eb26c018eb",
      "principalId": "eb18c026-c026-eb18-26c0-18eb26c018eb",
      "roleDefinitionId": "eb18c026-c026-eb18-26c0-18eb26c018eb",
      "directoryScopeId": "eb18c026-c026-eb18-26c0-18eb26c018eb",
      "appScopeId": "eb18c026-c026-eb18-26c0-18eb26c018eb",
      "createdUsing": "eb18c026-c026-eb18-26c0-18eb26c018eb",
      "createdDateTime": "2020-09-09T21:35:27.91Z",
      "modifiedDateTime": "2020-09-09T21:35:27.91Z",
      "status": "Provisioned",
      "scheduleInfo": {
        "@odata.type": "microsoft.graph.requestSchedule"
      },
      "memberType": "direct"
    }
  ]
}
```

