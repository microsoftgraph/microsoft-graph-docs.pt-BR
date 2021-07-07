---
title: Obter cloudPcAuditEvent
description: Leia as propriedades e as relações de um objeto cloudPcAuditEvent.
author: ecmadao
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 9dc44e92d4e332a2e682c25f525d72faa7a62847
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2021
ms.locfileid: "53316871"
---
# <a name="get-cloudpcauditevent"></a><span data-ttu-id="b92c7-103">Obter cloudPcAuditEvent</span><span class="sxs-lookup"><span data-stu-id="b92c7-103">Get cloudPcAuditEvent</span></span>

<span data-ttu-id="b92c7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b92c7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b92c7-105">Leia as propriedades e as relações de um [objeto cloudPcAuditEvent.](../resources/cloudpcauditevent.md)</span><span class="sxs-lookup"><span data-stu-id="b92c7-105">Read the properties and relationships of a [cloudPcAuditEvent](../resources/cloudpcauditevent.md) object.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="b92c7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b92c7-106">Permissions</span></span>

<span data-ttu-id="b92c7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b92c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b92c7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b92c7-109">Permission type</span></span>| <span data-ttu-id="b92c7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b92c7-110">Permissions (from least to most privileged)</span></span> |
|:---|:---|
|<span data-ttu-id="b92c7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b92c7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b92c7-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b92c7-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="b92c7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b92c7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b92c7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b92c7-114">Not supported.</span></span>|
|<span data-ttu-id="b92c7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b92c7-115">Application</span></span>|<span data-ttu-id="b92c7-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b92c7-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b92c7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b92c7-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/auditEvents/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b92c7-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b92c7-118">Request headers</span></span>

| <span data-ttu-id="b92c7-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b92c7-119">Name</span></span>          | <span data-ttu-id="b92c7-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b92c7-120">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="b92c7-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b92c7-121">Authorization</span></span> | <span data-ttu-id="b92c7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b92c7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b92c7-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b92c7-124">Request body</span></span>

<span data-ttu-id="b92c7-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b92c7-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b92c7-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="b92c7-126">Response</span></span>

<span data-ttu-id="b92c7-127">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [cloudPcAuditEvent](../resources/cloudpcauditevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b92c7-127">If successful, this method returns a `200 OK` response code and a [cloudPcAuditEvent](../resources/cloudpcauditevent.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b92c7-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b92c7-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b92c7-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b92c7-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="b92c7-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="b92c7-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_cloudpcauditevent"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/auditEvents/{id}
```
# <a name="c"></a>[<span data-ttu-id="b92c7-131">C#</span><span class="sxs-lookup"><span data-stu-id="b92c7-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-cloudpcauditevent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b92c7-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b92c7-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-cloudpcauditevent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b92c7-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b92c7-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-cloudpcauditevent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b92c7-134">Java</span><span class="sxs-lookup"><span data-stu-id="b92c7-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-cloudpcauditevent-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b92c7-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="b92c7-135">Response</span></span>

><span data-ttu-id="b92c7-136">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b92c7-136">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcAuditEvent"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
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
}
```
