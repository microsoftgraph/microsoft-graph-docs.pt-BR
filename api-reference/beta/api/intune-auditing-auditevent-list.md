---
title: Listar auditEvents
description: Listar propriedades e relações dos objetos auditEvent.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 979d8b9a9a045d99733ccdf5389510069ab21b74
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30165797"
---
# <a name="list-auditevents"></a><span data-ttu-id="02028-103">Listar auditEvents</span><span class="sxs-lookup"><span data-stu-id="02028-103">List auditEvents</span></span>

> <span data-ttu-id="02028-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="02028-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="02028-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="02028-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02028-106">Listar propriedades e relações dos objetos [auditEvent](../resources/intune-auditing-auditevent.md).</span><span class="sxs-lookup"><span data-stu-id="02028-106">List properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="02028-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="02028-107">Prerequisites</span></span>
<span data-ttu-id="02028-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="02028-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="02028-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="02028-110">Permission type</span></span>|<span data-ttu-id="02028-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="02028-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="02028-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="02028-112">Delegated (work or school account)</span></span>|<span data-ttu-id="02028-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="02028-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="02028-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="02028-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="02028-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02028-115">Not supported.</span></span>|
|<span data-ttu-id="02028-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="02028-116">Application</span></span>|<span data-ttu-id="02028-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02028-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="02028-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="02028-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents
```

## <a name="request-headers"></a><span data-ttu-id="02028-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="02028-119">Request headers</span></span>
|<span data-ttu-id="02028-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="02028-120">Header</span></span>|<span data-ttu-id="02028-121">Valor</span><span class="sxs-lookup"><span data-stu-id="02028-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="02028-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="02028-122">Authorization</span></span>|<span data-ttu-id="02028-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="02028-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="02028-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="02028-124">Accept</span></span>|<span data-ttu-id="02028-125">application/json</span><span class="sxs-lookup"><span data-stu-id="02028-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="02028-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="02028-126">Request body</span></span>
<span data-ttu-id="02028-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="02028-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="02028-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="02028-128">Response</span></span>
<span data-ttu-id="02028-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [auditEvent](../resources/intune-auditing-auditevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="02028-129">If successful, this method returns a `200 OK` response code and a collection of [auditEvent](../resources/intune-auditing-auditevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02028-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="02028-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="02028-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="02028-131">Request</span></span>
<span data-ttu-id="02028-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="02028-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/auditEvents
```

### <a name="response"></a><span data-ttu-id="02028-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="02028-133">Response</span></span>
<span data-ttu-id="02028-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="02028-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1632

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
        "userId": "User Id value"
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




