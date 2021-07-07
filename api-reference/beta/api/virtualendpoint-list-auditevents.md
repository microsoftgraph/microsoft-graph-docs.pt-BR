---
title: Listar auditEvents
description: Obter uma lista dos objetos cloudPcAuditEvent e suas propriedades.
author: ecmadao
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 2a2694a2b854c9fbaba137506d925ba8cf4829d6
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2021
ms.locfileid: "53316563"
---
# <a name="list-auditevents"></a><span data-ttu-id="58d9c-103">Listar auditEvents</span><span class="sxs-lookup"><span data-stu-id="58d9c-103">List auditEvents</span></span>

<span data-ttu-id="58d9c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58d9c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="58d9c-105">Listar todos os [objetos cloudPcAuditEvent](../resources/cloudpcauditevent.md) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="58d9c-105">List all the [cloudPcAuditEvent](../resources/cloudpcauditevent.md) objects for the tenant.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="58d9c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="58d9c-106">Permissions</span></span>

<span data-ttu-id="58d9c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58d9c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58d9c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="58d9c-109">Permission type</span></span>|<span data-ttu-id="58d9c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="58d9c-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58d9c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="58d9c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="58d9c-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58d9c-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="58d9c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="58d9c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58d9c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="58d9c-114">Not supported.</span></span>|
|<span data-ttu-id="58d9c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="58d9c-115">Application</span></span>|<span data-ttu-id="58d9c-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58d9c-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="58d9c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="58d9c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/auditEvents
```

## <a name="optional-query-parameters"></a><span data-ttu-id="58d9c-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="58d9c-118">Optional query parameters</span></span>

<span data-ttu-id="58d9c-119">Este método oferece `$skiptoken` suporte a parâmetros de consulta OData e para `$top` ajudar a personalizar a `$filter` resposta.</span><span class="sxs-lookup"><span data-stu-id="58d9c-119">This method supports `$skiptoken`, `$top` and `$filter` OData query parameters to help customize the response.</span></span> <span data-ttu-id="58d9c-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="58d9c-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="58d9c-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="58d9c-121">Request headers</span></span>

| <span data-ttu-id="58d9c-122">Nome</span><span class="sxs-lookup"><span data-stu-id="58d9c-122">Name</span></span>          | <span data-ttu-id="58d9c-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="58d9c-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="58d9c-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="58d9c-124">Authorization</span></span> | <span data-ttu-id="58d9c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="58d9c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="58d9c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="58d9c-127">Request body</span></span>

<span data-ttu-id="58d9c-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="58d9c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="58d9c-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="58d9c-129">Response</span></span>

<span data-ttu-id="58d9c-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [cloudPcAuditEvent](../resources/cloudpcauditevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="58d9c-130">If successful, this method returns a `200 OK` response code and a collection of [cloudPcAuditEvent](../resources/cloudpcauditevent.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="58d9c-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="58d9c-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="58d9c-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="58d9c-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="58d9c-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="58d9c-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_cloudpcauditevent"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/auditEvents
```
# <a name="c"></a>[<span data-ttu-id="58d9c-134">C#</span><span class="sxs-lookup"><span data-stu-id="58d9c-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-cloudpcauditevent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="58d9c-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="58d9c-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-cloudpcauditevent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="58d9c-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="58d9c-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-cloudpcauditevent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="58d9c-137">Java</span><span class="sxs-lookup"><span data-stu-id="58d9c-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-cloudpcauditevent-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="58d9c-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="58d9c-138">Response</span></span>

><span data-ttu-id="58d9c-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="58d9c-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcAuditEvent",
  "isCollection": true
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.cloudPcAuditEvent",
      "id": "250473f5-029f-4037-813d-ba4768201d61",
      "displayName": "Display Name value",
      "componentName": "Component Name value",  
      "activity": "Activity value",  
      "activityDateTime": "2021-02-14T13:10:51.814636+08:00",  
      "activityType": " Activity Type value",  
      "activityOperationType": "Activity Operation Type value",  
      "activityResult": "Activity Result value",  
      "correlationId": "a5c71cc6-2271-4d5c-9bfe-d94781e83fe6",  
      "category": "Category value",
      "actor": {
          "@odata.type": "microsoft.graph.cloudPcAuditActor",
          "type": "Type value",
          "userPermissions": [
              "User Permissions value"
          ],
          "applicationId": "Application Id value",
          "applicationDisplayName": "Application Display Name value",
          "userPrincipalName": "User Principal Name value",
          "servicePrincipalName": "Service Principal Name value",
          "ipAddress": "Ip Address value",
          "userId": "User Id value",
          "userRoleScopeTags": [
              {
                  "@odata.type": "microsoft.graph.cloudPcUserRoleScopeTagInfo",
                  "displayName": "Display Name value",
                  "roleScopeTagId": "Role Scope Tag Id value"
              }
          ],
          "remoteTenantId": "Remote Tenant Id value",
          "remoteUserId": "Remote User Id value"
      },
      "resources": [
        {
          "@odata.type": "microsoft.graph.cloudPcAuditResource",
          "displayName": "Display Name value",
          "modifiedProperties": [
            {
              "@odata.type": "microsoft.graph.cloudPcAuditProperty",
              "displayName": "Display Name value",
              "oldValue": "Old Value value",
              "newValue": "New Value value"
            }
          ],
          "type": "Type value",
          "resourceId": "Resource Id value"
        }
      ],
    }
  ]
}
```
