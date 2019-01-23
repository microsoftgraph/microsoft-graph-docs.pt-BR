---
title: Listar auditEvents
description: Listar propriedades e relações dos objetos auditEvent.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b16ddbf9a4b110afe172ced3ba9fdccc52b8e80c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409535"
---
# <a name="list-auditevents"></a><span data-ttu-id="72200-103">Listar auditEvents</span><span class="sxs-lookup"><span data-stu-id="72200-103">List auditEvents</span></span>

> <span data-ttu-id="72200-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="72200-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="72200-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="72200-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="72200-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="72200-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="72200-107">Listar propriedades e relações dos objetos [auditEvent](../resources/intune-auditing-auditevent.md).</span><span class="sxs-lookup"><span data-stu-id="72200-107">List properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="72200-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="72200-108">Prerequisites</span></span>
<span data-ttu-id="72200-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="72200-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="72200-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="72200-111">Permission type</span></span>|<span data-ttu-id="72200-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="72200-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="72200-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="72200-113">Delegated (work or school account)</span></span>|<span data-ttu-id="72200-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="72200-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="72200-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="72200-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="72200-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="72200-116">Not supported.</span></span>|
|<span data-ttu-id="72200-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="72200-117">Application</span></span>|<span data-ttu-id="72200-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="72200-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="72200-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="72200-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents
```

## <a name="request-headers"></a><span data-ttu-id="72200-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="72200-120">Request headers</span></span>
|<span data-ttu-id="72200-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="72200-121">Header</span></span>|<span data-ttu-id="72200-122">Valor</span><span class="sxs-lookup"><span data-stu-id="72200-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="72200-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="72200-123">Authorization</span></span>|<span data-ttu-id="72200-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="72200-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="72200-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="72200-125">Accept</span></span>|<span data-ttu-id="72200-126">application/json</span><span class="sxs-lookup"><span data-stu-id="72200-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="72200-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="72200-127">Request body</span></span>
<span data-ttu-id="72200-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="72200-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="72200-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="72200-129">Response</span></span>
<span data-ttu-id="72200-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [auditEvent](../resources/intune-auditing-auditevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="72200-130">If successful, this method returns a `200 OK` response code and a collection of [auditEvent](../resources/intune-auditing-auditevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72200-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="72200-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="72200-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="72200-132">Request</span></span>
<span data-ttu-id="72200-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="72200-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/auditEvents
```

### <a name="response"></a><span data-ttu-id="72200-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="72200-134">Response</span></span>
<span data-ttu-id="72200-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="72200-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




