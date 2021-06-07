---
title: Listar auditEvents
description: Listar propriedades e relações dos objetos auditEvent.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f4cc59d8bcfaa266ff9239df74b704994ddc209c
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757435"
---
# <a name="list-auditevents"></a><span data-ttu-id="1cbd3-103">Listar auditEvents</span><span class="sxs-lookup"><span data-stu-id="1cbd3-103">List auditEvents</span></span>

<span data-ttu-id="1cbd3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1cbd3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1cbd3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1cbd3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1cbd3-106">Listar propriedades e relações dos objetos [auditEvent](../resources/intune-auditing-auditevent.md).</span><span class="sxs-lookup"><span data-stu-id="1cbd3-106">List properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1cbd3-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1cbd3-107">Prerequisites</span></span>
<span data-ttu-id="1cbd3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1cbd3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1cbd3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1cbd3-110">Permission type</span></span>|<span data-ttu-id="1cbd3-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1cbd3-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1cbd3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1cbd3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1cbd3-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1cbd3-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1cbd3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1cbd3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1cbd3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1cbd3-115">Not supported.</span></span>|
|<span data-ttu-id="1cbd3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1cbd3-116">Application</span></span>|<span data-ttu-id="1cbd3-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1cbd3-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1cbd3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1cbd3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents
```

## <a name="request-headers"></a><span data-ttu-id="1cbd3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1cbd3-119">Request headers</span></span>
|<span data-ttu-id="1cbd3-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1cbd3-120">Header</span></span>|<span data-ttu-id="1cbd3-121">Valor</span><span class="sxs-lookup"><span data-stu-id="1cbd3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1cbd3-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1cbd3-122">Authorization</span></span>|<span data-ttu-id="1cbd3-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1cbd3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1cbd3-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1cbd3-124">Accept</span></span>|<span data-ttu-id="1cbd3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1cbd3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1cbd3-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1cbd3-126">Request body</span></span>
<span data-ttu-id="1cbd3-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1cbd3-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1cbd3-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="1cbd3-128">Response</span></span>
<span data-ttu-id="1cbd3-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [auditEvent](../resources/intune-auditing-auditevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1cbd3-129">If successful, this method returns a `200 OK` response code and a collection of [auditEvent](../resources/intune-auditing-auditevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1cbd3-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1cbd3-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="1cbd3-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1cbd3-131">Request</span></span>
<span data-ttu-id="1cbd3-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1cbd3-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/auditEvents
```

### <a name="response"></a><span data-ttu-id="1cbd3-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="1cbd3-133">Response</span></span>
<span data-ttu-id="1cbd3-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1cbd3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




