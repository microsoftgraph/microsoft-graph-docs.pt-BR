---
title: 'accessPackageAssignment: filterByCurrentUser'
description: Recupere uma lista de objetos accesspackageassignment filtrados no usuário de entrada.
localization_priority: Normal
author: sbounouh
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 72164fb7f9567d1a1c1b79316f19bbd304fabae3
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299010"
---
# <a name="accesspackageassignment-filterbycurrentuser"></a><span data-ttu-id="7fa3a-103">accessPackageAssignment: filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="7fa3a-103">accessPackageAssignment: filterByCurrentUser</span></span>
<span data-ttu-id="7fa3a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7fa3a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7fa3a-105">No [Azure AD Entitlement Management](../resources/entitlementmanagement-root.md), recupere uma lista de objetos [accessPackageAssignment](../resources/accesspackageassignment.md) filtrados no usuário de entrada.</span><span class="sxs-lookup"><span data-stu-id="7fa3a-105">In [Azure AD Entitlement Management](../resources/entitlementmanagement-root.md), retrieve a list of [accessPackageAssignment](../resources/accesspackageassignment.md) objects filtered on the signed-in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="7fa3a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7fa3a-106">Permissions</span></span>
<span data-ttu-id="7fa3a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7fa3a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7fa3a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7fa3a-109">Permission type</span></span>|<span data-ttu-id="7fa3a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7fa3a-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7fa3a-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7fa3a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7fa3a-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7fa3a-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span>|
|<span data-ttu-id="7fa3a-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7fa3a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7fa3a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7fa3a-114">Not supported.</span></span>|
|<span data-ttu-id="7fa3a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7fa3a-115">Application</span></span>|<span data-ttu-id="7fa3a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7fa3a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7fa3a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7fa3a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/entitlementManagement/accessPackageAssignments/filterByCurrentUser
```

## <a name="function-parameters"></a><span data-ttu-id="7fa3a-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="7fa3a-118">Function parameters</span></span>
<span data-ttu-id="7fa3a-119">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="7fa3a-119">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="7fa3a-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="7fa3a-120">Parameter</span></span>|<span data-ttu-id="7fa3a-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="7fa3a-121">Type</span></span>|<span data-ttu-id="7fa3a-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="7fa3a-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7fa3a-123">on</span><span class="sxs-lookup"><span data-stu-id="7fa3a-123">on</span></span>|[<span data-ttu-id="7fa3a-124">accessPackageAssignmentFilterByCurrentUserOptions</span><span class="sxs-lookup"><span data-stu-id="7fa3a-124">accessPackageAssignmentFilterByCurrentUserOptions</span></span>](../resources/accesspackageassignment-accesspackageassignmentfilterbycurrentuseroptions.md)|<span data-ttu-id="7fa3a-125">A lista de opções de usuário atuais que podem ser usadas para filtrar na lista de atribuições do pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="7fa3a-125">The list of current user options that can be used to filter on the access package assignments list.</span></span>|

- <span data-ttu-id="7fa3a-126">`target` é usado para obter os `accessPackageAssignment` objetos em que o usuário inscreva é o destino.</span><span class="sxs-lookup"><span data-stu-id="7fa3a-126">`target` is used to get the `accessPackageAssignment` objects where the signed-in user is the target.</span></span> <span data-ttu-id="7fa3a-127">A lista resultante inclui todas as atribuições, atuais e expiradas, para o chamador em todos os catálogos e pacotes de acesso.</span><span class="sxs-lookup"><span data-stu-id="7fa3a-127">The resulting list includes all of the assignments, current and expired, for the caller across all catalogs and access packages.</span></span>

- <span data-ttu-id="7fa3a-128">`createdBy` é usado para obter `accessPackageAssignment` os objetos criados pelo usuário in-locar.</span><span class="sxs-lookup"><span data-stu-id="7fa3a-128">`createdBy` is used to get the `accessPackageAssignment` objects created by the signed-in user.</span></span> <span data-ttu-id="7fa3a-129">A lista resultante inclui todas as atribuições que o chamador criou para si ou em nome de outras pessoas, como no caso de atribuição direta do administrador, em todos os catálogos e pacotes de acesso.</span><span class="sxs-lookup"><span data-stu-id="7fa3a-129">The resulting list includes all of the assignments that the caller created for themselves or on behalf of others, such as in case of admin direct assignment, across all catalogs and access packages.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7fa3a-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7fa3a-130">Request headers</span></span>
|<span data-ttu-id="7fa3a-131">Nome</span><span class="sxs-lookup"><span data-stu-id="7fa3a-131">Name</span></span>|<span data-ttu-id="7fa3a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="7fa3a-132">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7fa3a-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="7fa3a-133">Authorization</span></span>|<span data-ttu-id="7fa3a-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7fa3a-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7fa3a-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7fa3a-136">Request body</span></span>
<span data-ttu-id="7fa3a-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7fa3a-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7fa3a-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="7fa3a-138">Response</span></span>

<span data-ttu-id="7fa3a-139">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` [coleção accessPackageAssignment](../resources/accesspackageassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7fa3a-139">If successful, this method returns a `200 OK` response code and an [accessPackageAssignment](../resources/accesspackageassignment.md) collection in the response body.</span></span>

<span data-ttu-id="7fa3a-140">Quando um conjunto de resultados abrange várias páginas, o Microsoft Graph retorna essa página com uma propriedade na resposta que contém uma URL para `@odata.nextLink` a próxima página de resultados.</span><span class="sxs-lookup"><span data-stu-id="7fa3a-140">When a result set spans multiple pages, Microsoft Graph returns that page with an `@odata.nextLink` property in the response that contains a URL to the next page of results.</span></span> <span data-ttu-id="7fa3a-141">Se essa propriedade estiver presente, continue fazendo solicitações adicionais com a URL em `@odata.nextLink` cada resposta, até que todos os resultados sejam retornados.</span><span class="sxs-lookup"><span data-stu-id="7fa3a-141">If that property is present, continue making additional requests with the `@odata.nextLink` URL in each response, until all the results are returned.</span></span> <span data-ttu-id="7fa3a-142">Para obter mais informações, [consulte paging Microsoft Graph data in your app](/graph/paging.md).</span><span class="sxs-lookup"><span data-stu-id="7fa3a-142">For more information, see [paging Microsoft Graph data in your app](/graph/paging.md).</span></span>

## <a name="examples"></a><span data-ttu-id="7fa3a-143">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7fa3a-143">Examples</span></span>

<span data-ttu-id="7fa3a-144">O exemplo a seguir obtém o status das atribuições de pacote de acesso direcionadas para o usuário de entrada.</span><span class="sxs-lookup"><span data-stu-id="7fa3a-144">The following example gets the status of access package assignments targeted for the signed-in user.</span></span>

### <a name="request"></a><span data-ttu-id="7fa3a-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7fa3a-145">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "accesspackageassignment_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignments/filterByCurrentUser(on='target')
```


### <a name="response"></a><span data-ttu-id="7fa3a-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="7fa3a-146">Response</span></span>
> <span data-ttu-id="7fa3a-147">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7fa3a-147">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.accessPackageAssignment)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
        {
            "@odata.type": "#microsoft.graph.accessPackageAssignment",
            "id": "5521fb4f-6a6c-410a-9191-461a65fd39d4",
            "catalogId": "34cfe9a8-88bc-4c82-b3d8-6b77d7035c33",
            "accessPackageId": "ca6992f8-e413-49a1-9619-c9819f4f73e0",
            "assignmentPolicyId": "7c6e6874-789e-4f11-b351-cc7b5883deef",
            "targetId": "2cb14f51-0108-41d8-89da-cd0e05e2c988",
            "assignmentStatus": "Delivered",
            "assignmentState": "Delivered",
            "isExtended": false,
            "expiredDateTime": null,
            "schedule": {
                "startDateTime": "2021-01-19T20:02:36.013Z",
                "recurrence": null,
                "expiration": {
                    "endDateTime": "2022-01-19T20:02:36.013Z",
                    "duration": null,
                    "type": "afterDateTime"
                }
            }
        }
  ]
}

```

