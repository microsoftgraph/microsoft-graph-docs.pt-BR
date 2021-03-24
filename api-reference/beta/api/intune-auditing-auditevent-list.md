---
title: Listar auditEvents
description: Listar propriedades e relações dos objetos auditEvent.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 10bde94668b7814d1ed110f5da8dab5a7daad3ef
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51131894"
---
# <a name="list-auditevents"></a><span data-ttu-id="b28f9-103">Listar auditEvents</span><span class="sxs-lookup"><span data-stu-id="b28f9-103">List auditEvents</span></span>

<span data-ttu-id="b28f9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b28f9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b28f9-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b28f9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b28f9-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b28f9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b28f9-107">Listar propriedades e relações dos objetos [auditEvent](../resources/intune-auditing-auditevent.md).</span><span class="sxs-lookup"><span data-stu-id="b28f9-107">List properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b28f9-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b28f9-108">Prerequisites</span></span>
<span data-ttu-id="b28f9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b28f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b28f9-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b28f9-111">Permission type</span></span>|<span data-ttu-id="b28f9-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b28f9-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b28f9-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b28f9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b28f9-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b28f9-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b28f9-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b28f9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b28f9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b28f9-116">Not supported.</span></span>|
|<span data-ttu-id="b28f9-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b28f9-117">Application</span></span>|<span data-ttu-id="b28f9-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b28f9-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b28f9-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b28f9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents
```

## <a name="request-headers"></a><span data-ttu-id="b28f9-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b28f9-120">Request headers</span></span>
|<span data-ttu-id="b28f9-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b28f9-121">Header</span></span>|<span data-ttu-id="b28f9-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b28f9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b28f9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b28f9-123">Authorization</span></span>|<span data-ttu-id="b28f9-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b28f9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b28f9-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b28f9-125">Accept</span></span>|<span data-ttu-id="b28f9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b28f9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b28f9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b28f9-127">Request body</span></span>
<span data-ttu-id="b28f9-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b28f9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b28f9-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b28f9-129">Response</span></span>
<span data-ttu-id="b28f9-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [auditEvent](../resources/intune-auditing-auditevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b28f9-130">If successful, this method returns a `200 OK` response code and a collection of [auditEvent](../resources/intune-auditing-auditevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b28f9-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b28f9-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b28f9-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b28f9-132">Request</span></span>
<span data-ttu-id="b28f9-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b28f9-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/auditEvents
```

### <a name="response"></a><span data-ttu-id="b28f9-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b28f9-134">Response</span></span>
<span data-ttu-id="b28f9-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b28f9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1975

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.auditEvent",
      "id": "59653ce8-3ce8-5965-e83c-6559e83c6559",
      "displayName": "Display Name value",
      "componentName": "Component Name value",
      "actor": {
        "@odata.type": "microsoft.graph.auditActor",
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
            "@odata.type": "microsoft.graph.roleScopeTagInfo",
            "displayName": "Display Name value",
            "roleScopeTagId": "Role Scope Tag Id value"
          }
        ],
        "remoteTenantId": "Remote Tenant Id value",
        "remoteUserId": "Remote User Id value"
      },
      "activity": "Activity value",
      "activityDateTime": "2016-12-31T23:59:51.6363086-08:00",
      "activityType": "Activity Type value",
      "activityOperationType": "Activity Operation Type value",
      "activityResult": "Activity Result value",
      "correlationId": "52effe71-fe71-52ef-71fe-ef5271feef52",
      "resources": [
        {
          "@odata.type": "microsoft.graph.auditResource",
          "displayName": "Display Name value",
          "modifiedProperties": [
            {
              "@odata.type": "microsoft.graph.auditProperty",
              "displayName": "Display Name value",
              "oldValue": "Old Value value",
              "newValue": "New Value value"
            }
          ],
          "type": "Type value",
          "resourceId": "Resource Id value"
        }
      ],
      "category": "Category value"
    }
  ]
}
```




